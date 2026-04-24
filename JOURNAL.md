---
title: Coaxial Swerve Drive Base (Flowstate)
author: Ziqi Guan
description: This will be a four-wheel coaxial swerve drive robot. It will just be a drive base; however, it is completely custom. 
created_at: 2026-4-23
---
### Total time spent: 0 Hours

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

I also did some part lightening on the wheel so when it is 3D printed, it can be printed at 100% infil without much worry and also for aesthetics. 

Here is an isometric view:
![Isometric view ofthe partlightened wheel](Images/CADImages/Day1/WheelPartLightenedSideIsometricView.png)

After getting the wheels made, I switched to making the mounting plate as it also determines things like bolt mounting points, size of the module, etc. Here is a halfway done version that was good enough to get started with the support brackets for the wheels. 

![Top view of the halfway done mounting part](Images/CADImages/Day1/MountingPlateHalfwayProgressTopView.png)

Also as a side note, I modeled the bearings I want to use as Swerve Drive Specialties, the vendor I plan on getting 4" x 3.5" x .25" bearings from doesn't have a CAD or drawing, so I based it off of my best guesses for the size. It turns out that my guess was very close to the actual dimensions, so I didn't need to redo anything there. 

![Top view of the bearing](Images/CADImages/Day1/4in-x-3.5in-x-.25inBearingTopView.png)

The brackets to mount the wheel onto took a surprising amount of time as a lot of its geometry matters. I initially had a very rounded design, but I eventually settled on this very angular design. A key thing about the 

![Day 1 progress (Above Isometric View)](Images/CADImages/Day1/DayOneProgressIsometricViewAbove.png)