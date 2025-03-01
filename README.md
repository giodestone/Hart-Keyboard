# Hart Keyboard

![Hart keyboard on a white background](https://raw.githubusercontent.com/giodestone/Hart-Keyboard/refs/heads/dev/Images/Image2.jpg)

Hart is a 80% ISO layout 3D-Printable, hand-soldered keyboard based on the RP2040 platform (Raspberry Pi Pico 1), and Cherry MX Brown-like switches. It is supposed to be cheap, achievable, and usable.

This is my first DIY keyboard, so it is a bit rough around the edges. 

I suggest using this a reference for making your own keyboard, rather than trying to 3D print it (but if you do - please open an issue/pull-request with your build pictures!).

If you are thinking of building your first Keyboard and are new to CAD, 3D printing, and microcontrollers - build a numpad first. Or you can buy kits off websites where you solder it yourself but still pick the parts.

## Features
* RP2040-based (Raspberry Pi Pico 1)
* Rotary Encoder
* 128x64 SSD1306 OLED Display
* [Luna Keyboard Pet](https://www.youtube.com/watch?v=HgIQRazCAjo)
* 3 'extra' buttons (currently as F13-F15)
* Tenkeyless/80%-ish layout (full f-row)
* ISO Layout (menu key-less)
* Compact
* Relatively thin
* QMK-based
* Cherry-compatible switch design

## 🛒Bill of Materials (BoM)
This keyboard should cost £70-100 to make.

* About 500g of filament (actual requirement is much lower)
* 90x switches - I used lubed Gatreon Brown from Glorius, as 120x is only £35.
* 90x keycaps, some with Cherry-style or Costar style stabalisers.
    * 1x 6.25u key (stabalised)
    * 1x 2u key (stabalised)
    * 1x ISO enter key (stabalised)
    * 2x 1.75u
    * 2x 1.5u
    * 2x 1.25u
    * 81x 1u
* 90x 1N4148 diodes
* 30cm of steel wire
* 2x paper clips
* 1x SSD1306 OLED
* 1x EC11 Rotary Encoder
* 1x RP2040 (micro USB)
* 1x USB C breakout board ([for it to work with a USB C to C cable, some resistors are needed](https://www.youtube.com/watch?v=X6A6_k5L0_g))
* 1x Micro usb spare cable (for getting between RP2040 and breakout board)
* 1x Adhesive (e.g. superglue)
* 2x 2u Costar stabaliser wires (or 2x paperclips and necessary tools to manipulate them)
* 1x 6.25u Costar stabaliser wire (or gauge 20 steel wire + necessary tools)
* for the back (subject to change)
    * 7x M3 nuts
    * 7x M3x8 bolts or screws

## 🔨Tools
* Access to a calibrated, reliable 3D printer.
    * and related tools for 3D print refinement such as a file/sandpaper.
* 1x flush cutters (aka snips)
* 1x ruler
* 2x needle-nose pliers for stabaliser wire creation (or 1x needle-nose plier, 1x wire straightener/double nylon jaw)
* 1x soldering iron with your preferred tip (I used a Pinecil - highly recommend)
* 1x solder sucker (I used a SS 02 Ali-Express clone - it was 10x better than my previous one and cost only £4)
* 1x rosin-core lead-free solder spool
* 1x spool of enamelled wire for wiring everything together
* 1x roll of electrical tape (I used white)


## 💭Design Choices
First, I had to establish some goals, these ended up being:

1. Usable
2. Achievable
3. Cheap

After thinking about it some more, the keyboard had to:
* have a familar/standard-ish layout.
* be compatibile with a computer running Windows.
* be quiet enough.
* be novel enough so I remain interested as to finish it.
* be achievable with the tools and knowledge I have.
* use generally avaliable parts.
* use cheap parts.

So, that's why it was 3D-printable, uses the RP2040, and has some gimmicks.

### ℹ Useful Links
> 👁: Inspiration |
> 📖: Guides/documentation |
> 🎁: Parts

- 👁 General Inspiration: [Gallery](https://imgur.com/gallery/P90jZJq), [Reddit Thread](https://www.reddit.com/r/MechanicalKeyboards/comments/qaxoyn/built_my_own_3dprinted_handwired_keyboard/)
- 👁 [Sick68 3D Printed Keyboard for Reference](https://www.thingiverse.com/thing:3478494)
- 👁 🎁 [Fully 3D Printed Keyboard with Costar Stabalisers](https://fornellas.github.io/3d_printed_keyboard/design.html)
- 👁 [Another Stabiliser](https://www.thingiverse.com/thing:4747414)
- 📖 [Comprehensive Guide Building (not designing) a Keyboard](https://matt3o.com/book/)
- 📖 [Reddit wiki on Handbuilding a keyboard](https://www.reddit.com/r/MechanicalKeyboards/comments/4l0p41/guide_detailed_guide_to_making_a_custom_keyboard/)
- 📖 [Keycap Guide](https://www.reddit.com/r/MechanicalKeyboards/wiki/keycap_guides/)
- 📖 [Keyboard Wiki (terminology, overview of all components etc.)](https://deskthority.net/wiki/)
- 📖 [Easy DIY Key Legends](https://www.youtube.com/watch?v=bnU0FQforaw)
- 📖 [QMK Guides for Layer setup](https://thomasbaart.nl/category/mechanical-keyboards/firmware/qmk/)
- 📖 [Beginners guide to switches](https://www.theremingoat.com/blog/beginners-guide)
- 🔧 [Keyboard Layout Editor](http://www.keyboard-layout-editor.com/#/)
- 🔧 [Keyboard Layout to STL Generator](https://kbd.news/Keyboard-layout-STL-generator-1259.html)
- 🔧 [Keyboard Layout to CAD Drawings](http://builder.swillkb.com/)
    - [Alternative tool](https://github.com/swill/kad)
- 🔧 [keebcu - a customizer for 3d printable keyboard cases](https://github.com/andimoto/keebcu)
- 🔧 🎁 [Keycap Generator](https://www.thingiverse.com/thing:2783650)
    - 🔧 🎁 [Github Link (Heavily reccomended)](https://github.com/rsheldiii/KeyV2)
- 🎁 [3D Printable Cherry Stabaliser](https://www.reddit.com/r/MechanicalKeyboards/comments/lv7l8t/i_made_simple_3d_printable_stabilizers/)


### 🖼 Aesthetics
[I really liked this DIY keyboard](https://imgur.com/gallery/custom-3d-printed-handwired-keyboard-P90jZJq). It was dead simple so, and aesthetically pleasant. I wanted it to be even smaller, as space is tight on my desk so I hid the diodes.[Mysterium v2 was another keyboard](https://github.com/coseyfannitutti/mysterium) I found interesitng. There's quite a few more, but these were the main ones.


### 🗺 Layout

I wanted the layout to be as close as possible to an ISO full layout, and also compact. However, as I wanted extra features it would not be possible to make a 100% layout due to microcontroller limitations (it is diffuclt to find a controller with more than 25 GPIO pins - you can connect them). This is fine, as I could create a numpad at a future date.

I wanted a fn layer (i.e. F-keys pretend to be something else) for volume keys, additional media controls, and brightness adjustment. You can get very elaborate with this, even making the number row be the f-row - but I program so I wanted easy access to the F5 button.

I used to have a keyboard that had macro keys. I found them to be more useful as extra f-keys as virtually a lot of software supports them (surisingly), and they're left unbound. So I can have a safe push to talk button. I never found the macro feature useful (but it can be added to the firmware easily).

The layout was based off my Dell laptop, which has an ISO layout. I did this because I was familar with it and thought it was good enough.

I could have tried an ortholinear or differnetly-staggered keyboard (i.e. how e.g. the QWE and ASD keys align). But I don't think this was bad. I like QWERTY because that is what I am familar with.

### 💅 Ergonomics

I like flat keyboards. I think the non-ergonomic layout is fine. I wanted my keyboard to be one piece for these reasons - and upon further investigation getting the two sides to connect can be tricky.

The thickness of the keyboard was important. In the case of using Cherry-like switches, the thinner the better. I didn't want it to be much thicker than my current one.

Since, I have used a Microsoft Ergonomic Keyboard 4000 and really like the reduced wrist strain - but also think it can be improved quite a bit especially typing feel and reducing the size footprint.

### 🎪 Gimmicks (Rotary Encoder, Display)

I saw a video of Luna, a companion keyboard pet. It responds to your typing. I really liked it. Plus I always found the indicator LEDs ugly.

I had a keyboard in the past with a scroll wheel for volume adjustment. I really liked it, but I thought it felt cheap and looked bad (though arguably more ergonomic). I also wanted the volume controller to act as media controls.


### 🎹 Keys

#### Keycaps
The keycaps were flat as they print well, and I like the aestetis and feel of flat keycaps 
(that's what I'm used to from the keyboard).

They were generated using the [Key V2 Library](https://github.com/rsheldiii/KeyV2), and tweaked using OpenSCAD. Note you need the nightly version, and you need to look through the issues if you want a fix for a stem generation easy.

You can just buy the keycaps, but make sure you have a compatible spacebar. Its probably similar material cost wise and much easier.

#### Switches
There are a multitude of switch formats to pick from. Cherry-style are the most prevelant so I went with them. I would have picked low profile, if they weren't both out of stock and overpriced (well.. unless I wanted the ones with a Choc-style stem, which the keycap generation library did not support - and at the time of writing, still doesn't).

There's a much better article explaining this in the useful links section. All you need to know: switches affect the price, sound, and feel the most!

#### Stabalisers
Stabalisers are the things that stop the larger keys (space, enter, backspace, right-shift) from wobbling and being near unusable. 

I chose Costar-style as I wanted to make the keyboard as 3D printable as possible, and they seemed actually printable on an FDM printer versus the cherry style. Costar, is also reportedley more stable than Cherry, but a bigger nightmare to take apart. 

Assembly of this took up an inordenate amount of time and effort causing undue frustration, but unless you buy screw-in cherry kit (and ensure your plate + layout can accomodate), then this is your best option. Homebrew methods are possible too.   


### 🔌 RP2040
I wanted a keyboard which was as close to a full layout, with support for a display and rotary encoder. 

This means I needed:
* at least 21 pins to create a matrix (but I used 22 foolishly)
* 2 for the rotary encoder (note that it is wired into the matrix - i.e. you need 1 matrix slot for this)
* 2 for the display (SDA/SCL - this is the I2C SSD1306 - which uses less pins than the SPI). 
* This is exluding 3.3V/5v (5v aka VDD) & GND for the OLED and GND for the rotary encoder (they do not use data)
* Enough headroom for an OLED display and some images to be stored (8kb per image frame).
* USB OTG/HID device mode (so the Pi can pretend to be an input device)

Pico Pinout Image: https://www.raspberrypi.com/documentation/microcontrollers/images/pico-pinout.svg
Pico Pinout Website: https://pico.pinout.xyz/

The Pi Pico has 25 usable GPIO pins (26 if you count the one used for the built-in LED). This means it has enough for the matrix and rotary encoder (which uses GPIO pins). It has 2 I2C controllers (IC20 and IC21), making it suitable for the I2C based SSD1306 display. The RP2040 I got was the reference one. It had 16MB of 'storage' and 264KB of RAM (there are the variants that have as much as 64MB of 'storage') - enough for storing plenty of imaes. Two community-based keyboard firmwares support the RP2040: QMK (C-based) and KMK (Python-based). The RP2040 can also 'pretend' to be a USB keyboard. Finally, the price was good - about £4. Therefore, the RP2040 was chosen.

The RP2040 was not as well established when this keyboard was spec'd out (late 2022). But it appered that everything worked as intended.

#### Type C Port
I wanted for the keyboard to have a type-c port as it allows for swapping out of the wire, and easier packing away (no cable to clutter the space up).

This keyboard is designed with anticipation for a very specific (but hopefully widely-avaliable) type-c board. You will have to modify the model if you do not have it. It lacks the resistors to make it work with a c-c wire, because I forgot them.

As a consequence, it means that the microcontroller is more protected from being plugged/unplugged and can be accessed easier for soldering/desoldering.

#### Alternatives to the RP2040
Alternatives I considered include the ATMEGA32A, Makey-makey, Arduino Pro Micro. Especially with the Pro Micro, there is support for some other firmware (though QMK seems the standard) and you can find more documentation. But they were costly by comparison, had less storage, and fewer pins. They all seemed equally easy to program, arguably the RP2040 easiest, as you just drag+drop the compiled firmare onto it. You could use any microcontroller that can pretend to be a USB HID device.

#### Why Wired?

This was my first keyboard. I decided batteries were for a future project.

But seriously - wireless would require more pins, more thought, and a battery. QMK isn't wireless-native (KMK is), and there are some exta-low-power modes etc. that would need to be thought about. Plus, the OLED would drain the battery quicker. The Pi Pico W has a Bluetooth radio that can be made to make it a keyboard. Look at other firmware thats wireless first if you want to pursue this (and to pick a supported microcontroller).

### 🔇 Making things quiet
I spent a not insiginficant amount of time on this.

There are some things you can do, such as:
* Use silent-ish switches. This probably makes the biggest differece. Lubed switches should help (also with the 'feel'). Silent switches will have dampeners in their shell and potentially at the bottom of the stem internally.
* Change keycap shape. I found this out by printing some other keycaps, and turns out the shape makes a big difference.
* Use o-rings. If you bottom out keys with force, this can help at the expense of the feel (becomes mushier and reduced key travel distance).
* Use hollow materials. The infill on the sides of the case/plate is 20%, so it means some sound is 'absorbed'. If it was solid, the sound would spread more evenely.

Things you can allegedaly do (I read about these but didn't try them):
* Add pillow fluff to the inside.
* Use rubber feet. This will reduce the vibrations passed to the desk at the expense of size. Plus the keyboard will be much gripper!
* Add a foam layer between the plate and the case/base. This was almost a thing, but I couldn't find any consistent foam standards or wanted to compormise on the structural integrity.
    * <sup><sub>Plus I was hoping this keyboard would be somewhat recyclable - mixing materials stops a keyboard from being recyclable. Plus the people sorting would have probably thrown away the keyboard parts in the recycling/sorting centre anyway as they don't look like PETG-recyclable... And I couldn't find much info about whether the PETG fillament is even recyclabe, given the potential additives?</sub></sup>




## 👨‍🔬Modelling the Keyboard

I used [Autodesk Fusion360](https://www.autodesk.com/products/fusion-360/personal) because I was familar with Autodesk Inventor (a similar tool) & it was free for personal use, alongside [OpenSCAD](https://openscad.org/) to use the keycap library, KeyV2

I wish I had used [OnShape](https://www.onshape.com/en/), or maybe even FreeCad (much better since the 1.0 release) as both are free and don't have stupid editable file limitations like Fusion360 and strange cloud integration in places.


### ✏Sketching out
First, I sketched out some thumbnails to get an idea of the rough shape and size, and where things may go, like the key placement, OLED, macro keys etc.

During this process, I decided I was happy with the clear PETG look. In retrospect, I would have liked it to be more colourful. I didn't mind seeing the plate either (usually a third layer is added which extends to the bottom of the switches to hide them somewhat).

I also thought about the size at this point by estimating some dimensions. Generally, I thought a 5mm border sufficient. I also knew there had to be extra strength added due to the lack of a dedicated plate.

### Making the layout
The layout was made using [Keyboard Layout Editor](https://www.keyboard-layout-editor.com/#/). While no longer actively developed and sometimes frustrating to use, it is the easiest to use tool I have found.

The layout is based off a Dell laptop keyboard, but with a few changes - namely no numpad and a wrap around layout.

The standard 'staggered' layout is only one of the options. There are various 'staggered' layouts to choose from. A grid layout (aka ortholinear) can be used instead.

### Generating the plate
The keyboard plate (aka the bit with the switch holes) was generated using [SwillLib Plate Builder](http://builder.swillkb.com/). This was definately the right option as making this CAD sketch manually would have been error prone and taken ages.

### 🪑CAD Modelling
I took the generated plate CAD drawing, then modified it to make the borders the correct size.

Subsiquently, I got to modelling the parts and creating a digital assembly.

This is where knowledge of CAD modelling practices and being aware of 3D printing limitations were handy. Here are some key ones:
* Think of the model as parts. Each part should be in a seperate file, later places into a digital assembly.
* Digital assemblies help avoid unnecessary prints. Especially as CAD models of common parts are avaliable online (e.g. Pi Pico, SSD1306)
* Dimensions should end in 2,4,6,8 to reflect the nozzle diameter and layer height (e.g. 12.02mm).
* If something is not a multiple of the layer height (0.12mm in my case) - it may not print correctly.
* Avoid overhangs or voids where supports will be needed. Removing them is annoying, the finish is rough, and causes unecessary material waste.
* Sense of scale can be difficult to visualise without being able to hold some components. Print them off, or have them avaiable to look at.
* Large parts warp, so split them.
* Certain areas are more prone to iteration, so split accordingly. That way if you decide the side of the keyboard is silly, avoid.
* Ensure your tolerance takes into account at least 0.5mm. This is both for an error in measurements, variance in parts, and 3D printer calibrations.
* Rounded edges on the layer axis (up/down) should be avoided, as they will be rough. If they cannot be avoided, a smaller nozzle, or provision for smoothing should be thought of. <sub>Smoothing can be carried out by varnishing, sanding, chemical abraison, or a combination of all three. Ordered  easiest to least approchable.</sub>

I deliberately avoided melt-in threaded inserts as they are (IMO) overpriced. The bolt screw mount was chosen as I figured I may want to tinker with wiring. A [plastic self-tapping screwhole](https://www.youtube.com/watch?v=HgEEtk85rAY) can be incorporated into the design instead, but will wear out if frequently used.



## 🖨Printing
The printing process took a long time, mostly because my printer was poorly calibrated and I played around too much with the settings trying to find perfect ones.

The printer I used was an Ender 3 Pro (no bed leveling when I made this - V1.1.4/8bit mainboard). Truly a no-frills printer.

### 💿Print Settings
A lot of these settings can be improved.
* CURA Slicer
* 0.4mm nozzle
* PETG (I used eSun Clear PETG - I used a no-label fillament for a first protype and it was terrible)
    * 230C print, 90C glass bed, with a hairspray coating to aid de/adhesion.
* 0.16mm 'dynamic' layer height (0.12-0.18mm)
* 20% gyroid inflill (gives it strength + interesting pattern)
* Brim for bed adhesion, 8mm width, also for inside of the plate
* 1.2mm walls

### ⚗Part Processing (sanding etc.)
I had to add the brim to the interior of the switch holes to ensure adhesion. Getting rid of them was a nightmare but it helped a lot. I used my snips to do the majority of the work. I could almost peel a lot of it away. I'm sure there's a slicer setting to make them peel easier somewhere.

The keycaps also used brims. I used nail polish to smooth some out, as dirt can get trapped in grooves.

I tried to avoid sanding too much in order to avoid creating too many microplastics.

Getting rid of the supports which filled the void for the type-c connect was a nightmare. Turns out it should have been printed as two seperate pieces. The one layer of plastic that was holding it together almost snapped. the Type-C connect became structural.



## 🧰Assembly
Overall, the soldering took the longest, followed by getting the stabilisers right.

The keyboard is effectively two piece. The body is screwed together with the bottom plate.

The body and bottom plate are printed off in two parts, therefore have to be glued together.

The body then requires for screw mounts to be glued in (with hex bolts glued in as well).

The type-c connect has to be glued in as well.

### 〰Wiring/Soldering
I highly recommend using enamelled single core wire (i.e. single strand). The enamel is easy enough to burn off where needed. Do not use multi-core wire like I did.

First, each of the keys had to have a diode soldered to one of the pins.

Next, I suggest using a single wire for each row/column and burning off the bits of the enamel where the keys connect.

Finally (for the keys at least), I soldered the each row/col to the RP2040. Each wire should be thin enough to fit through the holes as it makes it much easier to solder them.

I had to check for shorts between each of the rows/cols using a multimeter and fix them using the white electrical tape.

The USB C board was wired to the micro USB connector via enamelled wire, as was the OLED.

The rotary encoder encoding pins were soldered in to the micro controller, however the switch was soldered into the keyboard matrix, requiring a diode.

For the rows to RP2040, OLED and rotary encoders I left some extra wire to allow for the RP2040 to be lifted out - but not so much to where it would take up unnecessary space.

Lead-free solder was used, which is a little more challenging to work with - but less likely to accidentally contaminate something with lead.

The Pinecil was an excellent soldering iron and had enough heating power @ 45w.

### 🚅Key Stabilisers
The space, return, and backspace keys all required quite a lot of thought, as they required a stabiliser wire. To make your own, you need to measure the distance between the far ends of the stabilisers once they are in the board, then measure 11mm, and then about 5mm (this distance doesn't matter too much) and bend it in place.

For the space key stabiliser wire, I went through 4 different types. Turns out, just get the steel wire as jewellery wire is not strong enough (turns out the plated ones are not steel-core). You can adapt the key insert for the Costar to make it work properly. I heard that orthodontic wire is steel wire and can be bought cheaply.

### Uploading QMK / Luna
I chose [QMK](https://qmk.fm/) as Luna (the keyboard pet) was supported by it. I am also familar with C and C++. [ZMK](https://zmk.dev/) or [KMK](https://github.com/KMKfw/kmk_firmware) are Python based, and can used instead.

First, I needed to setup the QMK development envrionment. QMK provides an MSYS installer for this. Then, you need to fork your own repo of QMK and create the mappings etc. in a config file. Finally, the firmware can be built and uploaded by dragging the file onto the RP2040.

[My firmware fork](https://github.com/giodestone/qmk_firmware/tree/master/keyboards/giodestone/hart) contains the code for my firmware.

The biggest challenges were figuring out how I wired it together, and making Luna work for the OLED display.

The easiest method is to copy over a similar keyboard and start messing with it until it works AND [follow one of these guides](https://thomasbaart.nl/category/mechanical-keyboards/firmware/qmk/) (especially or getting USB VIDs).

#### Luna
Luna was designed for a 32x128 display. I have a 128x64 display. I had to rewrite the rendering code to make it work correcly as otherwise Luna was in four segments. This involved a lot of trial end error and putting up with the rather strange way sprites are stored and rendered. I did break the jumping function however. I also had an issue where I thought my code caused memory corruption, but it turns out I had some dodgy soldering and potentially incorrect sizes.

There is also some code for 'honk' a keyboard pet I was working on... I may finish it some day in the future.

## 🎓Learnings / Reflection

### Parts
Overall, the externally bought parts were great choices and desired parts were good enough.

#### Casing
I wish I had split up the casing a little more. I could have avoided the need for supports in the type-c, OLED, and rotary encoder enclosures. This would have resulted in a better finish, despite a greater requirement to assemble. Overall, the plastic wasted for supports was low, but could have been none.

I could have improved the structural integrity and assembly experience by adding indents/grooves to the body and bottom plate. This would have improved the strength by making the print rely on mechanical contact, rather than adhesive strength. Not that the keyboard is fragile!

The space left on the bottom of the keyboard was just enough after resoldering parts of the keyboard with lower gauge enamlelled copper wire - as opposed to some generic (multi-core) wire I got.

I wished I had placed the screw mounts in the corners, as they make some wires difficult to inspect. I thought it would require increasing the size of the case too much. I was wrong.

### RP2040

The RP2040 has two I2C controllers (I2C0 and I2C1), avaliable only on certain pins! Moreover, it appearts the pinout is a lie, and pins 1, 2 (which claim I2C support), did not work for me. This is why the OLED display is on pins 4,5. I didn't try disabling UART, which may have been the issue.

Apart from this, it was an excellent choice due to native QMK support and ease of flashing new firmware.

#### USB C Breakout Board
I think it was a good idea. I didn't have to glue or screw the microcontroller in place to fix solder connections. I will likely continue this for future hand-built keyboards.

Due to my oversight, its missing the resistors required to make it work with a USB C to C cable.

#### OLED Display/SSD1306
Overall, I think it was the right choice as it was cheap and simple. You can get bi-colour OLED displays, and even colour ones - but you would be far more space microcontroller space concerned if you had to deal with a full-RGB palette (you can definitely cut it down by using a fixed-palette).

I want to do more with it!

#### Volume Knob/EC11
It was the right choice. The EC11 is natively supported by QMK. I was trying to test it before assembling and I couldn't get an Arduino library to work for some reason.

### Keys
The key switch choice was very good - they feel very satisfying to type on and smoother than rubber-dome (aka generic keyboard) or scissor (aka laptop).

The keycaps take getting used to. I think I should have made them smaller (their key top size matches the laptop one) - but the bottom tapers out too quickly making it easy to mistype. The keycaps either have to be bevelled or their top be higher than the next key when depressed to avoid the edge of your finger from pressing the next key. Fortunately, it is very easy to reprint keycaps and iteratively design due to low resource use and fast printing times.

#### Stabalisers
Bending the wires was a pain. Getting the distances more so. Getting the wires flat even more.

I wish I had used one for the caps lock and right shift, as it flexes more than I would like it to.