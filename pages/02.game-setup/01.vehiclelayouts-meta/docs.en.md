---
title: VehicleLayouts.meta
taxonomy:
    category:
        - docs
---

## VehicleLayouts.meta

### What is a _vehiclelayouts_ file?
> VehicleLayouts.meta is a file that stores information about the vehicle layout, it's entry points, seats, passenger animations. 
> <br>Below is a list of all the sections inside the file, and their short description. The list is sorted in the same way as in the file.

[ui-accordion independent=true open=none]
[ui-accordion-item title="Click to expand"]
* `AnimRateSet`
> Animation speed rate for SP and MP (?)
* `ClipSetMaps`
> ClipSets for entering and exiting a vehicle.
* `VehicleCoverBoundOffsetInfos`
> Cover bounds are set using vehicle collisions. This section allows setting cover bounds offset for the layout. 
* `BicycleInfos`
> Name tells everything, contains values for animations speeds for slow and fast gear, character leaning, helmet use, etc.
* `POVTuningInfos`
> Camera angles for Los Santos Customs (?)
* `EntryAnimVariations`
> Name tells everything, the section allows to set conditions for clipsets grouped as entry animation variations. 
* `VehicleExtraPointsInfos`
> Basically a section to set "extra" points for the vehicles based on desired bone and offset to that bone. 
* `DrivebyWeaponGroups`
> As the name tells, it defines weapon groups for drive-by (shooting inside the vehicle). By default consists of one-handed, two-handed, etc.
* `VehicleDriveByAnimInfos`
> Drive-by animations
* `VehicleDriveByInfos`
> Drive-by angles of aiming, animation references, and other values.
* `VehicleSeatInfos`
> Seat bone name, seat shuffle, rear set link, flags.
* `VehicleSeatAnimInfos`
> Animations clipsets from `ClipSetMaps`, drive-by info and other ~~useless~~ stuff.
* `VehicleEntryPointInfos`
> Which door, handle, and side to use. Also, which seat can be accessed with that EntryPoint.
* `VehicleEntryPointAnimInfos`
> EntryPoint animation clipsets from `ClipSetMaps`.
* `VehicleExplosionInfos`
> Explosion delay and position. Parts velocity and angle.
* **`VehicleLayoutInfos`** [color=red]<i class="fa fa-exclamation" aria-hidden="true"></i>[/color]
> Probably the most important section, this is where you make a summary of the entire layout; which seats, entry points, animations.
> <br>The name you use, will be the layout name in vehicles.meta
* `VehicleScenarioLayoutInfos`
> Scenario layouts, such as train driver.
* `SeatOverrideAnimInfos`
* `InVehicleOverrideInfos`
> Animation overrides, such as prostitutes.
* `FirstPersonDriveByLookAroundData`
> Name, just FOV settings for first person.
[/ui-accordion-item]
[/ui-accordion]

***
