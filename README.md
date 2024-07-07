# Ellis SuperSlicer Profiles for PrusaSlicer

This is a close adaption of [Ellis SuperSlicer Profiles](https://github.com/AndrewEllis93/Ellis-SuperSlicer-Profiles) for PrusaSlicer.
Please read through the upstream README thoroughly for important **WARNINGS**, pitfalls, headaches and useful tips & tricks.

Same as the original SuperSlicer profiles these can work well on any printer, provided you adjust the speeds, accelerations, machine limits/dimensions, and volumetric flow limits accordingly. They have been verified and are in use on a Voron V0, Trident and V2.

Please check the changelog at the end of this document for the latest changes.

## Important Notes

* **⚠** Tested PrusaSlicer version: **2.8.0** (2024-06-27)
* **⚠** Use these at your own risk. Make backups of your existing profiles before using these.
* **⚠** All the warnings and notes from the [upstream profile](https://github.com/AndrewEllis93/Ellis-SuperSlicer-Profiles/blob/master/README.md) apply
* **⚠** Use different PrusaSlicer versions at your peril.

## Important Differences / Changes

* Extrusion widths are absolute values for a 0.4mm nozzle.
* Auto emitting temperature commands has been disabled - no more workarounds in the start G-Code.
* Not connected infill styles have been approximated using "Monotonic Lines" infill

## What's missing (key features)

* 45° profiles - [PR #10651](https://github.com/prusa3d/PrusaSlicer/pull/10651)
* Matching „Solid Infill Pattern“ - [PR #10652](https://github.com/prusa3d/PrusaSlicer/pull/10652)
* Reduced (50%) bridge density - [PR #10650](https://github.com/prusa3d/PrusaSlicer/pull/10650)
* Many advanced (micro) adjustments from SuperSlicer  
  In my experience most of these are not required to get an equal print quality from PrusaSlicer. Many of the speed/cooling-related ones can be replaced with newer features like "Dynamic Fan Speeds" and "Dynamic Overhang Speeds".

## Miscellaneous

The Voron bed models linked from the upstream readme work in PrusaSlicer as well, spruce up your previews with them.

## Changelog

* 2024-07-06:
  * Updated profiles for PrusaSlicer 2.8.0
    * Enabled `chamber_temperature` and `chamber_minimal_temperature` settings
    * Enabled single perimeter on all top surfaces
* 2023-07-27:
  * Initial release based on the upstream version from 2022-11-09 (flip-flopping edition!).
