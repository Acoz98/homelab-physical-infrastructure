# Parts List

This document lists the hardware, networking equipment, 3D-printed components, and supporting materials used to build the custom **10-inch 5U homelab rack**.

The goal of this project is to create a compact and modular rack capable of housing networking, compute, storage, and wireless infrastructure using a combination of repurposed hardware and custom 3D-printed mounts.

> **Note:** You do not need to use the exact same computers or networking equipment to reproduce this project. Equivalent hardware can be substituted as long as the rack mounts are designed or adapted for the dimensions of the replacement device.

---

## 1. Core Hardware

| Qty | Component                              | Purpose                                            |
| --: | -------------------------------------- | -------------------------------------------------- |
|   1 | Lenovo ThinkCentre Tiny PC             | Dedicated network/firewall platform                |
|   1 | Apple Mac mini                         | Server, NAS, and application host                  |
|   1 | Raspberry Pi 4 Model B                 | Low-power infrastructure and network-services host |
|   1 | NETGEAR GS308E 8-Port Managed Switch   | Managed Ethernet switching and VLAN connectivity   |
|   1 | Linksys Wireless Router / Access Point | Wireless network connectivity                      |
|   1 | Keystone Patch Panel                   | Front-accessible structured Ethernet connections   |

### Hardware Roles

#### Lenovo ThinkCentre

The Lenovo ThinkCentre was repurposed as a dedicated infrastructure system.

Its compact form factor, x86 architecture, replaceable components, and Ethernet connectivity made it suitable for use as a firewall/router platform.

A custom 3D-printed rack enclosure was used to adapt the non-rackmount computer to the 10-inch rack.

---

#### Apple Mac mini

The Mac mini was repurposed as the primary server and storage platform for the homelab.

Planned and current uses include:

* Network-attached storage
* Linux server workloads
* Docker containers
* Self-hosted applications
* File storage
* Backup experimentation

Because the Mac mini was not designed for rack installation, a custom 3D-printed tray was used to mount it securely.

---

#### Raspberry Pi 4 Model B

The Raspberry Pi 4 provides a low-power platform for services that benefit from remaining online continuously.

Possible roles include:

* DNS services
* Network utilities
* Remote-access services
* Monitoring
* Lightweight Linux services

Its small physical footprint makes it well suited for integration alongside the patch panel.

---

#### NETGEAR GS308E

An 8-port managed Ethernet switch provides centralized network connectivity between the different devices in the rack.

The managed switch allows the lab to later support features such as:

* VLANs
* Tagged and untagged ports
* Network segmentation
* Managed uplinks
* Multiple infrastructure networks

A custom rack mount positions the switch so that all Ethernet interfaces remain accessible from the front.

---

#### Wireless Access Point

A wireless router was repurposed as an access point and mounted at the top of the rack.

Positioning the wireless equipment at the top provides convenient access to the antennas and minimizes physical obstruction from the equipment below.

An equivalent standalone access point can also be used.

---

## 2. Structured Cabling Components

|       Qty | Component                    | Purpose                                       |
| --------: | ---------------------------- | --------------------------------------------- |
|         1 | Custom 10-inch patch panel   | Provides front-accessible network connections |
|         5 | RJ45 Keystone Jacks          | Ethernet connections for rack equipment       |
| As needed | Ethernet Patch Cables        | Connect devices to the managed switch         |
| As needed | Cat5e or Cat6 Ethernet Cable | Network connectivity                          |
| As needed | Cable Labels                 | Identifies network connections                |

The patch panel used in this build provides labeled connections for devices such as:

* ISP / WAN
* Camera network
* Client computer
* Server
* Firewall LAN

The exact labels can be changed depending on the network design.

### Why Use a Patch Panel?

Using a patch panel helps:

* Keep cabling organized
* Simplify cable tracing
* Reduce access to the rear of the rack
* Improve troubleshooting
* Provide clear connection labels
* Make future changes easier

---

## 3. 3D-Printed Rack Components

The physical rack and equipment adapters were produced using 3D printing.

### Rack Structure

The rack consists of custom printed structural components forming a compact **10-inch 5U enclosure**.

Printed components include:

* Rack frame rails
* Vertical rack supports
* Corner brackets
* Equipment mounting points
* Wall/structure mounting components

---

### Equipment Mounts

Separate mounts were printed for the equipment used in the rack.

| Component             | Printed Mount                 |
| --------------------- | ----------------------------- |
| Mac mini              | 10-inch rack tray             |
| Lenovo ThinkCentre    | 10-inch front rack enclosure  |
| NETGEAR GS308E        | Managed switch rack mount     |
| Raspberry Pi 4        | Raspberry Pi mounting bracket |
| Keystone Patch Panel  | Custom front panel            |
| Wireless Access Point | Upper rack mounting platform  |

Because consumer and small-form-factor equipment does not normally include rack ears, these adapters allow the devices to be integrated into a standardized rack layout.

---

## 4. 3D Printing Materials

### Filament

The rack was printed using:

**PETG filament**

PETG was selected because it offers a useful balance between:

* Strength
* Impact resistance
* Temperature resistance
* Layer adhesion
* Durability

PETG is generally better suited for structural components than more brittle materials when the rack will be supporting equipment for extended periods.

### Estimated Materials

The exact amount of filament required depends on:

* Infill percentage
* Number of walls/perimeters
* Layer height
* Rack depth
* Equipment mount designs
* Print failures or revisions

---

## 5. Fasteners and Mounting Hardware

Various screws and fasteners are required to assemble the rack and secure equipment.

Typical hardware includes:

* Rack assembly #M6 screws 
* Equipment mounting #M6 screws
* Washers # M6
* Nuts # M6
* Wall anchors,1000-lb 5/16-in x 1-5/8-in Sleeve Anchors with Screws 
* Screws suitable for the mounting surface


---

## 6. Tools Used

The following tools are useful when reproducing the build:

* 3D printer
* Screwdriver set
* Hex/Allen keys
* Measuring tape
* Digital calipers
* Pliers
* Ethernet cable tester
* RJ45 crimping tool, if creating custom cables
* Label maker or printable labels
* Computer for configuring network equipment


---

## 7. Rack Layout

The completed rack uses approximately the following physical arrangement:

```text
┌─────────────────────────────────────┐
│             Wireless                │
├─────────────────────────────────────┤
│       Patch Panel / Raspberry Pi    │
├─────────────────────────────────────┤
│       NETGEAR Managed Switch        │
├─────────────────────────────────────┤
│         Lenovo ThinkCentre          │
├─────────────────────────────────────┤
│             Mac mini                │
└─────────────────────────────────────┘
```

This arrangement keeps frequently accessed Ethernet connections near the front while placing the wireless equipment toward the top of the rack.

---

## 8. Equipment Substitutions

One of the goals of this project is reproducibility.

The exact hardware used here is **not required**.

For example:

| This Build           | Possible Replacement                                      |
| -------------------- | --------------------------------------------------------- |
| Lenovo ThinkCentre   | Dell OptiPlex Micro, HP EliteDesk Mini, other x86 mini PC |
| Mac mini             | Mini PC, Intel NUC, small Linux server                    |
| Raspberry Pi 4       | Raspberry Pi 5 or other small ARM/Linux computer          |
| NETGEAR GS308E       | Any similarly sized managed switch                        |
| Linksys Access Point | Standalone wireless access point                          |
| Custom Patch Panel   | Commercial 10-inch keystone patch panel                   |

When replacing equipment, verify:

1. Physical dimensions
2. Power requirements
3. Cooling requirements
4. Ethernet interface locations
5. Cable clearance
6. Rack-mount dimensions
7. Weight

A new 3D-printed adapter may be required when the dimensions of the replacement device differ.

---

## 9. Before You Start

Before printing anything, inventory all equipment that will be installed in the rack.

Search 3D-model repositories such as:

- Thingiverse
- MakerWorld
- Printables

Many common networking devices, mini PCs, switches, routers, and Raspberry Pi models already have community-created 10-inch rack mounts available.

Before downloading and printing a model:

1. Verify that it matches the exact model and hardware revision of your device.
2. Check the dimensions of the mount against your equipment.
3. Confirm that Ethernet, power, USB, and ventilation openings remain accessible.
4. Review the creator's license before modifying or redistributing the design.
5. Read comments or print notes for known fitment issues.

If a suitable mount is not available, measure the equipment using a ruler or digital caliper and create or modify a mount for your specific device.

> **Tip:** Print a small test section first when possible. A short test print can confirm screw-hole spacing, port alignment, and device fit before committing several hours and a large amount of filament to the full mount.

---

## Next Step

After gathering the required components, continue to:

**[3D Printing Guide](printing-guide.md)**

The printing guide documents the preparation and fabrication of the rack structure and individual equipment mounts.
