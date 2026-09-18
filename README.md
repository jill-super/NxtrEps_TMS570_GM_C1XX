# Electric Power Steering (EPS) System for GM C1XX

[![Deploy docs to GitHub Pages](../../actions/workflows/deploy.yml/badge.svg)](../../actions/workflows/deploy.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)
![Language: C](https://img.shields.io/badge/language-C-blue.svg)
![Platform: TI TMS570](https://img.shields.io/badge/platform-TI_TMS570-red.svg)
![Standard: AUTOSAR](https://img.shields.io/badge/standard-AUTOSAR-green.svg)
![Safety: ISO 26262 ASIL D](https://img.shields.io/badge/safety-ISO_26262_ASIL_D-orange.svg)
![Docs: Astro + Starlight](https://img.shields.io/badge/docs-Astro_Starlight-purple.svg)

Complete **Electric Power Steering (EPS)** firmware for the **GM C1XX** platform
(Cadillac XT5/XT6, Chevrolet Traverse, Buick Enclave, GMC Acadia) on the
**Texas Instruments TMS570** (ARM Cortex-R4), developed to **AUTOSAR** and
**ISO 26262 ASIL D**. Implements torque sensing, power-assisted steering
control, motor control, diagnostics (UDS/CAN) and manufacturing services.

> **Documentation site:** after enabling GitHub Pages (see
> [Deployment](#documentation-website) below), the full documentation is
> published at `https://<owner>.github.io/<repo>/`
> (the workflow derives the URL from the repository itself, so forks work
> without changes). The site source lives in [`docs/`](./docs).

## Table of contents

- [Features](#features)
- [Repository structure](#repository-structure)
- [AUTOSAR layers and modules](#autosar-layers-and-modules)
- [Vector vs. in-house code](#vector-vs-in-house-code)
- [Installation and build](#installation-and-build)
- [Documentation website](#documentation-website)
- [Testing](#testing)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Key components**:
  - **Texas Instruments TMS570**: the microcontroller used for EPS control.
  - **AUTOSAR**: the software development standard for automotive embedded systems.
  - **ISO 26262 ASIL D**: the functional safety standard for automotive systems.
  - **CAN**: Controller Area Network, a communication protocol for automotive systems.
  - **UDS**: on-board diagnostics protocol.
- **Functionality**:
  - Precise power-assisted steering control.
  - Electric motor power management.
  - Hands-on/off-wheel detection, return/damping/firewall torque functions.
  - End-of-travel management, thermal duty cycle, power-limit functions.

## Repository structure

```text
<repo root>/
  <Module>/            # one folder per SW-C / driver / library
    autosar/           # AUTOSAR model (.arxml) and RTE templates
    doc/               # original design docs (.docx/.doc/.pdf) — converted into the site
    generate/          # DaVinci/ARTT generation templates (*.tt, *_Generate.bat)
    src/ / include/    # C sources and headers
    tools/             # RteGen.bat / Integrate.bat per-module scripts
    utp/               # unit-test artefacts (Tessy reports)
  GM_C1XX_EPS_TMS570/  # ECU integration project (SwProject, RTE/BSW config, tools, HLDD)
  docs/                # documentation website source (Astro v7 + Starlight project root)
  .github/workflows/   # Pages deployment + Dependabot auto-merge
  LICENSE              # MIT License
```

Each module follows the same layout, so once you know one `Ap_*` component
(e.g. [`Assist/`](./Assist)) you know them all. The full per-module reference —
purpose, key files, public API, dependencies and converted design documents —
is published on the documentation site (see [below](#documentation-website)).

## AUTOSAR layers and modules

The firmware is organised into AUTOSAR layers. Each table below lists the
module short name (directory name) together with its full descriptive name.
Origin legend: **Custom** = Nexteer in-house; **Vector** = Vector
MICROSAR/provided code; **TI**/**Gliwa** = third-party drivers/tools.
Sections containing only in-house modules state the origin once instead of
repeating it on every row.

Click a layer to expand its module list.

<details>
<summary><strong>Application Software (ASW)</strong> — AUTOSAR application SW-Cs (<code>Ap_*</code>), diagnostics, state management (49 modules, all Custom in-house)</summary>

| Module | Full name |
| --- | --- |
| AbsHwPos_TcI2cVd | Absolute Handwheel Position (TC I2C VD) |
| ActivePull | Active Pull Compensation |
| Assist | Base Assist |
| AssistFirewall | Assist Firewall |
| AstLmt_CM | Assist Sum Limit, Current Mode |
| AvgFricLrn | Average Friction Learning |
| BVDiag | Battery Voltage Diagnostics |
| BatteryVoltage | Battery Voltage |
| ComplErr | Compliance Error |
| CtrldDisShtdn | Controlled Disable Shutdown |
| Damping | Damping |
| DampingFirewall | Damping Firewall |
| DiagMgr | Diagnostic Manager |
| EOTActuatorMng | End-of-Travel Actuator Management |
| EtDmpFw | End-of-Travel Damping Firewall |
| FltInjection | Fault Injection |
| FrqDepDmpnInrtCmp | Frequency-Dependent Damping and Inertia Compensation |
| GMSrlComOutput | Serial Communication Output |
| GMStrtStop | GM Start-Stop |
| GenPosTraj | General Position Trajectory |
| HOWDetect | Hands-On-Wheel Detection |
| HiLoadStall | High-Load Stall |
| HighFreqAssist | High-Frequency Assist |
| HwPwUp | Hardware Power-Up |
| HystComp | Hysteresis Compensation |
| LmtCod | Limiter Conditioning |
| LrnEOT | Learn End-of-Travel |
| MtrTempEst | Motor Temperature Estimation |
| Polarity | Polarity |
| PosServo | Position Servo |
| PwrLmtFuncCr | Power Limit Function, Current Mode |
| Return | Return |
| ReturnFirewall | Return Firewall |
| SF46_GCCDiag_Implementation | GCC Diagnostics, SF46 |
| SF47_TSMit_Implementation | Torque Steer Mitigation, SF47 |
| SgnlCond | Signal Conditioning |
| StOpCtrl | State Output Control |
| StaMd | States and Modes |
| StabilityComp | Stability Compensation |
| Sweep | Sweep |
| ThrmDutyCycle | Thermal Duty Cycle |
| TqRsDg | Torque Reasonableness Diagnostics |
| TrqArblim | Torque Arbitration and Limiting |
| TrqOsc | Torque Oscillation Function, Current Mode |
| TrqOvlSta | Torque Overlay Status |
| TuningSelAuth | Tuning Select Authority |
| VehDyn | Vehicle Dynamics |
| VehSpdLmt | Vehicle Speed Limit |
| WhlImbRej | Wheel Imbalance Rejection |

</details>

<details>
<summary><strong>Sensor / Actuator Abstraction</strong> — SW-Cs (<code>Sa_*</code>) and associated diagnostics (11 modules, all Custom in-house)</summary>

| Module | Full name |
| --- | --- |
| BkCpPc | Bulk Capacitor Precharge |
| CmMtrCurr | Common Motor Current |
| CtrlTemp | Controller Temperature |
| DigColPs | Digital Column Position |
| DigHwTrqSENT | Digital Handwheel Torque via SENT |
| DigMSB | Digital MSB Interface |
| MtrVel_Digi | Motor Velocity, Digital |
| OvrVoltMon | Overvoltage Monitor |
| SVDiag | Motor-Drive Diagnostics (incl. Digital Phase Reasonableness) |
| ShtdnMech | Shutdown Mechanisms |
| TmprlMon | Temporal Monitor |

</details>

<details>
<summary><strong>Complex Device Drivers (CDD)</strong> — motor-control / power-stage drivers (<code>Cd_*</code>) (4 modules, all Custom in-house)</summary>

| Module | Full name |
| --- | --- |
| MtrCtrl_CM | Motor Control, Current Mode |
| NvMProxy | NVRAM Proxy |
| SVDrvr_CM | Space-Vector PWM Driver, Current Mode |
| TMS570_uDiag | TMS570 Micro Diagnostics |

</details>

<details>
<summary><strong>Basic Software (BSW)</strong> — Vector MICROSAR stack, memory stack, XCP, ECU services</summary>

| Module | Full name | Origin |
| --- | --- | --- |
| Fee | Flash EEPROM Emulation | TI |
| NvMMgr | NVRAM Manager (Fee Interface) | Custom |
| Xcp | XCP Measurement and Calibration SW-C | Custom |
| `SwProject/Source/GenData*` (GenData, GenDataRte, GenDataOS) | DaVinci-Generated Configuration Data | Vector |
| `SwProject/Source/BSW/Can` | CAN Driver | Vector |
| `SwProject/Source/BSW/ComM` | Communication Manager | Vector |
| `SwProject/Source/BSW/Crc` | CRC Library | Vector |
| `SwProject/Source/BSW/Dem` | Diagnostic Event Manager | Vector |
| `SwProject/Source/BSW/Det` | Development Error Tracer | Vector |
| `SwProject/Source/BSW/Diag` | Diagnostic Gateway (ggda, project-specific) | Custom |
| `SwProject/Source/BSW/Dio` | Digital I/O Driver | Vector |
| `SwProject/Source/BSW/EcuM` | ECU State Manager | Vector |
| `SwProject/Source/BSW/Gpt` | General Purpose Timer Driver | Vector |
| `SwProject/Source/BSW/Il` | Interaction Layer | Vector |
| `SwProject/Source/BSW/IoHwAb` | I/O Hardware Abstraction | Vector |
| `SwProject/Source/BSW/Mcu` | MCU Driver | Vector |
| `SwProject/Source/BSW/MemIf` | Memory Abstraction Interface | Vector |
| `SwProject/Source/BSW/Nm` | GM Network Management (gmnm, project-specific) | Custom |
| `SwProject/Source/BSW/NvM` | NVRAM Manager | Vector |
| `SwProject/Source/BSW/Os` | OSEK Operating System | Vector |
| `SwProject/Source/BSW/Port` | Port Driver | Vector |
| `SwProject/Source/BSW/Tp` | Transport Protocol | Vector |
| `SwProject/Source/BSW/VStdLib` | Vector Standard Library | Vector |
| `SwProject/Source/BSW/Wdg` | Watchdog Driver (TMS570LS3x) | Vector |
| `SwProject/Source/BSW/WdgIf` | Watchdog Interface | Vector |
| `SwProject/Source/BSW/WdgM` | Watchdog Manager | Vector |
| `SwProject/Source/BSW/Xcp` | XCP Protocol Stack (XcpProf, xcp_can) | Vector |
| `SwProject/Source/BSW/_Common` | Common Headers (Std_Types, Compiler, MemMap, Platform_Types) | Vector |

</details>

<details>
<summary><strong>MCAL & MCU drivers</strong> — on-chip peripheral drivers, startup code, platform types (8 modules)</summary>

| Module | Full name | Origin |
| --- | --- | --- |
| Adc | Analog-to-Digital Converter Driver | Custom |
| Dma | Direct Memory Access Driver | Custom |
| Fls | Flash Driver (TI F021 Flash API) | TI |
| I2cNxtr | I2C Driver, Nexteer | Custom |
| SpiNxt | SPI Driver, Nexteer | Custom |
| StdDef | Standard Definitions | Custom |
| TMS570_Startup | TMS570 Startup Code | Custom |
| ePWM | Enhanced PWM / NHET Driver | Custom |

</details>

<details>
<summary><strong>RTE & system integration</strong></summary>

| Module | Full name | Origin |
| --- | --- | --- |
| GM_C1XX_EPS_TMS570 | ECU Integration Project (SwProject: RTE, BSW configuration, SW-C integration, linker script, post-build tools) | Custom integration + Vector generated code |

</details>

<details>
<summary><strong>Libraries & common</strong> (5 modules)</summary>

| Module | Full name | Origin |
| --- | --- | --- |
| CMS_Common | CMS Common Utilities | Custom |
| GliwaT1 | Timing-Measurement Support (Gliwa T1) | Gliwa |
| Metrics | Execution-Time Metrics | Custom |
| NxtrLib | Nexteer Math Library (filters, interpolation, fixed-point math) | Custom |
| QAC | MISRA Compliance Configuration (PRQA QAC) | Third-party |

</details>

## Vector vs. in-house code

- **Custom (Nexteer in-house):** all `Ap_*` / `Sa_*` / `Cd_*` application
  modules, MCAL drivers and libraries. A file is in-house unless its header
  says otherwise.
- **Vector-provided:** the MICROSAR BSW stack and all DaVinci-generated
  artefacts — recognisable by the header
  `This software is copyright protected and proprietary to Vector Informatik GmbH`,
  or by location under
  `GM_C1XX_EPS_TMS570/SwProject/Source/{BSW,GenData,GenDataRte,GenDataOS}`.
  RTE contract stubs (`utp/contract/`, `tools/contract/`) and DaVinci files
  (`.arxml`, `.dcf`, `generate/*.tt`) are Vector-generated scaffolding around
  in-house code — do not edit them by hand.
- **Third-party:** TI (`Fee`, `Fls`), Gliwa (`GliwaT1`), PRQA (`QAC`).

The documentation site marks every module page with an origin badge and
provides the full matrix under *General → Vector vs. custom code*.

## Installation and build

### Prerequisites

- TI ARM compiler toolchain (`hex470`, see
  `GM_C1XX_EPS_TMS570/Tools/`) for the TMS570 target.
- Vector DaVinci Configurator / Developer for RTE/BSW generation.
- Windows host for the `*.bat` integration scripts
  (`tools/Integrate.bat`, `tools/RteGen.bat`, `SwProject/postbuild.bat`).
- Node.js 22+ only for building this repository's documentation website.

### Firmware build (typical flow)

1. Clone this repository.
2. Generate the RTE/BSW configuration with DaVinci Configurator into
   `GM_C1XX_EPS_TMS570/SwProject/Source/GenData*`.
3. Generate each SW-C via its `generate/*_Generate.bat` / `.tt` templates
   (ARTT framework, see each module's Integration Manual on the docs site).
4. Compile the TMS570 sources with the TI ARM compiler.
5. Link with `GM_C1XX_EPS_TMS570/SwProject/TMS570LS202x6SFlashLnk.cmd`,
   then run `postbuild.bat` / `HexView`.
6. Flash the resulting image onto the TMS570 ECU.

Per-module integration steps are documented in each module's
*Integration Manual* (published on the docs site from the original
`doc/*.docx` files).

### Documentation website (local preview)

```bash
cd docs
npm install
npm run dev      # preview with hot reload
npm run build    # production build into docs/dist/
```

Requires Node.js 22.12 or later (Astro 7 requirement).

## Documentation website

The full reference — AUTOSAR layer overviews, one page per module (purpose,
key files, public API, dependencies, origin badge), all converted
`doc/*.docx` / `*.pdf` / `*.txt` design documents, build-system notes, safety
notes and unit-test reports — is built with **Astro v7 + Starlight** from the
[`docs/`](./docs) folder and deployed to **GitHub Pages** on every push to the
default branch:

- Workflow: [`.github/workflows/deploy.yml`](./.github/workflows/deploy.yml)
- Enable it once under **Settings → Pages → Build and deployment → Source:
  GitHub Actions**. No code changes are needed: the site URL is derived from
  the repository itself, so forks deploy to their own Pages URL automatically.
- Deployment is gated on repository visibility: the workflow deploys only when
  the repository is public (GitHub Pages deployment from Actions is a public
  feature gate built into `deploy.yml`), and it builds only when `docs/`
  content or the workflow itself changes.

## Testing

- Unit-test artefacts (Tessy reports, `index_WithPS` / `index_WithOutPS`)
  live in each module's `utp/` folder and are catalogued on the docs site
  under *General → Unit-test reports*.
- The docs site itself is validated in CI (`npm install && npm run build`
  inside `docs/`); Dependabot updates are auto-merged only when that build
  passes (see `.github/workflows/auto-merge-dependabot.yml`).

## Contributing

We encourage contributions! If you'd like to improve this project, please
submit a pull request. Please keep Vector-provided and third-party files
untouched, and keep module documentation (`doc/`) in sync with code changes.

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE)
file for the full text.
