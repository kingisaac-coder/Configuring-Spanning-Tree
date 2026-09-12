# Configuring-Spanning-Tree
Cisco Packet Tracer lab focused on configuring and verifying Spanning Tree Protocol (STP) to prevent Layer 2 switching loops and control root bridge selection.


# Configuring Spanning Tree Protocol (STP)

## 📖 Overview

This lab focused on configuring and verifying Spanning Tree Protocol (STP) on Cisco switches.

The lab provided hands-on experience with Layer 2 loop prevention, root bridge elections, port roles, and STP behavior in a switched network containing redundant paths.

## 🎯 Objectives

The lab was designed to:

* Understand the purpose of Spanning Tree Protocol.
* Configure and verify STP on Cisco switches.
* Identify the root bridge.
* Examine STP port roles and states.
* Influence root bridge selection.
* Observe how STP prevents Layer 2 switching loops.
* Verify the resulting spanning-tree topology.
* Troubleshoot STP-related configuration issues.

## 🧠 Concepts Practiced

* Spanning Tree Protocol (STP)
* Root bridge
* Bridge ID
* Root port
* Designated port
* Alternate/blocking port
* STP convergence
* Redundant Layer 2 links
* Broadcast storms
* Layer 2 loop prevention
* Switch priority

## 🛠️ Tools Used

* Cisco Packet Tracer
* Cisco IOS CLI

## ⚙️ Configuration

The switches were configured and connected using redundant Layer 2 links.

STP was then examined to determine which switch was elected as the root bridge and which ports were forwarding or blocking.

Switch priority was configured where necessary to influence which switch became the root bridge.

## 🧪 Verification & Testing

The spanning-tree topology was verified using commands such as:

```text
show spanning-tree
show spanning-tree vlan 1
show running-config
```

These commands were used to identify:

* The root bridge
* Root ports
* Designated ports
* Blocking/alternate ports
* STP priority
* Port states

Connectivity was also tested to ensure that the network remained operational while STP prevented redundant paths from creating Layer 2 loops.

## 🔍 Troubleshooting

Potential STP issues investigated during the lab included:

* An unexpected switch becoming the root bridge.
* Incorrect STP priority.
* Unexpected port roles or states.
* Interfaces being down.
* Incorrect switch connectivity.
* Redundant links causing unexpected topology changes.

Troubleshooting involved examining the spanning-tree output and comparing bridge IDs, priorities, and port roles to determine why STP selected a particular topology.

## 🔐 Why STP Matters

Redundant links are commonly used in switched networks to provide resilience. However, Ethernet networks can experience serious problems when multiple active Layer 2 paths create a loop.

STP prevents these loops by logically blocking redundant paths while maintaining them as backup paths.

If the active path fails, STP can allow an alternative path to become available, improving network resilience while preventing Layer 2 loops.

## ✅ Outcome

Successfully configured and verified Spanning Tree Protocol, identified the root bridge and STP port roles, and demonstrated how STP prevents Layer 2 switching loops in a redundant network topology.

## 📚 Skills Demonstrated

* Cisco IOS CLI
* Spanning Tree Protocol
* Root bridge selection
* STP priority configuration
* Port-role identification
* Layer 2 troubleshooting
* Network redundancy
* Loop prevention
* STP verification
