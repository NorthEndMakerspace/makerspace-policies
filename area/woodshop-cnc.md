---
layout: area-policy
order: 2
title: Woodshop - CNC
discord_channel_name: "#woodworking"
discord_channel_url: https://discord.com/channels/775417143029661748/775418072428970076
stewards: "@steward (cnc)"
---

The CNC requires certification to use. The async learning module ([CNC 101 - Learn @ NEM](https://learn.northendmakers.org/course/view.php?id=3)) must be completed before certification.

The basic woodshop certification is also required and all [woodshop policies]({% link area/woodshop.md %}) apply while using the CNC.

## Before cutting

1. Press the “Stop” button on the spindle paddle switch, even if it appears off.
1. Check that there is nothing on the CNC or gantry rails that could interfere with the motion of the CNC gantry or spindle (e.g. snagged wires, material in the way, etc).
1. **Badge in and briefly test the spindle works before setting up to check your certification is valid.**
1. Press the "Start" button on the CNC paddle switch.
1. Log in to the laptop and launch [gSender](https://resources.sienci.com/view/gs-using-gsender/).
1. Home the machine.
   * If the gantry or spindle was moved while the machine was off, you must re-home the machine.
   * If you crash the spindle, you must re-home the machine (you can re-home just Z if crashed only in Z).
1. Place your stock on the spoil board and clamp it down. It should not move if you try to push or pull it with your body weight.
1. Ensure the correct bit for your cut is inserted and secure.
   * With the Musclechuck, this means tightening the bolt with the allen key until it is just barely snug, then tighten another quarter turn. Note that overtightening risks damage to the chuck.
1. Zero the machine relative to your stock based on the origin you specified during tool path generation. Be mindful of whether your Z origin is at the top or bottom of your stock.
1. Use the “outline” feature of gSender to ensure the cutter and router will not collide with any clamps (or manually jog the machine around).
   * It’s worth raising the endmill above any clamps or fixtures initially to avoid accidentally crashing if adjustments are needed.
   * Be aware the “outline” feature attempts to calculate a concave hull, but this sometimes yields an outline that exceeds the actual toolpath.
1. Jog the machine above your stock and within the tool path outline. (This just helps avoid crashing when starting the job)
1. Check the router RPM setting matches what is expected in your design.
   * 1-6 is 8000-24000 RPM, with 3.5 being around 16000RPM
1. Attach the dust boot and turn on the dust collector.
1. Turn on the spindle.
1. Start your job.

## While cutting

1. Keep hands and feet clear of the machine, especially the cutting area, gantry, and rails.
1. Do not lean on or over the machine bed or gantry rails.
1. **Always be within arm’s reach of the E-Stop buttons.**
1. If anything goes wrong press the E-Stop for both the machine and the spindle. This includes: the work piece becomes no longer secured, the end mill breaks, the gantry moves in an unexpected way, etc.
1. Turn off the spindle when your job is complete.

## Before leaving

1. Move the CNC to the home position.
1. Clear the machine bed and put away clamps, etc.
1. Use the dust collector hose to clean sawdust/chips off of the machine bed, rails, and area around the CNC.
1. Sweep/vacuum any chips off the floor.
1. Press the “Stop” button on the spindle paddle switch, even if it appears off. Press the button on the badger to badge out.
1. Press the "Stop" button on the CNC paddle switch. The light under the gantry should be off.
1. Ensure that you have all your end mills and materials.
1. Close the laptop lid.

## Allowed materials:

* Hard wood and soft wood, except excessively sappy/green wood
* HDPE
* Aluminum and brass, with special training

## Other

* You must provide your own end mills and cutters.
* Do not remove the spoil board.
* Do not remove the Musclechuck. It is clocked to the spindle in a specific position to minimize runout.
* Do not change settings on the machine or in the sender.
* **VCarve file version compatibility**: if your local version of VCarve is newer than the CNC laptop, you may need to update the CNC laptop version.
* **Fusion360 post process settings**: Post process using the "Grbl / grbl" post. In "Safe retracts and home positioning" (under "Post properties"), set "Safe retracts" to "Clearance Height".
   * After the job finishes, "Clearance Height" will retract the spindle to the clearance height of the last cut.
   * "G28" and "G53" will attempt to move the spindle to the G28 or G53 origin after the last cut, which may result in unexpected movement that could collide with your stock or clamps.