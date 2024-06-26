# Validate State Report

**Table of Contents:**

- [Validate State Report](validate-state-report)
  - [Test Results Summary](#test-results-summary)
  - [Failed Test Results Summary](#failed-test-results-summary)
  - [All Test Results](#all-test-results)

## Test Results Summary

### Summary Totals

| Total Tests | Total Tests Passed | Total Tests Failed | Total Tests Skipped |
| ----------- | ------------------ | ------------------ | ------------------- |
| 144 | 108 | 6 | 30 |

### Summary Totals Device Under Test

| Device Under Test | Total Tests | Tests Passed | Tests Failed | Tests Skipped | Categories Failed | Categories Skipped |
| ------------------| ----------- | ------------ | ------------ | ------------- | ----------------- | ------------------ |
| s1-leaf1 | 21 | 15 | 1 | 5 | Services | Hardware, LANZ |
| s1-leaf2 | 21 | 15 | 1 | 5 | Services | Hardware, LANZ |
| s1-leaf3 | 21 | 15 | 1 | 5 | Services | Hardware, LANZ |
| s1-leaf4 | 21 | 15 | 1 | 5 | Services | Hardware, LANZ |
| s1-spine1 | 30 | 24 | 1 | 5 | Services | Hardware, LANZ |
| s1-spine2 | 30 | 24 | 1 | 5 | Services | Hardware, LANZ |

### Summary Totals Per Category

| Test Category | Total Tests | Tests Passed | Tests Failed | Tests Skipped |
| ------------- | ----------- | ------------ | ------------ | ------------- |
| Connectivity | 28 | 28 | 0 | 0 |
| Hardware | 24 | 0 | 0 | 24 |
| Interfaces | 56 | 56 | 0 | 0 |
| LANZ | 6 | 0 | 0 | 6 |
| MLAG | 6 | 6 | 0 | 0 |
| Services | 6 | 0 | 6 | 0 |
| Software | 12 | 12 | 0 | 0 |
| System | 6 | 6 | 0 | 0 |

## Failed Test Results Summary

| ID | Device Under Test | Categories | Test | Description | Inputs | Result | Messages |
| -- | ----------------- | ---------- | ---- | ----------- | ------ | -------| -------- |
| 18 | s1-leaf1 | Services | VerifyDNSLookup | Verifies the DNS name to IP address resolution. | - | FAIL | ValueError: "AntaCommand" object has no field "failed" |
| 39 | s1-leaf2 | Services | VerifyDNSLookup | Verifies the DNS name to IP address resolution. | - | FAIL | ValueError: "AntaCommand" object has no field "failed" |
| 60 | s1-leaf3 | Services | VerifyDNSLookup | Verifies the DNS name to IP address resolution. | - | FAIL | ValueError: "AntaCommand" object has no field "failed" |
| 81 | s1-leaf4 | Services | VerifyDNSLookup | Verifies the DNS name to IP address resolution. | - | FAIL | ValueError: "AntaCommand" object has no field "failed" |
| 111 | s1-spine1 | Services | VerifyDNSLookup | Verifies the DNS name to IP address resolution. | - | FAIL | ValueError: "AntaCommand" object has no field "failed" |
| 141 | s1-spine2 | Services | VerifyDNSLookup | Verifies the DNS name to IP address resolution. | - | FAIL | ValueError: "AntaCommand" object has no field "failed" |

## All Test Results

| ID | Device Under Test | Categories | Test | Description | Inputs | Result | Messages |
| -- | ----------------- | ---------- | ---- | ----------- | ------ | -------| -------- |
| 1 | s1-leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet1 - Remote: s1-leaf2 Ethernet1 | PASS | - |
| 2 | s1-leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet2 - Remote: s1-spine1 Ethernet2 | PASS | - |
| 3 | s1-leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet3 - Remote: s1-spine2 Ethernet2 | PASS | - |
| 4 | s1-leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet6 - Remote: s1-leaf2 Ethernet6 | PASS | - |
| 5 | s1-leaf1 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 6 | s1-leaf1 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 7 | s1-leaf1 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 8 | s1-leaf1 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 9 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet1 - MLAG_PEER_s1-leaf2_Ethernet1 = 'up' | PASS | - |
| 10 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet2 - S1-SPINE1_Ethernet2 = 'up' | PASS | - |
| 11 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet3 - S1-SPINE2_Ethernet2 = 'up' | PASS | - |
| 12 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - MLAG_PEER_s1-leaf2_Ethernet6 = 'up' | PASS | - |
| 13 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel1 - MLAG_PEER_s1-leaf2_Po1 = 'up' | PASS | - |
| 14 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel2 - SPINES_Po2 = 'up' | PASS | - |
| 15 | s1-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan4094 - MLAG_PEER = 'up' | PASS | - |
| 16 | s1-leaf1 | LANZ | VerifyLANZ | Verifies if LANZ is enabled. | - | SKIPPED | VerifyLANZ test is not supported on cEOSLab. |
| 17 | s1-leaf1 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 18 | s1-leaf1 | Services | VerifyDNSLookup | Verifies the DNS name to IP address resolution. | - | FAIL | ValueError: "AntaCommand" object has no field "failed" |
| 19 | s1-leaf1 | Software | VerifyEOSVersion | Verifies the EOS version of the device. | - | PASS | - |
| 20 | s1-leaf1 | Software | VerifyTerminAttrVersion | Verifies the TerminAttr version of the device. | - | PASS | - |
| 21 | s1-leaf1 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 22 | s1-leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet1 - Remote: s1-leaf1 Ethernet1 | PASS | - |
| 23 | s1-leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet2 - Remote: s1-spine1 Ethernet3 | PASS | - |
| 24 | s1-leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet3 - Remote: s1-spine2 Ethernet3 | PASS | - |
| 25 | s1-leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet6 - Remote: s1-leaf1 Ethernet6 | PASS | - |
| 26 | s1-leaf2 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 27 | s1-leaf2 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 28 | s1-leaf2 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 29 | s1-leaf2 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 30 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet1 - MLAG_PEER_s1-leaf1_Ethernet1 = 'up' | PASS | - |
| 31 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet2 - S1-SPINE1_Ethernet3 = 'up' | PASS | - |
| 32 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet3 - S1-SPINE2_Ethernet3 = 'up' | PASS | - |
| 33 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - MLAG_PEER_s1-leaf1_Ethernet6 = 'up' | PASS | - |
| 34 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel1 - MLAG_PEER_s1-leaf1_Po1 = 'up' | PASS | - |
| 35 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel2 - SPINES_Po2 = 'up' | PASS | - |
| 36 | s1-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan4094 - MLAG_PEER = 'up' | PASS | - |
| 37 | s1-leaf2 | LANZ | VerifyLANZ | Verifies if LANZ is enabled. | - | SKIPPED | VerifyLANZ test is not supported on cEOSLab. |
| 38 | s1-leaf2 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 39 | s1-leaf2 | Services | VerifyDNSLookup | Verifies the DNS name to IP address resolution. | - | FAIL | ValueError: "AntaCommand" object has no field "failed" |
| 40 | s1-leaf2 | Software | VerifyEOSVersion | Verifies the EOS version of the device. | - | PASS | - |
| 41 | s1-leaf2 | Software | VerifyTerminAttrVersion | Verifies the TerminAttr version of the device. | - | PASS | - |
| 42 | s1-leaf2 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 43 | s1-leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet1 - Remote: s1-leaf4 Ethernet1 | PASS | - |
| 44 | s1-leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet2 - Remote: s1-spine1 Ethernet4 | PASS | - |
| 45 | s1-leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet3 - Remote: s1-spine2 Ethernet4 | PASS | - |
| 46 | s1-leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet6 - Remote: s1-leaf4 Ethernet6 | PASS | - |
| 47 | s1-leaf3 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 48 | s1-leaf3 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 49 | s1-leaf3 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 50 | s1-leaf3 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 51 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet1 - MLAG_PEER_s1-leaf4_Ethernet1 = 'up' | PASS | - |
| 52 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet2 - S1-SPINE1_Ethernet4 = 'up' | PASS | - |
| 53 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet3 - S1-SPINE2_Ethernet4 = 'up' | PASS | - |
| 54 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - MLAG_PEER_s1-leaf4_Ethernet6 = 'up' | PASS | - |
| 55 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel1 - MLAG_PEER_s1-leaf4_Po1 = 'up' | PASS | - |
| 56 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel2 - SPINES_Po4 = 'up' | PASS | - |
| 57 | s1-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan4094 - MLAG_PEER = 'up' | PASS | - |
| 58 | s1-leaf3 | LANZ | VerifyLANZ | Verifies if LANZ is enabled. | - | SKIPPED | VerifyLANZ test is not supported on cEOSLab. |
| 59 | s1-leaf3 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 60 | s1-leaf3 | Services | VerifyDNSLookup | Verifies the DNS name to IP address resolution. | - | FAIL | ValueError: "AntaCommand" object has no field "failed" |
| 61 | s1-leaf3 | Software | VerifyEOSVersion | Verifies the EOS version of the device. | - | PASS | - |
| 62 | s1-leaf3 | Software | VerifyTerminAttrVersion | Verifies the TerminAttr version of the device. | - | PASS | - |
| 63 | s1-leaf3 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 64 | s1-leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet1 - Remote: s1-leaf3 Ethernet1 | PASS | - |
| 65 | s1-leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet2 - Remote: s1-spine1 Ethernet5 | PASS | - |
| 66 | s1-leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet3 - Remote: s1-spine2 Ethernet5 | PASS | - |
| 67 | s1-leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet6 - Remote: s1-leaf3 Ethernet6 | PASS | - |
| 68 | s1-leaf4 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 69 | s1-leaf4 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 70 | s1-leaf4 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 71 | s1-leaf4 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 72 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet1 - MLAG_PEER_s1-leaf3_Ethernet1 = 'up' | PASS | - |
| 73 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet2 - S1-SPINE1_Ethernet5 = 'up' | PASS | - |
| 74 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet3 - S1-SPINE2_Ethernet5 = 'up' | PASS | - |
| 75 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - MLAG_PEER_s1-leaf3_Ethernet6 = 'up' | PASS | - |
| 76 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel1 - MLAG_PEER_s1-leaf3_Po1 = 'up' | PASS | - |
| 77 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel2 - SPINES_Po4 = 'up' | PASS | - |
| 78 | s1-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan4094 - MLAG_PEER = 'up' | PASS | - |
| 79 | s1-leaf4 | LANZ | VerifyLANZ | Verifies if LANZ is enabled. | - | SKIPPED | VerifyLANZ test is not supported on cEOSLab. |
| 80 | s1-leaf4 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 81 | s1-leaf4 | Services | VerifyDNSLookup | Verifies the DNS name to IP address resolution. | - | FAIL | ValueError: "AntaCommand" object has no field "failed" |
| 82 | s1-leaf4 | Software | VerifyEOSVersion | Verifies the EOS version of the device. | - | PASS | - |
| 83 | s1-leaf4 | Software | VerifyTerminAttrVersion | Verifies the TerminAttr version of the device. | - | PASS | - |
| 84 | s1-leaf4 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 85 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet1 - Remote: s1-spine2 Ethernet1 | PASS | - |
| 86 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet2 - Remote: s1-leaf1 Ethernet2 | PASS | - |
| 87 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet3 - Remote: s1-leaf2 Ethernet2 | PASS | - |
| 88 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet4 - Remote: s1-leaf3 Ethernet2 | PASS | - |
| 89 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet5 - Remote: s1-leaf4 Ethernet2 | PASS | - |
| 90 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet6 - Remote: s1-spine2 Ethernet6 | PASS | - |
| 91 | s1-spine1 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 92 | s1-spine1 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 93 | s1-spine1 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 94 | s1-spine1 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 95 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet1 - MLAG_PEER_s1-spine2_Ethernet1 = 'up' | PASS | - |
| 96 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet2 - S1-LEAF1_Ethernet2 = 'up' | PASS | - |
| 97 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet3 - S1-LEAF2_Ethernet2 = 'up' | PASS | - |
| 98 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet4 - S1-LEAF3_Ethernet2 = 'up' | PASS | - |
| 99 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet5 - S1-LEAF4_Ethernet2 = 'up' | PASS | - |
| 100 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - MLAG_PEER_s1-spine2_Ethernet6 = 'up' | PASS | - |
| 101 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Loopback0 - Router_ID = 'up' | PASS | - |
| 102 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel1 - MLAG_PEER_s1-spine2_Po1 = 'up' | PASS | - |
| 103 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel2 - RACK1_Po2 = 'up' | PASS | - |
| 104 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel4 - RACK2_Po2 = 'up' | PASS | - |
| 105 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan10 - Ten = 'up' | PASS | - |
| 106 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan20 - Twenty = 'up' | PASS | - |
| 107 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan4093 - MLAG_PEER_L3_PEERING = 'up' | PASS | - |
| 108 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan4094 - MLAG_PEER = 'up' | PASS | - |
| 109 | s1-spine1 | LANZ | VerifyLANZ | Verifies if LANZ is enabled. | - | SKIPPED | VerifyLANZ test is not supported on cEOSLab. |
| 110 | s1-spine1 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 111 | s1-spine1 | Services | VerifyDNSLookup | Verifies the DNS name to IP address resolution. | - | FAIL | ValueError: "AntaCommand" object has no field "failed" |
| 112 | s1-spine1 | Software | VerifyEOSVersion | Verifies the EOS version of the device. | - | PASS | - |
| 113 | s1-spine1 | Software | VerifyTerminAttrVersion | Verifies the TerminAttr version of the device. | - | PASS | - |
| 114 | s1-spine1 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 115 | s1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet1 - Remote: s1-spine1 Ethernet1 | PASS | - |
| 116 | s1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet2 - Remote: s1-leaf1 Ethernet3 | PASS | - |
| 117 | s1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet3 - Remote: s1-leaf2 Ethernet3 | PASS | - |
| 118 | s1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet4 - Remote: s1-leaf3 Ethernet3 | PASS | - |
| 119 | s1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet5 - Remote: s1-leaf4 Ethernet3 | PASS | - |
| 120 | s1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet6 - Remote: s1-spine1 Ethernet6 | PASS | - |
| 121 | s1-spine2 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 122 | s1-spine2 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 123 | s1-spine2 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 124 | s1-spine2 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 125 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet1 - MLAG_PEER_s1-spine1_Ethernet1 = 'up' | PASS | - |
| 126 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet2 - S1-LEAF1_Ethernet3 = 'up' | PASS | - |
| 127 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet3 - S1-LEAF2_Ethernet3 = 'up' | PASS | - |
| 128 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet4 - S1-LEAF3_Ethernet3 = 'up' | PASS | - |
| 129 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet5 - S1-LEAF4_Ethernet3 = 'up' | PASS | - |
| 130 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - MLAG_PEER_s1-spine1_Ethernet6 = 'up' | PASS | - |
| 131 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Loopback0 - Router_ID = 'up' | PASS | - |
| 132 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel1 - MLAG_PEER_s1-spine1_Po1 = 'up' | PASS | - |
| 133 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel2 - RACK1_Po2 = 'up' | PASS | - |
| 134 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel4 - RACK2_Po2 = 'up' | PASS | - |
| 135 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan10 - Ten = 'up' | PASS | - |
| 136 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan20 - Twenty = 'up' | PASS | - |
| 137 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan4093 - MLAG_PEER_L3_PEERING = 'up' | PASS | - |
| 138 | s1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan4094 - MLAG_PEER = 'up' | PASS | - |
| 139 | s1-spine2 | LANZ | VerifyLANZ | Verifies if LANZ is enabled. | - | SKIPPED | VerifyLANZ test is not supported on cEOSLab. |
| 140 | s1-spine2 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 141 | s1-spine2 | Services | VerifyDNSLookup | Verifies the DNS name to IP address resolution. | - | FAIL | ValueError: "AntaCommand" object has no field "failed" |
| 142 | s1-spine2 | Software | VerifyEOSVersion | Verifies the EOS version of the device. | - | PASS | - |
| 143 | s1-spine2 | Software | VerifyTerminAttrVersion | Verifies the TerminAttr version of the device. | - | PASS | - |
| 144 | s1-spine2 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
