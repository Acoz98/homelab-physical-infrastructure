# 3D Printing Guide

This guide documents the 3D-printed components used to build my custom **10-inch 5U homelab rack**.

Rather than designing every component from scratch, I researched existing community-created models that matched the hardware I already owned.

This approach reduced development time while still requiring:

* Hardware compatibility research
* Physical measurements
* Model selection
* Print planning
* Material selection
* Fitment testing
* Assembly
* Troubleshooting

All original models remain the work of their respective creators. This repository documents how I used those designs to build my homelab and links directly back to the original model pages.

---

# Source Models

## 1. Lab Rax 10-Inch 5U Server Rack

**Model:** Lab Rax 10" Server Rack — 5U
**Platform:** MakerWorld
**Model ID:** `1294480`
**Used for:** Main 10-inch 5U rack structure

**Original Model:**
[MakerWorld — Lab Rax 10" Server Rack 5U](https://makerworld.com/en/models/1294480-lab-rax-10-server-rack-5u?from=search#profileId-1325352)

This is the primary structure used for the homelab.

The model provides the structural components required to build the compact 10-inch rack, including the vertical and horizontal frame components.

This model established the physical foundation for the rest of the project.

---

## 2. Lab Rax French Cleat Mount

**Model:** Lab Rax 10" Server Rack — French Cleat Mount 20mm
**Platform:** MakerWorld
**Model ID:** `2182884`
**Used for:** Mounting the completed rack to the wall

**Original Model:**
[MakerWorld — Lab Rax French Cleat Mount 20mm](https://makerworld.com/en/models/2182884-lab-rax-10-server-rack-french-cleat-mount-20mm?from=search#profileId-2369420)

This model provides the interface between the Lab Rax structure and the French cleat wall-mounting system.

The French cleat allows the rack to be securely mounted while still making it possible to remove the rack for maintenance, upgrades, or changes.

---

## 3. 3-Inch French Cleat

**Model:** 3in French Cleat
**Platform:** Printables
**Model ID:** `163275`
**Used for:** Wall-side French cleat mounting system

**Original Model:**
[Printables — 3in French Cleat](https://www.printables.com/model/163275-3in-french-cleat)

This component was used as part of the wall-mounting solution.

A French cleat provides a simple way to securely support the rack while keeping the rack removable if access is required later.

---

## 4. Raspberry Pi + Keystone Rack Mount

**Model:** 10-Inch Rack Mount for 1 Raspberry Pi + 5x Keystone
**Platform:** MakerWorld
**Model ID:** `2019551`
**Used for:** Raspberry Pi installation and front-facing Ethernet connections

**Original Model:**
[MakerWorld — Raspberry Pi + 5x Keystone Rack Mount](https://makerworld.com/en/models/2019551-10-inch-rack-mount-for-1-raspberry-pi-5x-keystone?from=search#profileId-2176282)

This 1U panel combines two useful functions:

* Raspberry Pi mounting
* Five keystone openings

The Raspberry Pi can therefore be integrated directly into the rack while the keystone ports provide structured front-facing Ethernet connections.

This was useful because the Raspberry Pi and patch-panel functionality could share the same rack unit.

---

## 5. Mac mini 10-Inch Rack Mount

**Model:** Mac mini 10-Inch Rackmount
**Platform:** MakerWorld
**Model ID:** `2792527`
**Used for:** Mounting the Mac mini server

**Original Model:**
[MakerWorld — Mac mini 10-Inch Rackmount](https://makerworld.com/en/models/2792527-mac-mini-10-inch-rackmount?from=search#profileId-3105346)

The Mac mini was not originally designed for rack installation.

This mount allows the Mac mini to be integrated into the 10-inch rack while maintaining access to the computer and its connections.

Before printing, verify that the model is compatible with the specific Mac mini generation being used.

---

## 6. Lenovo ThinkCentre Tiny Rack Mount

**Model:** Lenovo ThinkCentre Tiny 10" Rack Mount — M720q
**Platform:** MakerWorld
**Model ID:** `1945283`
**Used for:** Mounting the Lenovo ThinkCentre Tiny

**Original Model:**
[MakerWorld — Lenovo ThinkCentre Tiny M720q Rack Mount](https://makerworld.com/en/models/1945283-lenovo-thinkcentre-tiny-10-rack-mount-m720q?from=search#profileId-2280061)

The Lenovo ThinkCentre Tiny was repurposed as infrastructure hardware for the homelab.

Because the ThinkCentre is a small-form-factor computer rather than traditional rackmount equipment, this adapter allows it to occupy a standard position inside the 10-inch rack.

Before printing, verify the exact ThinkCentre model because dimensions and port locations can differ between generations.

---

## 7. NETGEAR GS308E Rack Mount

**Model:** NETGEAR GS308E Screwless 10-Inch Rack Mount
**Platform:** MakerWorld
**Model ID:** `1859737`
**Used for:** Mounting the managed Ethernet switch

**Original Model:**
[MakerWorld — NETGEAR GS308E Screwless Rack Mount](https://makerworld.com/en/models/1859737-netgear-gs308e-screwless-10-inch-rack-mount?from=search#profileId-1988907)

This mount was designed specifically for the NETGEAR GS308E managed switch.

The switch fits into the rack mount while keeping all Ethernet interfaces accessible from the front of the rack.

Front-facing Ethernet connections make network changes, cable tracing, and troubleshooting significantly easier.

---

## 8. Lab Rax 1U Shelf with Slots

**Model:** Lab Rax 1U Shelf with Slots
**Platform:** MakerWorld
**Model ID:** `1357259`
**Used for:** General-purpose equipment support

**Original Model:**
[MakerWorld — Lab Rax 1U Shelf with Slots](https://makerworld.com/en/models/1357259-lab-rax-1u-shelf-with-slots?from=search#profileId-1401156)

This shelf provides a general-purpose 1U mounting surface for devices that do not have a dedicated rack adapter.

The slots also provide additional ventilation around equipment placed on the shelf.

This makes the rack more flexible because future equipment can be installed without necessarily requiring a device-specific mount.

---

# Model Selection Process

Before printing a component, I verified that the model was appropriate for the equipment I planned to install.

For each device, I checked:

1. Exact hardware model
2. Device dimensions
3. Mount dimensions
4. Ethernet-port accessibility
5. Power-connector accessibility
6. USB-port accessibility
7. Cooling and ventilation
8. Rack compatibility
9. Required fasteners
10. Print orientation and support requirements

When possible, I also reviewed photographs, comments, print profiles, and community builds before committing to a long print.

---

# Recommended Workflow

If you are building a similar rack, I recommend following this process before printing any equipment mount:

```text
Inventory Hardware
        ↓
Identify Exact Model Number
        ↓
Search Printables / MakerWorld / Thingiverse
        ↓
Find Compatible Rack Mount
        ↓
Check Measurements
        ↓
Check Ports and Ventilation
        ↓
Review License
        ↓
Review Community Feedback
        ↓
Print
        ↓
Test Fit
        ↓
Install
```

Do not assume that a mount will fit simply because the device name is similar.

Different hardware revisions can have changes in:

* Dimensions
* Ventilation
* Port locations
* Power connectors
* Screw locations

Always verify your exact equipment model before printing.

---

# Important Licensing Note

The models listed in this guide were created by members of the 3D-printing community.

The original creators retain ownership of their designs.

Before downloading, modifying, redistributing, or commercially using any model, review the license displayed on the original model page.

This GitHub repository links directly to the original model pages rather than redistributing the original STL or 3MF files.

This helps:

* Credit the original designers
* Respect the model licenses
* Direct users to the latest version of each design
* Allow users to review updated print profiles and instructions
* Keep this repository focused on documenting the homelab build

---

# Why I Am Linking the Original Files

The purpose of documenting the source models is to make this build reproducible while properly crediting the designers who made the physical build possible.

Anyone attempting to reproduce this project can:

1. Review the equipment list.
2. Follow the original model links.
3. Verify compatibility with their hardware.
4. Review the model's license.
5. Download the files directly from the original creator.
6. Select an appropriate print profile.
7. Follow the printing and assembly process documented in this repository.

This approach allows someone to recreate the physical infrastructure without requiring the exact same hardware or relying on files copied into this repository.

---
