# NavGrid

NavGrid is an all-in-one navigation system for Starbase.

NavGrid builds upon Collective's ISAN2 GPS system, adding a familiar visual
interface to supplement ISAN's raw-numbers display.

[NavGrid UI picture]

It features 6 directional presets, up to 14 editable user-defined waypoints,
and a wide variety of optional displays to help point you whichever direction
you might be going.

[Navgrid + NavP + ISAN Picture]

NavGrid is designed with the following audiences in mind:
- Pilots who want to just choose a destination and fly to it, without needing
to stare at numbers, without fiddling with transponder settings, and without
puzzling over which way is "up".
- Streamers who want to navigate without displaying their numbers on the
screen.
- Clans who want member to be able to easily navigate multiple company stations.
- Ship designers who want to provide more navigational quality-of-life without
losing compatibility with Starbase's most prevalent GPS system.

[Navgrid in action; pointing at Origin 14]

## Requirements and Features

Performance: *0.8s* refresh time with max *3.0s* processing latency

**Core:**
[Picture 3 nav recievers, 4 racks, and the required controls]
- Triplicate ISAN synchronization: 3 individual ISAN units operate on separate
synchronized chips to provide maximum accuracy with zero performance loss.
- Full support for any other ISAN addons you might be using, as long as they
let you run with ISAN `speed` enabled.
- Nav "Ball" display: visual ASCII display for easy directional navigation.
- 6 Directional presets for general navigation (2 for each x, y, z axis)
- 10 user-defined waypoints

**(Optional) ISAN QUAD:**
[Picture 9 more nav recievers]
+ QUAD damage detection: QUAD mode has the same automatic damage detection as
standard ISAN, with all three units entering MONO in unison if receivers are
damaged or destroyed.
+ Significantly reduced jitter while turning.

**(Optional) Expansion modules:**
[Picture 1 memory card and 1 chip]
+ 4 more user-defined waypoints
+ Display navpoint coordinates and ship attitude

**(Optional) Use your own waypoint system:**
[Picture 1 rack]
+ Replace NavGrid's navpoint management with your favorite waypoint system, as
long as it uses ISAN coordinates.

## Installation

Installation is similar to ISAN2, but with more units. Please refer to the [ISAN
manual](isan.to/doc) for a really good explanation of how to install, name, and
operate each unit.

#### Chips and memory:
[Picture mapping chip types to file names]
[Picture of memory contents]

#### Receivers:
It is very important that receivers are installed in the correct "L" shape. If
your axes are misaligned, your navigation will be misaligned.

[Picture showing reciever axes]

By default, NavGrid assumes your recievers will be "forward" and "down" from
your primary ISAN receiver(s). You can use "rear" and "up" receivers instead
with a small code edit:

[Picture showing axis options]

For quad setups, name location is also very important. Make sure corresponding
receivers for each ISAN direction are in-axis with each other as shown here:

[Picture showing QUAD naming]

#### Controls and operation:
TODO