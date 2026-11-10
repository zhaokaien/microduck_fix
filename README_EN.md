# MicroDuck Replica Guide

**A beginner-first troubleshooting and build guide for MicroDuck replicas using Radxa Zero 3W, the RPI Robot HAT, `imu_to_dxl`, and 15 Feetech HD-1910 servos.**

[简体中文](README.md) · [Full documentation index](docs/README.md)

> This is an independent third-party project for personal, non-commercial learning and research. It is not affiliated with or endorsed by Pollen Robotics.

**Current status:** the HAT and `imu_to_dxl` designs have been studied; Radxa Zero 3W boots; the servos and 3D-printed structure are assembled. Bus integration, calibration, full-robot motion, and training validation are in progress.

## What this repository is for

`microduck_fix` is an independent, hands-on troubleshooting and navigation guide for people building a MicroDuck replica. It records research, procedures, failure modes, fixes, and verification results across the HAT board, `imu_to_dxl`, Radxa Zero 3W, Feetech servos, 3D-printed assembly, and reinforcement learning.

The repository focuses on:

- A beginner-first build route from part selection to the first stable walking test.
- Problem-based entry points for boot failures, servo issues, frame drops, IMU errors, and overheating.
- Reproducible notes that separate confirmed results from untested assumptions.
- Explanations of power delivery, servo buses, IMU mounting, control loops, ONNX policies, and sim2real.
- Navigation to the official project and the fanhao and kissqy replica repositories.

It supplements upstream hardware, firmware, and training projects rather than replacing them.

## Start by problem

| Your situation | Start here |
|---|---|
| Choosing servos and parts | [Hardware selection](docs/build/hardware-selection.md) |
| Building or checking the HAT | [HAT board](docs/build/hat-board.md) |
| Connecting the body IMU | [IMU_TO_DXL](docs/build/imu-to-dxl.md) |
| Board will not boot | [Radxa boot and SD card](docs/troubleshooting/radxa-boot.md) |
| Servo ID or calibration problems | [Servo calibration](docs/troubleshooting/servo-calibration.md) |
| Frame drops or random resets | [Bus troubleshooting](docs/troubleshooting/frame-drop.md) |
| Preparing reinforcement learning | [Training roadmap](docs/build/training.md) |
| Robot can stand but not walk | [Integration guide](docs/build/integration.md) |

## Documentation structure

```text
L1  README: identify your current problem
L2  Task page: choose a build, troubleshooting, or principle area
L3  Article: operation, verification, and the underlying principle
```

The detailed guides are currently written in Simplified Chinese. File names, hardware terms, commands, and logs remain in English where useful.

## Main repositories

- [pollen-robotics/microduck](https://github.com/pollen-robotics/microduck)
- [fanhao375/microduck-replica](https://github.com/fanhao375/microduck-replica)
- [kissqy/Microduck-kissqy](https://github.com/kissqy/Microduck-kissqy)

## Community

MicroDuck replica discussion, HAT group purchase, and issue reporting: [Community guide](docs/community/README.md).

If this project saves you time, please Star the repository or share a reproducible test result.
