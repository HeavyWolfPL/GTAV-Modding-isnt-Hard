---
title: VehicleLayoutsInfo
taxonomy:
    category:
        - docs
---

[ui-accordion independent=true open=none]
[ui-accordion-item title="Layout Example"]
```
<Item type="CVehicleLayoutInfo">
  <Name>LAYOUT_CUSTOM</Name>
  <Seats>
	<Item>
	  <SeatInfo ref="SEAT_CUSTOM_FRONT_LEFT" />
	  <SeatAnimInfo ref="SEAT_ANIM_VAN_FRONT_LEFT" />
	</Item>
	<Item>
	  <SeatInfo ref="SEAT_CUSTOM_FRONT_RIGHT" />
	  <SeatAnimInfo ref="SEAT_ANIM_VAN_FRONT_RIGHT" />
	</Item>
		<Item>
	  <SeatInfo ref="SEAT_CUSTOM_LEFT" />
	  <SeatAnimInfo ref="SEAT_ANIM_CUSTOM_LEFT" />
	</Item>
	<Item>
	  <SeatInfo ref="SEAT_CUSTOM_RIGHT" />
	  <SeatAnimInfo ref="SEAT_ANIM_CUSTOM_RIGHT" />
	</Item>
  </Seats>
  <EntryPoints>
	<Item>
	  <EntryPointInfo ref="ENTRY_POINT_CUSTOM_FRONT_LEFT" />
	  <EntryPointAnimInfo ref="ENTRY_POINT_ANIM_VAN_FRONT_LEFT" />
	</Item>
	<Item>
	  <EntryPointInfo ref="ENTRY_POINT_CUSTOM_FRONT_RIGHT" />
	  <EntryPointAnimInfo ref="ENTRY_POINT_ANIM_VAN_FRONT_RIGHT" />
	</Item>
		<Item>
	  <EntryPointInfo ref="ENTRY_POINT_CUSTOM_LEFT" />
	  <EntryPointAnimInfo ref="ENTRY_POINT_ANIM_VAN_REAR_LEFT" />
	</Item>
	<Item>
	  <EntryPointInfo ref="ENTRY_POINT_CUSTOM_RIGHT" />
	  <EntryPointAnimInfo ref="ENTRY_POINT_ANIM_VAN_REAR_RIGHT" />
	</Item>
  </EntryPoints>
  <LayoutFlags>StreamAnims UseVanOpenDoorBlendParams UseDoorOscillation UseLeanSteerAnims UseLowerDoorBlockTest</LayoutFlags>
  <BicycleInfo ref="NULL" />
  <HandsUpClipSetId>busted_vehicle_van</HandsUpClipSetId>
  <SteeringWheelOffset x="0.006700" y="0.330000" z="0.270000" />
  <MaxXAcceleration value="3.00000" />
  <FirstPersonAdditiveIdleClipSets>
	<Item>clipset@veh@van@ds@idle_a</Item>
	<Item>clipset@veh@van@ds@idle_b</Item>
	<Item>clipset@veh@van@ds@idle_c</Item>
	<Item>clipset@veh@van@ds@idle_d</Item>
	<Item>clipset@veh@van@ds@idle_e</Item>
  </FirstPersonAdditiveIdleClipSets>
  <FirstPersonRoadRageClipSets>
	<Item>clipset@veh@van@ds@hit_wheel@idle_a</Item>
	<Item>clipset@veh@van@ds@hit_wheel@idle_b</Item>
	<Item>clipset@veh@van@ds@hit_wheel@idle_c</Item>
  </FirstPersonRoadRageClipSets>
</Item>
```
[/ui-accordion-item]
[/ui-accordion]