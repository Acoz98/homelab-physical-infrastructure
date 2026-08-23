# Rack Assembly Guide

This guide documents the physical assembly of the custom **10-inch 5U homelab rack** after all required components have been printed.

The rack was built to organize several pieces of networking and server equipment that were not originally designed for traditional rack installation.

The completed rack integrates:

* Mac mini server
* Lenovo ThinkCentre Tiny
* NETGEAR GS308E managed switch
* Raspberry Pi 4
* Keystone patch panel
* Wireless access point
* French cleat wall-mounting system

> **Note:** Your equipment and rack layout may differ. Use this guide as a general assembly reference and adapt the installation order to your own hardware.

---

# 1. Before Assembly

Before assembling the rack, verify that all printed components are complete and free of major defects.

Inspect each part for:

* Cracks
* Layer separation
* Warping
* Damaged mounting holes
* Poor fitment
* Sharp edges
* Obstructed screw holes

Perform a test fit of equipment mounts before permanently installing the rack.

It is much easier to correct a fitment problem before the rack is mounted and fully populated.

---

# 2. Gather the Printed Components

For this build, the printed components included:

* 10-inch 5U rack frame
* Rack side supports
* French cleat rack mounts
* Mac mini rack mount
* Lenovo ThinkCentre rack mount
* NETGEAR GS308E rack mount
* Raspberry Pi + five-keystone panel
* 1U slotted shelf
* Additional mounting components

The original models used for this project are documented in:

**[3D Printing Guide](printing-guide.md)**

---

# 3. Assemble the 5U Rack Frame

Start with the main Lab Rax structural components.

Lay the pieces on a flat surface before attaching them.

The basic structure should form a rigid rectangular frame with mounting positions on both sides.

A simplified representation is:

```text
Front View

┌──────────────────────────────┐
│                              │
│             5U               │
│                              │
│                              │
│                              │
└──────────────────────────────┘

       10-inch rack width
```

During assembly:

1. Align the rack rails and structural supports.
2. Install the required fasteners loosely at first.
3. Confirm that the frame sits square.
4. Tighten the fasteners gradually.
5. Verify that both sides remain parallel.
6. Test a rack-mounted component before continuing.

Avoid fully tightening one side before the remaining frame pieces are aligned.

This helps prevent the frame from becoming twisted or uneven.

---

# 4. Install the French Cleat Mount

This build uses a **French cleat system** so the rack can be mounted to the wall while remaining removable for maintenance.

The system consists of two parts:

```text
          ________________|
         /                |
        / Rack-Side Cleat |
       /                  |
Wall
 │
 │    Wall-Side Cleat
 │   ╱
 │  ╱
 │ ╱
 │╱

```

One part of the cleat is secured to the wall.

The corresponding rack-side component attaches to the rear of the rack.

When the rack is lowered onto the wall cleat, the two angled surfaces lock together.

### Important

The wall mounting hardware must be appropriate for:

* Wall material
* Rack weight
* Equipment weight
* Cable load
* Total expected load

Whenever possible, secure the wall-side cleat to a wall stud or another suitable structural surface.

Do not rely on lightweight mounting hardware for a fully populated rack.

---

# 5. Plan the Equipment Layout

Before installing equipment, determine where each device will sit.

The layout used in this build was organized approximately as follows:

```text
┌────────────────────────────────────┐
│       Wireless / Upper Shelf       │
├────────────────────────────────────┤
│    Raspberry Pi + Patch Panel      │
├────────────────────────────────────┤
│      NETGEAR Managed Switch        │
├────────────────────────────────────┤
│       Lenovo ThinkCentre Tiny      │
├────────────────────────────────────┤
│            Mac mini                │
└────────────────────────────────────┘
```

The exact position of equipment can be changed depending on your hardware.

When planning the rack layout, consider:

* Equipment weight
* Cooling
* Ethernet cable access
* Power cable access
* USB access
* Wireless antennas
* Future expansion
* Ease of maintenance

Heavier equipment should generally be positioned lower when possible.

---

# 6. Install the Mac mini Mount

The Mac mini occupies one of the lower rack positions.

Because the Mac mini is not traditional rackmount equipment, a dedicated 10-inch rack adapter was used.

Before installation:

1. Test fit the Mac mini inside the printed mount.
2. Verify that the computer slides in without excessive force.
3. Confirm access to the power connection.
4. Confirm access to Ethernet and other required ports.
5. Check that ventilation is not blocked.

Install the rack mount into the frame and verify that it remains level.

Once secured, place the Mac mini into the mount.

Do not connect all cables yet.

Leaving the rack uncabled makes the remaining equipment easier to install.

---

# 7. Install the Lenovo ThinkCentre

The Lenovo ThinkCentre Tiny is installed using a device-specific 10-inch rack mount.

Before installation, confirm that the printed mount matches the exact ThinkCentre model being used.

Check access to:

* Ethernet interfaces
* Power
* USB
* Display connections
* Ventilation

Install the mount into the rack and carefully insert the ThinkCentre.

Verify that the computer is secure and does not shift when light pressure is applied.

---

# 8. Install the Managed Switch

The **NETGEAR GS308E** is installed using a  10-inch rack mount.

The switch is positioned so that the Ethernet interfaces face toward the front of the rack.

This provides several advantages:

* Easier patch cable installation
* Faster troubleshooting
* Easier port identification
* Improved cable management
* No need to reach behind the rack for normal network changes

After inserting the switch, verify that it sits securely inside the printed mount.

Do not connect the Ethernet cables yet.

---

# 9. Install the Raspberry Pi and Keystone Panel

The Raspberry Pi rack mount also includes space for **five keystone jacks**.

This allows one rack unit to perform two functions:

```text
┌───────────────────────────────────┐
│ Pi 4 │ K1 │ K2 │ K3 │ K4 │ K5  │
└───────────────────────────────────┘
```

Install the Raspberry Pi into its mounting location.

Then install the required keystone jacks into the front panel.

The keystone connections can be used for devices such as:

* WAN / ISP
* Firewall LAN
* Server
* Client computer
* Camera network
* Other rack equipment

The labels should reflect your own network design.

---

# 10. Label the Patch Panel

Every connection should be labeled before the final cabling is completed.

Example labels might include:

```text
WAN
LAN
SERVER
CLIENT
CAMERA
```

Avoid relying only on cable color to identify connections.

Proper labels make it easier to:

* Trace cables
* Troubleshoot connectivity
* Replace equipment
* Change switch ports
* Document the network
* Understand the rack months later


---

# 11. Install the Upper Shelf and Wireless Equipment

A slotted 1U shelf can be installed near the top of the rack for equipment that does not require a dedicated rack mount.

In this build, the upper area is used for wireless equipment.

Positioning the wireless device toward the top helps:

* Keep antennas unobstructed
* Maintain easy access
* Separate the wireless device from heavier equipment
* Allow convenient Ethernet and power connections

The shelf slots also provide additional airflow around the device.

Verify that the wireless equipment cannot easily slide or fall from the shelf.

---

# 12. Check Airflow

Before adding cables, inspect the rack for blocked ventilation.

Pay particular attention to:

* Lenovo ThinkCentre vents
* Mac mini airflow
* Managed switch ventilation
* Raspberry Pi cooling
* Wireless equipment

Avoid positioning cables directly against cooling openings.

A compact rack saves space, but the smaller physical area also makes airflow planning more important.

---

# 13. Connect Ethernet Cabling

Once all hardware is securely installed, begin connecting Ethernet cables.

A useful approach is:

```text
Device
   │
   ↓
Front Keystone
   │
   ↓
Patch Cable
   │
   ↓
Managed Switch
```

Use cables that are long enough to reach comfortably but not significantly longer than necessary.

Excess cable inside a compact rack can:

* Block airflow
* Make troubleshooting harder
* Put unnecessary pressure on connectors
* Make the rack appear disorganized

---

# 14. Connect Power

After network cabling is organized, connect power to each device.

Typical powered equipment includes:

* Mac mini
* Lenovo ThinkCentre
* Managed switch
* Raspberry Pi
* Wireless access point

Route power cables separately from network cables where practical.

Leave enough cable slack so that equipment can be removed for maintenance without immediately placing strain on the connector.

---

# 15. Final Physical Inspection

Before powering on the entire rack, perform a final inspection.

Verify:

* [ ] Rack frame is secure
* [ ] French cleat is properly seated
* [ ] Rack remains level
* [ ] Mac mini is secure
* [ ] Lenovo ThinkCentre is secure
* [ ] Managed switch is secure
* [ ] Raspberry Pi is secure
* [ ] Keystone jacks are fully seated
* [ ] Wireless equipment is stable
* [ ] Ethernet cables are labeled
* [ ] Power cables are secure
* [ ] Ventilation openings are clear
* [ ] Cables are not under excessive tension
* [ ] No loose screws or hardware remain inside the rack

---

# 16. Completed Physical Infrastructure

At this point, the physical infrastructure is assembled.

The rack now provides a centralized location for:

```text
                    HOMELAB RACK
                         │
          ┌──────────────┼──────────────┐
          │              │              │
      COMPUTE         NETWORKING      SERVICES
          │              │              │
     Mac mini         Managed          Pi 4
     ThinkCentre       Switch
                         │
                    Patch Panel
                         │
                      Wireless
```

The physical infrastructure provides the foundation for the network and server projects that follow.

---

# Why This Layout Was Chosen

The goal was not simply to make the equipment fit inside a rack.

The layout was designed around:

* Accessibility
* Modularity
* Cable management
* Serviceability
* Cooling
* Equipment reuse
* Future upgrades

Using 3D-printed mounts made it possible to integrate consumer and small-form-factor equipment into a standardized rack layout without purchasing traditional enterprise rackmount servers.

---

# If You Are Building Your Own

You do not need to reproduce this rack exactly.

The most important part of the process is designing around the hardware you actually have.

A good workflow is:

```text
Inventory Equipment
        ↓
Measure Hardware
        ↓
Select Rack Size
        ↓
Find Compatible Mounts
        ↓
Print Components
        ↓
Test Fit
        ↓
Plan Rack Layout
        ↓
Assemble Frame
        ↓
Install Hardware
        ↓
Label Connections
        ↓
Cable Equipment
        ↓
Inspect
        ↓
Begin Network Configuration
```

This makes the project adaptable to other mini PCs, switches, Raspberry Pi models, access points, and server hardware.

---

# Related Documentation

* [Parts List](parts-list.md)
* [3D Printing Guide](printing-guide.md)

---

# Project Status

**Physical rack assembly:** Complete

The rack is now ready for the networking and server configuration stages of the homelab.
