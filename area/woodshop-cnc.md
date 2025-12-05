---
layout: area-policy
order: 2
title: Woodshop - CNC
discord_channel_name: "#woodworking"
discord_channel_url: https://discord.com/channels/775417143029661748/775418072428970076
stewards: "@steward (cnc)"
---

## Before cutting

1. The CNC requires certification to use.
2. Press the “Stop” button on the spindle paddle switch and badge in before setting up to check your certification is valid.
3. Home the machine before doing anything else
   1. Re-home the machine if you crash the spindle (you can re-home just Z if crashed only in Z)
4. Check that there is nothing that could interfere with the motion of the CNC gantry (e.g. snagged wires, material in the way, etc)
5. Check the router RPM setting matches what is expected in your design.
   1. 1-6 is 8000-24000 RPM, with 3.5 being around 16000RPM
6. Place your stock on the spoil board and clamp it down. It should not move if you try to push or pull it with your body weight.
7. Ensure the correct bit for your cut is inserted and secure.
   1. With the Musclechuck, this means tightening the bolt until finger-tight, then turn another quarter turn with the allen key. Note that overtightening risks damage to the chuck.
8. Zero the machine relative to your stock based on the origin you specified during tool path generation.
9. Use the “outline” feature of gSender to ensure the cutter and router will not collide with any clamps (or manually jog the machine around).
   1. It’s worth raising the endmill above any clamps or fixtures initially to avoid accidentally crashing if adjustments are needed.
   2. Be aware the “outline” feature attempts to calculate a concave hull, but this sometimes yields an outline that exceeds the actual toolpath.
10. Jog the machine above your stock and within the tool path outline. (This just helps avoid crashing when starting the job)
11. Attach the dust boot and turn on the dust collector.
12. Turn on the spindle.
13. Start your job.

## While cutting

1. Keep hands and feet clear of the machine, especially the cutting area, gantry, and rails.
2. Do not lean over the machine bed.
3. Always be within arm’s reach of the E-Stop buttons.
4. If anything goes wrong press the E-Stop for both the machine and the spindle. This includes: the work piece becomes no longer secured, the end mill breaks, the gantry moves in an unexpected way, etc.
5. Turn off the spindle when your job is complete.

## Before leaving

1. Press the “Stop” button on the spindle paddle switch, even if it appears off. Press the button on the badger to badge out.
2. Move the CNC to the home position.
3. Use the dust collector hose to clean the machine bed, rails, and area around the CNC.
4. Sweep/vacuum any chips off the floor.
5. Close the laptop lid.

## Allowed materials:

* Wood
* HDPE
* Soft metals (with special training)

## Other

* You must provide your own end mills and cutters.
* Do not remove the spoil board
* Do not change settings on the machine or in the sender.
* TODO VCarve version differences?
