# Validation Summary

Test date: November 1, 2026.

The integration tests exercised the path from simulated decoy detections through automatic notification and optical reception to a latched cutoff state and saved Windows reports.

## Software checks

The decoy and notification software passed 16 tests covering scheduled activity handling, notification processing, and logging.

The Windows receiver application passed a separate set of 16 self-tests covering input processing, logging, and related application behavior.

## Hardware integration

| Observation | Result |
| --- | --- |
| Simulated detections | Six categories exercised |
| Automatic notification | Transmitter-side behavior verified for all six categories |
| Optical emergency events | Six new events recorded at the receiver |
| Receiver state | Cutoff state remained latched after emergency reception |
| Report logging | 53 reports across the six categories recorded in the evaluated receiver-log period |

Transmitter-side hardware records were reconciled with the receiver-log summary supplied from the separate PC. The trials used simulated detection events; no live malware was used.

## Evidence scope

The counts above are aggregate results from the tested experimental configuration. Receiver state refers to the controller state recorded in the logs. These observations characterize this prototype and test run, rather than a general security effectiveness rating or a product certification.

[Back to the project](README.md)
