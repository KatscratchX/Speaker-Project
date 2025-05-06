**Short description**

Wall mounted 3D printed passive speakers for a home desk/ studio setup with bluetooth and Aux connectivity. Took me a month (mostly weekends) to plan the sound output, source the drivers, electronics and metal parts, model the body, print, assemble and iterate the speakers.
All designs are original.

**1. Introduction**

I've always wanted a clean, wall-mounted speaker setup that sounds as good as it looks next to my workstation. This project started as a simple idea and turned into a deep dive into speaker acoustics, enclosure design, and electronics.
![image](https://github.com/user-attachments/assets/f0f38e97-aa82-43ea-9967-929a373306f0)

**2. Planning**

As i delved deeper into studying speaker enclosure design, to get a really decent bass, a ported and larger body is best suited.
I wanted to have an overall flat response so that i can enjoy all genres of music and listen to media/ movies , I opted for a Mid bass and tweeter driver combination.

**3. Component selection and sourcing**

I used VituiXCAD to simulate the frequency response i am looking for and replaced the driver variables (FRD/ ZMA) from the online vendor's list of available drivers. https://kimmosaunisto.net/
The combination that gave me a decent response was using a 30 watt (RMS), 60 watt (Max) Dayton mid bass driver a Dayton 30 watt tweeter.
Adjusting the Inductance and capacitance can make all the difference in getting a decent overlapping region for the tweeter and mid bass!

![image](https://github.com/user-attachments/assets/d14399c6-adc9-46e0-8d69-e0bb43710556)

I followed Kirbymeetsaudio's tutorial to get started - https://www.youtube.com/watch?v=kJqvjjyHqqA&t=1500s&ab_channel=KirbyMeetsAudio

Crossover components :
1. Dayton Mid Bass driver - [https://diyaudiocart.com/product/dayton-audio-nd105-aluminum-cone-midbass-neo-driver-4ohm/]
2. Dayton Tweeter driver - https://diyaudiocart.com/product/dayton-audio-nd16fa-4-soft-dome-neodymium-tweeter-4-ohm/
3. Capacitor - https://diyaudiocart.com/product/bevenbi-2200uf-100v-electrolytic-non-polarized-crossover-capacitor/ & https://diyaudiocart.com/product/bevenbi-3300-uf-63-v-low-esr-aluminium-electrolytic-capacitors-leaded/
4. Inductor - https://diyaudiocart.com/product/dac-082mh-air-core-inductor-crossover-coil-18-awg/ & https://diyaudiocart.com/product/dac-0-15mh-air-core-inductor-crossover-coil-20-awg/
5. Resistor - https://diyaudiocart.com/product/weet-33-ohm-20w-precision-audio-grade-resistor-1/

Chose a blueooth and AUX input compatible DAC (Digital to analog audio convertor) and powered it using a 12V buck converter. Links to the components - https://inkocean.in/products/ink202-inkocean-ink202-2-1-50-50-100w-class-d-amplifier

In order to convert the speakers into a device detectable in the apple home system, I installed homebridge and shareport sync in raspberry pi 4B.

**4. Circuitry**

![image](https://github.com/user-attachments/assets/ae5ac245-f4b7-4c69-a3e8-415df1c5dd6b)
![image](https://github.com/user-attachments/assets/65c9b127-8523-4102-b574-f9076fdab16b)

**5. Enclosure design**

Replaced the driver dimensions in this calculator to find out the appropriate box volume - 7Litres in my case
https://www.diyaudioandvideo.com/Calculator/SpeakerBoxVolume/

![image](https://github.com/user-attachments/assets/f33bebe2-94ef-44a0-b9ef-2ac1af19d314)
Modelled in Rhino 8, basic rhino rendering.

**6. 3d printing**

Printer - Bambulab P1S
Matte PLA - Black, White, grey and red
Total printing time - 54 hours, 26 hours for each unit.
Total material weight - 2,132 grams
![image](https://github.com/user-attachments/assets/ca294124-ab2a-4276-84ef-dffffb6594ee)
![image](https://github.com/user-attachments/assets/a1a7e858-0654-4b1c-9fd4-8d25fdb75e7a)

**7. Assembly**

![image](https://github.com/user-attachments/assets/11c45249-71fc-4b39-acb5-cb6d954bcb88)

- 2 Insert nuts for holding the 4 pieces of the body together.
- 4 screws to hold the drivers to the mounting plate body
- 2 screws to hold the drivers on to the mounting plate
- 6 magnets + 6 washers for holding the Grill onto the body
- Once assembled, two layers of foam sheets was wrapped and glued inside the body walls to prevent sounds leakage and reverberation.
- Double sided foam tape wherever the parts were vibrating against each other during high volume bass.

**8. Tuning the speaker**

As i tested out different types of songs, I realised the bass was getting affected by the parts vibrating against each other because of the massive air displacement. The solution was to fill the gaps with the foam sheet which we get in usual amazon packaging.

