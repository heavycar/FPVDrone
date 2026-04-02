##If you don't know any terms mentioned here, check the end of the page ther will e a glossary
Ok, so like i said in the last commit i don't know where tf to start so i asked chatgpt to recommend me a battery for the fc, and it said to use a 4S li-po around 1200mah for 1500, and ≥ 75C (ideal 80–120C) idk what does this "C" stands for but it said that is cheaper, more realiable and better for initial fpv projects with low budget
It said that if i want more power i can use a 6S one but i don't think i need something like this, i can just upgrade it later, it said something about a "Voltage sag" that a 6S battery has less than a 4 one, i'll leave all complicated terms in the glossary don't worry
And i can't get a super big battery like 2200mah because it can weight so much that the 45A motors will have to reach near it's full capacity to lift it, and when it reaches it comes to be less efficient so it's actually worse
and no low C rating battery, still no idea of what tf is this
I can't take a 6s battery without knowing the motor KV rating, all those words and terms in the glossary :)

It reccomends me to use a 4S 1300mAh 100C LiPo with a commong XT60 connector.
  Voltage: 4S (14.8V)
  Capacity: 1300–1500mAh
  Discharge: ≥75C
  Use case: 5” freestyle / beginner
I should buy 3 or 4 of those because it don't last so much, 

I'm thinking about getting 2 batteries of 1500MAH 4S 120C with 14,8V from ChinaHobbyLine that is actually not just a store but a whole industry so i think it's good

Glossary
-  Li-po | this is bassicaly a type of battery, it exists, li-ion, life-po4 and other type of batteries=
-  S (Cells, seriess) | examples: 4S, 6S, this is how the battery is mounted, because inside of one 4S battery for example there are 4 smaller batteries wired in series and in a 6S there are 6 batteries wired in series
-  mAh (Milliamp Hour) | This is a measure unit for battery capacity to do a better understading let's take a 2000Mah battery, it means that this battery can give you 2000 mili amperes for one your or 2 amperes for an hour (this is therically it obvious will waste energy on heat and will not be 100% efficient)
- C rating | It means how much power the battery can give you | Formula: Max Current = (Capacity in mAh : 1000) * C So if we take a battery with 1300mah it is 1.3Ah with 100C points we make: Max current = 1.3 * 100 So Max current = 130A this is the max the battery can output, Sometimes it's fake, exaggerated, or real but under very favorable conditions that generally don't occur.
- Voltage Sag | it is basically the voltage drop when the drone requires too much current in a very low timing, like if each drone motor is running at 15A And suddenly push the joystick up and it starts running at 40A, there will be a low in the current because of the spike in current it's cased by: low C rating, bad battery quality, old "tired" battery and it can cause" instability in flight and even fall.
- XT60 connector | is the connector between the cable that is soldered in the FC and the battery, if you don't use a connector and just put the battery directly welded into the FV you won't be able to change the battery, that's why you use a connector.
- ESC | this is what turn the commands that the FC controller sends into actual high power to the motors , think of it like a translator between your brain(FV) and your muscles(Motor)
- KV rating | i din't really understand so to avoid talking shit i'll just put what chat gpt said: Motor speed constant (RPM per volt) | 👉 Higher KV:faster motor, less efficient and used with lower voltage (4S) Lower KV: slower motor, more efficient and used with higher voltage (6S)
- Efficiency (in FPV context) so efficiency is basically how optimized your drone is, Bad efficiency means more energy beign wasted into heat consequentially less flight time because energy that could be used in motors is beign wasted and more battery stress | good efficieny means less heat, more flight time and smoother perfomances


Battery chosen to be used by now: https://chinahobbyline.com/products/cnhl-ministar-series-1500mah-14-8v-4s-120c-lipo-battery-with-xt60-plug?variant=43581309092054

Here are some images to help you better understanding things
Series and parallel connection.
When you connect a batterie in parallel all the negative and positive are conected together, voltage doesn't rise but battery total capacity does

<img width="328" height="546" alt="Screenshot_20260402_180454" src="https://github.com/user-attachments/assets/5835ad9c-3527-4b6b-b3e2-d427be74982a" />

in series if u battery 1 and 2 and connect battery one negative and connect to positive of battery two you just made a series connection, capacity doens't rise but voltage does

<img width="328" height="546" alt="Screenshot_20260402_180537" src="https://github.com/user-attachments/assets/adaba3f3-1da1-4bb0-a15c-7a862399aa93" />

C rating thing

<img width="365" height="160" alt="RNAV3" src="https://github.com/user-attachments/assets/375ef200-24d9-40fd-bfb0-53e6d4cd88c3" />

Remember that the Amp  hours shown in the first and third are Ah not mAh, quick reminder that Ah means mAh : 1000 and mAh means Ah * 1000 simple equations to discover max amps a battery can deliver, how much time can a battery last with certain charge and the discharge charge value 

this image shows how voltage sag happens, we see clear voltage waves and probably when suddenly a high power is demanded the voltage drops

<img width="977" height="526" alt="Voltage-Sag" src="https://github.com/user-attachments/assets/5850e42b-0926-449b-89e6-b7866e062793" />

Thsi image shows a XT60 connector, a connector rated for high current and high temperatures
![XT60-Male-Female-Pair-Closeup-sq-jpg](https://github.com/user-attachments/assets/3bfa34b7-fc95-4cd9-bba8-7ee9df95cece)
This is all you need to see about those stuff
