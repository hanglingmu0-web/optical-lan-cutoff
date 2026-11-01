# System Overview

Optical LAN Cutoff brings together detection, optical notification, hardware power control, and logging on a separate computer.

## Components

| Component | Role |
| --- | --- |
| Decoy host | Runs decoys, simulates activity, and produces detection events |
| Notification bridge | Passes detection events to the transmitter |
| Arduino transmitter | Sends emergency signals and compact reports over the optical path |
| Arduino receiver | Receives optical notifications and controls the relay |
| Relay and LAN switch | Provide the controlled network power path |
| Windows receiver application | Displays receiver events and saves reports on a separate PC |
| External detection intake | Accepts notifications from other security tools |

## Information flow

Detection events travel from the decoy host toward the receiver through a one-way optical path. The receiver handles LAN switch power control locally and forwards event information to the Windows application over USB.

Emergency signaling and reporting share the optical path. After an emergency event, the receiver holds the cutoff state while reports continue to arrive and are saved on the separate PC.

## Hardware photograph

The [test-bench photograph](hardware-prototype.jpg) shows the hardware prototype with the earlier phone-based relay-control interface. The [validation summary](VALIDATION.md) describes the later integration tests using the Windows receiver application.

[Back to the project](README.md)
