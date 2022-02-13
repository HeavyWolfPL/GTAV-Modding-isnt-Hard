---
title: VehicleSeatInfos
date: '01/27/2022 17:39'
---

#### VehicleSeatInfos
This is the section where you define all seats that will be used within the layout. Please note that you can already use seats defined within the layout by default (such as front seats for example).

[ui-accordion independent=true open=none]
[ui-accordion-item title="Front Seat Example"]
```
	<Item type="CVehicleSeatInfo">
      <Name>SEAT_CUSTOM_FRONT_LEFT</Name>
      <SeatBoneName>seat_dside_f</SeatBoneName>
      <ShuffleLink>SEAT_CUSTOM_FRONT_RIGHT</ShuffleLink>
      <RearSeatLink>SEAT_CUSTOM_REAR_LEFT</RearSeatLink>
      <DefaultCarTask>TASK_DRIVE_WANDER</DefaultCarTask>
      <SeatFlags>IsFrontSeat</SeatFlags>
      <HairScale value="0.000000" />
    </Item>
```
[/ui-accordion-item]
[/ui-accordion]

[ui-accordion independent=true open=none]
[ui-accordion-item title="Rear Seat Example"]
```
    <Item type="CVehicleSeatInfo">
      <Name>SEAT_CUSTOM_REAR_LEFT</Name>
      <SeatBoneName>seat_dside_r</SeatBoneName>
      <ShuffleLink>SEAT_CUSTOM_REAR_RIGHT</ShuffleLink>
      <RearSeatLink />
      <DefaultCarTask>TASK_DRIVE_WANDER</DefaultCarTask>
      <SeatFlags>IsIdleSeat</SeatFlags>
      <HairScale value="0.000000" />
    </Item>
```
[/ui-accordion-item]
[/ui-accordion]

* `Name`
> Does it really need to be explained here? 
* `SeatBoneName`
> Seat dummy's name you define in the model itself. Usually `seat_(d/p)side_(f/r)`
* `ShuffleLink`
> This is the seat peds will shuffle to if needed/ordered. Recommended to set a seat that's in the same line, don't set it to a seat behind you.
* `RearSeatLink`
> Like the name says, seat that is behind the current seat. Leave as `<RearSeatLink />` if there isn't one.
* `DefaultCarTask`
> Unknown yet.
* `SeatFlags`
> Available flags: `IsFrontSeat`, `IsIdleSeat`, `NoIndirectExit`, `KeepOnHeadProp`, `DontDetachOnWorldCollision`.
* `HairScale`
> Unknown yet. Most likely setting it to higher value than 0.00 scales the hair down.