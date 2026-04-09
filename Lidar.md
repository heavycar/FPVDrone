What many people don't know is that you can actually add a lidar sensor to your project, is much more practical and useful in normal drones not fpv, but you can add it maybe by curiosity

So what is a lidar sensor? Lidar stands for "light detection and ranging" 

It works bassicaly like this:

It emits and light pulse(IR light pulse)

the light hits something it can be anything, ground, walls, it works for almost all, not very good in reflexive objects

the light comes back and hits the sensor

it estimates the time the pulse took from going to getting back

This thousands of time per second

each measure turns into a tiny dot, it creates thousands and thousands of dots for each angle, each second it works

then a scripts take this dots and put it all together in a 3D environment, creating then a tool that gives the receiving computer the ability to "see the world 

All this process it's called SLAM (Simultaneous Localization And Mapping)

How to put it in a drone

you can really do huge systems for this so we are going into levels

Basic level:

Only one lidar, it analyses the distance continuously, if distance < X = alerts the FV by script, it brakes

Intermediary level:

you use multiple lidars such as in the front, in the back, in the top, in the bottom, each lidar analyses it distance like in the first model, this creates a bubble all over the drone, with don't let it hit anything theoretically

Advanced level:

No multiple lidars, one big, heavy rotating lidar, it uses SLAM, so it creates a 3D map of the relief which doesn't get lost, it can use the map again, bassically remembering where it was, walls, obstacles, building

Lidar is overkill at all for an FPV because due to the high speed that fpv goes the lidar depending on the model can either don't catch details or miss everything and braking protocols can not work due to the high speed

It has multiple limitations

Cheap lidars can have:

Poor quality, don't catch details

Poor angle

and can work worse in high speeds

Advantages / functions

altitude hold, by measuring the distance between the ground it can maitain it altitude without fully depending on GPS

Avoid floor and other obstacles

That's how it works, but why is it so expensive, while beign so good

Stupid speed
It measure with nanosecond precision

If it's off by 1 ns (1 billionth of a second) it misses by 0,15m

How do they do that?

TDC (Time-to-Digital Converter) insane speed

high-frequency counters (effective hundreds of MHz or GHz)

Multiple measurements plus averaging to reduce noise.

Why is it so expensive:

Ultra-precise timing circuits are not just ordinary MCUs.

Any noise in the circuit or anything that shouldn't be happening turns into distance inconsistency

PCB layout and clock must be really controled

Few engineers of this area in the world which results in high paying which then it's converted into high price

Lens must be micrometically precise or unfocused laser beam = Distance inconsistency

High processing power needed

It needs to do millions of calculations per second, compesate this and that, filter noise and correct errors, no other ordinary MCU can do that 

Complex firmware

In resume that are many things that can go off but don't in a LIDAR that's why it's so expensive    

What should i use, here's a board

Basic, very basic

Sensor model: VL53L0X

What should you expect:

Range: 2km

Accuracy: reasonable, variation of cm difference.

Range of view: narrow

Interface: I2C

Where to use:

Avoid ground functions, low altitude

Tiny robot

experiment

indoor drone

limitations:

uselles at outdoor

do not work for fast obstacles avoiding

much low range

Intermediary

Sensor model: TF-luna LiDar

What expect:

range: 6-8m

frequency: high(fast)

interface: UART/I2C

Good precision and stability

Where to use:

FPV drones for basic functions such as altitude from ground

Avoid colissions

real basic automation

limitations:

only reads in one direction

don't create 3d map(SLAM) by itself

still not very useful with high light interference or sun

Advanced

Sensor model: RPLIDAR A1 360

What expect:

Range: ~12m

2d map creating

360 reading

precision: 

Distance           Error

1m               ±1cm

3m               ±3cm

10m              ±25cm

range of view: 360

where to use:

Autonomous drones 

smart hitting avoid

Autonomous robots

Environment mapping

Limitations
Need high power processing for 2d map that FC ussualy don't provide    

heavy

need external algorithm

All that is bassically useless for an fpv because if you want something lightweight and cheap then it wont have enough range, precion or reacting time but if you want something with high range and high precision the it won't be cheap or lightweight
