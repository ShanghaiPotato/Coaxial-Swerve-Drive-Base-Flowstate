---
title: Coaxial Swerve Drive Base (Flowstate)
author: Ziqi Guan
description: This will be a four-wheel coaxial swerve drive robot. It will just be a drive base; however, it is completely custom. 
created_at: 2026-4-23
---
### Total time spent: 0 Hours

#### Onshape Link: https://cad.onshape.com/documents/4e4e67b789c32e1c62490b55/w/3b147ca839286fae5a01baae/e/5d2ccd93d79c945d351b1f5a
## Day 1 - Designing the Base of the Swerve Drive - April 23rd - 0 Hours

Today was just laying down the basics of the swerve drive by making the individual module. I did some research into which motors I want to use, and I decided to use the HD Hex motor and the Core Hex motor from Rev Robotics because they have a small form factor and are brushed motors. The brushed motors allow me to use cheaper motor controllers instead of the expensive $50-100 dollar ones that can be sold online. 

Here is a link to the HD Hex motor and Core motor respectively:
https://www.revrobotics.com/REV-41-1291/
https://www.revrobotics.com/rev-41-1300/

The motor controller is the next big part of this project, and I found one relatively quickly that meets all the requirements. It has a 8 A continous current rating and a 15 A peak current rating. The HD Hex motor has a stall current of 8.5 A and the Core motor has a stall of 4.4 A. That is 12.9 A combined at stall, and it works perfectly. Each motor controller can support 2 motors, so there can be one motor controller for each module, simplifying everything significantly. The only issue is that they only have 2 left in stock, so I would either have to wait or find a new motor controller. 

Here is the link to the motor controller I plan on using: 
https://www.robotshop.com/products/dual-h-bridge-dc-motor-controller?srsltid=AfmBOoro6QaIrc8azvvy7qUHnBC8t_rmFe9d5oKzDVSwgjFejJFZqI1GqEc

That was just the research to get started, here is the actual CAD that was worked on most of today. 

![A front view of the bevel gear assembly](Images/CADImages/Day1/FrontBevelGearView.png)

I started off with just making a rough 3in wheel and then made the bevel gears that attatch to the sides. Starting off here is important because the entire module is built around the diamter and thickness of your wheel. The bevel gear runs at a 4:1 reduction, and it is one of two reductions from the motor to the wheel. The wheel is also driven by a .5in hex shaft because I am already getting a lot of items from Rev Robotics, so integrating the items they sell into this project would reduce the number of vendors to buy from. I also have access to a bunch of tools from my FRC team that can help in cutting the hex axles. In the future if I have the budget, I would like to CNC metal bevel gears instead of 3D printing them for reliability, however, because of costs its not very feesable. The robot as I envision it likely won't go under heavy load as it will only weigh approximately thirty to forty pounds at most. 

Here is a side view:
![A side view of the bevel gear assembly](Images/CADImages/Day1/SideBevelGearView.png)

Here is just the driving bevel gear:
![Isometric view of the driving bevel gear](Images/CADImages/Day1/BevelDrivingGearIsometricView.png)

I also did some part lightening on the wheel so when it is 3D printed, it can be printed at 100% infil without much worry and also for aesthetics. 

Here is an isometric view:
![Isometric view ofthe partlightened wheel](Images/CADImages/Day1/WheelPartLightenedSideIsometricView.png)

After getting the wheels made, I switched to making the mounting plate as it also determines things like bolt mounting points, size of the module, etc. Here is a halfway done version that was good enough to get started with the support brackets for the wheels. 

![Top view of the halfway done mounting part](Images/CADImages/Day1/MountingPlateHalfwayProgressTopView.png)

Also as a side note, I modeled the bearings I want to use as Swerve Drive Specialties, the vendor I plan on getting 4" x 3.5" x .25" bearings from doesn't have a CAD or drawing, so I based it off of my best guesses for the size. It turns out that my guess was very close to the actual dimensions, so I didn't need to redo anything there. 

![Top view of the bearing](Images/CADImages/Day1/4in-x-3.5in-x-.25inBearingTopView.png)

The brackets to mount the wheel onto took a surprising amount of time as a lot of its geometry matters. I initially had a very rounded design, but I eventually settled on this very angular design. A key thing about the mounting brackets is the area it contacts the bearing, as more areas of contact reduce the pressure applied. There are also hex holes for 3/8in nuts so using a wrench isn't required. 

![Above isometric view of the mounting bracket without the bevel gear](Images/CADImages/Day1/NonBevelWheelMountingBraceIsometricViewAbove.png) 

![Below isometric view of the mounting bracket without the bevel gear](Images/CADImages/Day1/NonBevelWheelMountingBraceIsometricViewBelow.png)

![Above isometric view of the mounting bracket on the bevel gear side](Images/CADImages/Day1/BevelWheelMountingBraceIsometricViewAbove.png)

![Below isometric view of the mounting bracket on the bevel gear side](Images/CADImages/Day1/BevelWheelMountingBraceIsometricViewBelow.png)

In the holes, 1.125" OD .5" ID hex bearings are going to support the weight of the entire drivebase. There will be a hex axle that runs through everything. Between the mounting brackets and the wheel itself, there will be snap on 3D printed spacers that will constrain the motion more securely. They are different sizes because the distance between the wheel and the mounting brackets are different on both sides. This is because the bevel gear adds significant thickness. 

![Isometric view of both snap on spacers that will go onto the shaft](Images/CADImages/Day1/BothSweveDriveSpacersIsometricView.png)

The next order of business was to finish off the entire mounting plate that the wheel mounts would be attatched to. While the basic plate was done, the motion transfer of turning the entire module still needs to be figured out. Because I'm trying to make ths build requiring the least amount of specified hardware as possible, I decided to just use helical gears in a V pattern instead. The mounting seems incredibly chunky, but it houses everything inside of it, including the motion transfer to power the wheel itself. The large slot holes the helical gear that transfers the motion. 

Here is a top isometric view of it:
![Above isometric view of the finished mounting plate](Images/CADImages/Day1/FinishedMountingPlateIsometricView.png)

Here is the same isometric view with the driving helical gear shown. It is running on a 2:1 reduction. 
![Both gears are shown here](Images/CADImages/Day1/MountingPlateWithOtherHelicalGearIsometricView.png)


Another thing that also needed to be completed was the top mounting plate. Not only did it help clean up the look, it also constrains the motion of the gears so they cannot pop up. 

![Top view of the mounting plate bracket cover](Images/CADImages/Day1/TopBracketMountingTopView.png)

The inside helical gears that transfer the motion is geared at a 1:1 ratio and are incredibly simple. On one end, it is constrained by a tiny bearing, and the other end has a hex axle with a hex bearing. 

![Above isometric view of both helical gears](Images/CADImages/Day1/SmallerInteriorDriverHelicalGearIsometricViewAbove.png)

![Below isometric view of both helical gears](Images/CADImages/Day1/SmallerInteriorDriverHelicalGearIsometricViewBelow.png)

The final thing is the mounting for it all. I decided to just make a basic shape and polish it up with mounting hols later just so it is easier to visualize. It is two plates, one on top and one on the bottom, that "captures" the bearing inbetween, holding the entire module down securely. Because it is two parts, there are six holes around the center that allow the use of bolts to secure everything properly. There is also a hole for mounting the other helical gear. 

Here is a view of both parts:
![Isometric view of both support plates](Images/CADImages/Day1/SupportPlatesIsometricView.png)

Here is an isometric view of just the top panel: 
![Isometric view of the top support plate](Images/CADImages/Day1/SupportPlatesThickIsometricView.png)

Here is an isometric view of just the bottom panel:
![Isometric view of the bottom support plate](Images/CADImages/Day1/SupportPlateThinIsometricView.png)

Here is a top view with all of its geometry: 
![Top view with all of the geomtry visible](Images/CADImages/Day1/SupportPlatesTopView.png)

Here are just some visualization photos of everything done so far in one piece. If anything is unclear/hard to see, the link to the OnShape document is linked at the very top of the journal for easy reference. 
![Day 1 progress (Above Isometric View)](Images/CADImages/Day1/DayOneProgressIsometricViewAbove.png)

![Day 1 progress (Below Isometric View)](Images/CADImages/Day1/DayOneProgressIsometricViewBelow.png)

![Day 1 progress(Side View)](Images/CADImages/Day1/DayOneProgressSideView.png)

![Day 1 progress (Front View)](Images/CADImages/Day1/DayOneProgressFrontView.png)

![Day 1 progress (Top View)](Images/CADImages/Day1/DayOneProgressTopView.png)

Anyways, that was about everything done today so far, and the next task is to create the motor packaging that will power this entire setup. 