# Validate State Report

**Table of Contents:**

- [Validate State Report](validate-state-report)
  - [Test Results Summary](#test-results-summary)
  - [Failed Test Results Summary](#failed-test-results-summary)
  - [All Test Results](#all-test-results)

## Test Results Summary

### Summary Totals

| Total Tests | Total Tests Passed | Total Tests Failed |
| ----------- | ------------------ | ------------------ |
| 92 | 92 | 0 |

### Summary Totals Devices Under Tests

| DUT | Total Tests | Tests Passed | Tests Failed | Categories Failed |
| --- | ----------- | ------------ | ------------ | ----------------- |
| s1-leaf1 |  13 | 13 | 0 | - |
| s1-leaf2 |  13 | 13 | 0 | - |
| s1-leaf3 |  13 | 13 | 0 | - |
| s1-leaf4 |  13 | 13 | 0 | - |
| s1-spine1 |  20 | 20 | 0 | - |
| s1-spine2 |  20 | 20 | 0 | - |

### Summary Totals Per Category

| Test Category | Total Tests | Tests Passed | Tests Failed |
| ------------- | ----------- | ------------ | ------------ |
| NTP |  6 | 6 | 0 |
| Interface State |  52 | 52 | 0 |
| LLDP Topology |  28 | 28 | 0 |
| MLAG |  6 | 6 | 0 |

## Failed Test Results Summary

| Test ID | Node | Test Category | Test Description | Test | Test Result | Failure Reason |
| ------- | ---- | ------------- | ---------------- | ---- | ----------- | -------------- |

## All Test Results

| Test ID | Node | Test Category | Test Description | Test | Test Result | Failure Reason |
| ------- | ---- | ------------- | ---------------- | ---- | ----------- | -------------- |
| 1 | s1-leaf1 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 2 | s1-leaf2 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 3 | s1-leaf3 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 4 | s1-leaf4 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 5 | s1-spine1 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 6 | s1-spine2 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 7 | s1-leaf1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - MLAG_PEER_s1-leaf2_Ethernet1 | PASS | - |
| 8 | s1-leaf1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet6 - MLAG_PEER_s1-leaf2_Ethernet6 | PASS | - |
| 9 | s1-leaf1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - S1-SPINE1_Ethernet2 | PASS | - |
| 10 | s1-leaf1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - S1-SPINE2_Ethernet2 | PASS | - |
| 11 | s1-leaf2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - MLAG_PEER_s1-leaf1_Ethernet1 | PASS | - |
| 12 | s1-leaf2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet6 - MLAG_PEER_s1-leaf1_Ethernet6 | PASS | - |
| 13 | s1-leaf2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - S1-SPINE1_Ethernet3 | PASS | - |
| 14 | s1-leaf2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - S1-SPINE2_Ethernet3 | PASS | - |
| 15 | s1-leaf3 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - MLAG_PEER_s1-leaf4_Ethernet1 | PASS | - |
| 16 | s1-leaf3 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet6 - MLAG_PEER_s1-leaf4_Ethernet6 | PASS | - |
| 17 | s1-leaf3 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - S1-SPINE1_Ethernet4 | PASS | - |
| 18 | s1-leaf3 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - S1-SPINE2_Ethernet4 | PASS | - |
| 19 | s1-leaf4 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - MLAG_PEER_s1-leaf3_Ethernet1 | PASS | - |
| 20 | s1-leaf4 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet6 - MLAG_PEER_s1-leaf3_Ethernet6 | PASS | - |
| 21 | s1-leaf4 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - S1-SPINE1_Ethernet5 | PASS | - |
| 22 | s1-leaf4 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - S1-SPINE2_Ethernet5 | PASS | - |
| 23 | s1-spine1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - MLAG_PEER_s1-spine2_Ethernet1 | PASS | - |
| 24 | s1-spine1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet6 - MLAG_PEER_s1-spine2_Ethernet6 | PASS | - |
| 25 | s1-spine1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - S1-LEAF1_Ethernet2 | PASS | - |
| 26 | s1-spine1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - S1-LEAF2_Ethernet2 | PASS | - |
| 27 | s1-spine1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - S1-LEAF3_Ethernet2 | PASS | - |
| 28 | s1-spine1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet5 - S1-LEAF4_Ethernet2 | PASS | - |
| 29 | s1-spine2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - MLAG_PEER_s1-spine1_Ethernet1 | PASS | - |
| 30 | s1-spine2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet6 - MLAG_PEER_s1-spine1_Ethernet6 | PASS | - |
| 31 | s1-spine2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - S1-LEAF1_Ethernet3 | PASS | - |
| 32 | s1-spine2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - S1-LEAF2_Ethernet3 | PASS | - |
| 33 | s1-spine2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - S1-LEAF3_Ethernet3 | PASS | - |
| 34 | s1-spine2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet5 - S1-LEAF4_Ethernet3 | PASS | - |
| 35 | s1-leaf1 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 - MLAG_PEER_s1-leaf2_Po1 | PASS | - |
| 36 | s1-leaf1 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel2 - SPINES_Po2 | PASS | - |
| 37 | s1-leaf2 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 - MLAG_PEER_s1-leaf1_Po1 | PASS | - |
| 38 | s1-leaf2 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel2 - SPINES_Po2 | PASS | - |
| 39 | s1-leaf3 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 - MLAG_PEER_s1-leaf4_Po1 | PASS | - |
| 40 | s1-leaf3 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel2 - SPINES_Po4 | PASS | - |
| 41 | s1-leaf4 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 - MLAG_PEER_s1-leaf3_Po1 | PASS | - |
| 42 | s1-leaf4 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel2 - SPINES_Po4 | PASS | - |
| 43 | s1-spine1 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 - MLAG_PEER_s1-spine2_Po1 | PASS | - |
| 44 | s1-spine1 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel2 - RACK1_Po2 | PASS | - |
| 45 | s1-spine1 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel4 - RACK2_Po2 | PASS | - |
| 46 | s1-spine2 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 - MLAG_PEER_s1-spine1_Po1 | PASS | - |
| 47 | s1-spine2 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel2 - RACK1_Po2 | PASS | - |
| 48 | s1-spine2 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel4 - RACK2_Po2 | PASS | - |
| 49 | s1-leaf1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 50 | s1-leaf2 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 51 | s1-leaf3 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 52 | s1-leaf4 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 53 | s1-spine1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | PASS | - |
| 54 | s1-spine1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 55 | s1-spine2 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | PASS | - |
| 56 | s1-spine2 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 57 | s1-spine1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - Router_ID | PASS | - |
| 58 | s1-spine2 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - Router_ID | PASS | - |
| 59 | s1-leaf1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: s1-leaf2_Ethernet1 | PASS | - |
| 60 | s1-leaf1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet6 - remote: s1-leaf2_Ethernet6 | PASS | - |
| 61 | s1-leaf1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: s1-spine1_Ethernet2 | PASS | - |
| 62 | s1-leaf1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: s1-spine2_Ethernet2 | PASS | - |
| 63 | s1-leaf2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: s1-leaf1_Ethernet1 | PASS | - |
| 64 | s1-leaf2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet6 - remote: s1-leaf1_Ethernet6 | PASS | - |
| 65 | s1-leaf2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: s1-spine1_Ethernet3 | PASS | - |
| 66 | s1-leaf2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: s1-spine2_Ethernet3 | PASS | - |
| 67 | s1-leaf3 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: s1-leaf4_Ethernet1 | PASS | - |
| 68 | s1-leaf3 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet6 - remote: s1-leaf4_Ethernet6 | PASS | - |
| 69 | s1-leaf3 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: s1-spine1_Ethernet4 | PASS | - |
| 70 | s1-leaf3 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: s1-spine2_Ethernet4 | PASS | - |
| 71 | s1-leaf4 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: s1-leaf3_Ethernet1 | PASS | - |
| 72 | s1-leaf4 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet6 - remote: s1-leaf3_Ethernet6 | PASS | - |
| 73 | s1-leaf4 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: s1-spine1_Ethernet5 | PASS | - |
| 74 | s1-leaf4 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: s1-spine2_Ethernet5 | PASS | - |
| 75 | s1-spine1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: s1-spine2_Ethernet1 | PASS | - |
| 76 | s1-spine1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet6 - remote: s1-spine2_Ethernet6 | PASS | - |
| 77 | s1-spine1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: s1-leaf1_Ethernet2 | PASS | - |
| 78 | s1-spine1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: s1-leaf2_Ethernet2 | PASS | - |
| 79 | s1-spine1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet4 - remote: s1-leaf3_Ethernet2 | PASS | - |
| 80 | s1-spine1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet5 - remote: s1-leaf4_Ethernet2 | PASS | - |
| 81 | s1-spine2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: s1-spine1_Ethernet1 | PASS | - |
| 82 | s1-spine2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet6 - remote: s1-spine1_Ethernet6 | PASS | - |
| 83 | s1-spine2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: s1-leaf1_Ethernet3 | PASS | - |
| 84 | s1-spine2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: s1-leaf2_Ethernet3 | PASS | - |
| 85 | s1-spine2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet4 - remote: s1-leaf3_Ethernet3 | PASS | - |
| 86 | s1-spine2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet5 - remote: s1-leaf4_Ethernet3 | PASS | - |
| 87 | s1-leaf1 | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 88 | s1-leaf2 | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 89 | s1-leaf3 | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 90 | s1-leaf4 | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 91 | s1-spine1 | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 92 | s1-spine2 | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
