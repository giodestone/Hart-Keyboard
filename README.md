# Hart Keyboard

![Hart keyboard on a white background](https://raw.githubusercontent.com/giodestone/Hart-Keyboard/refs/heads/dev/Images/Image2.jpg)

Hart is a 80% ISO layout 3D-Printable, hand-soldered keyboard based on the RP2040 platform (Raspberry Pi Pico 1). It is supposed to be cheap, achievable, and usable.

This is my first keyboard like this, so it contains a lot of newbie things. I suggest using this a reference for your own keyboard, rather than trying to 3D print it (but if you do - please open an issue/pull-request with your build pictures!).

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

## Bill of Materials (BoM)
This keyboard should cost £70-100 to make.

* c. 500g of filament (actual requirement is much lower)
* 90x switches
* 90x keycaps, some with Cherry-style or Costar style stabalisers.
    * 1x 6.25u key (stabalised)
    * 1x 2u key (stabalised)
    * 1x ISO enter key (stabalised)
    * 2x 1.75u
    * 2x 1.5u
    * 2x 1.25u
    * 81x 1u
* 90x diodes
* 1x SSD1306 OLED
* 1x EC11 Rotary Encoder
* 1x RP2040 (micro USB)
* 1x USB C breakout board ([for it to work with a USB C to C cable, some resistors are needed](https://www.youtube.com/watch?v=X6A6_k5L0_g))
* 1x Micro usb spare cable (for getting between RP2040 and breakout board)
* 1x Adhesive (e.g. superglue)
* 2x 2u Costar stabaliser wires (or 2x paperclips and necessary tools to manipulate them)
* 1x 6.25u Costar stabaliser wire (or gauge 20 steel wire + necessary tools)
* for the back (subject to change)
    * 7x M3 muts
    * 7x M3x8 bolts or screws

## Tools
* Access to a calibrated, reliable 3D printer.
    * + related tools for 3D print refinement such as a file/sandpaper.
* 1x flush cutters
* 1x tuler
* 2x needlenose pliers for stabaliser wire creation (or 1x needlenose plier, 1x wire straightner/double nylon jaw)
* 1x soldering iron with your preferred tip (I used a Pinecil - highly reccomend)
* 1x rosin-core lead-free solder spool
* 1x spool of enamelled wire
* 1x roll of electrical tape (I used white)


## Design Choices
First, I had to establish some goals, these ended up being:

1. Usable
2. Achievable
3. Cheap

After thinking about it some more, the keyboard had to:
* have a familar/standard-ish layout.
* be compatibile with a computer running Windows.
* be quiet enough.
* be novel enough so I remain interested in finish it.
* use achievable techniques with the tools I have.
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
- 🔧 [Keyboard Layout Editor](http://www.keyboard-layout-editor.com/#/)
- 🔧 [Keyboard Layout to STL Generator](https://kbd.news/Keyboard-layout-STL-generator-1259.html)
- 🔧 [Keyboard Layout to CAD Drawings](http://builder.swillkb.com/)
    - [Alternative](https://github.com/swill/kad)
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

### 🎪 Gimmicks (Rotary Encoder, Display)

I saw a video of Luna, a companion keyboard pet. It responds to your typing. I really liked it. Plus I always found the indicator LEDs ugly.

I had a keyboard in the past with a scroll wheel for volume adjustment. I really liked it, but I thought it felt cheap and looked bad (though arguably more ergonomic). I also wanted the volume controller to act as media controls.


### 🎹 Keys

#### Keycaps
The keycaps were flat as they print well, and I like the aestetis and feel of flat keycaps 
(that's what I'm used to from the keyboard).

They were generated using the [Key V2 Library](https://github.com/rsheldiii/KeyV2), and tweaked using OpenSCAD. Note you need the nightly version, and you need to look through the issues if you want a fix for a stem generation easy.

You can just buy the keycaps, but make sure you have a compatible spacebar.

#### Switches
There are a multitude of switch formats to pick from. Cherry are the most prevelant so I went with them. I would have picked low profile, if they weren't both out of stock and overpriced - unless I wanted the ones with a Choc-style stem, which the keycap generation library did not support (and at the time of writing, still doesn't).

#### Stabalisers
Stabalisers are the things that stop the larger keys (space, enter, backspace, right-shift) from wobbling. 

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
* USB OTG device mode (so the Pi can pretend to be an input device)

<details>
<summary>Expand for Pico Pinout Image</summary>
![Pico Pinout Image](https://www.raspberrypi.com/documentation/microcontrollers/images/pico-pinout.svg)
</details>
[Pico Pinout Website](https://pico.pinout.xyz/)

The Pi Pico has 25 usable GPIO pins (26 if you count the one used for the built-in LED). This means it has enough for the matrix and rotary encoder (which uses GPIO pins). It has 2 I2C controllers (IC20 and IC21), making it suitable for the I2C based SSD1306 display. The RP2040 I got was the reference one. It had 16MB of 'storage' and 264KB of RAM (there are the variants that have as much as 64MB of 'storage') - enough for storing plenty of imaes. Two community-based keyboard firmwares support the RP2040: QMK (C-based) and KMK (Python-based). The RP2040 can also 'pretend' to be a USB keyboard. Finally, the price was good - about £4. Therefore, the RP2040 was chosen.

The RP2040 was not as well established when this keyboard was spec'd out (late 2022). But it appered that everything worked as intended.

#### Type C Port
I wanted for the keyboard to have a type-c port as it allows for swapping out of the wire, and easier packing away (no cable to clutter the space up).

This keyboard is designed with anticipation for a very specific (but hopefully widely-avaliable) type-c board. You will have to modify the model if you do not have it. It lacks the resistors to make it work with a c-c wire, because I forgot them.

As a consequence, it means that the microcontroller is more protected from being plugged/unplugged and can be accessed easier for soldering/desoldering.

#### Alternatives to the RP2040
Alternatives I considered include the ATMEGA32A, Makey-makey, Arduino Pro Micro. Especially with the Pro Micro, there is support for some other firmware (though QMK seems the standard) and you can find more documentation. But they were costly by comparison, had less storage, and fewer pins. They all seemed equally easy to program, arguably the RP2040 easiest, as you just drag+drop the compiled firmare onto it. You could use any microcontroller that can pretend to be a USB device.

#### Why Wired?

This was my first keyboard. I decided that's for the future.

But seriously - wireless would require more pins, more thought, and a battery. QMK isn't wireless-native, and there are some exta-low-power modes etc. that would need to be thought about. Plus, the OLED would drain the battery quicker. The Pi Pico W has a Bluetooth radio that can be made to make it a keyboard. Look at other firmware thats wireless first if you want to pursue this (and to pick a supported microcontroller).

### 🔇 Making things quiet
I spent a not insiginficant amount of time on this.

There are some things you can do, such as:
* Use silent-ish switches. This probably makes the biggest differece.
* Change keycap shape. I found this out by printing some other keycaps, and turns out the shape makes a big difference.
* Use o-rings. If you bottom out keys with force, this can help at the expense of the feel (becomes mushier and reduced key travel distance).
* Use hollow materials. The infill on the sides of the case/plate is 20%, so it means some sound is 'absorbed'. If it was solid, the sound would spread more evenely.

Things you can allegedaly do (I read about these but didn't try them):
* Add pillow fluff to the inside.
* Use rubber feet. This will reduce the vibrations passed to the desk at the expense of size. Plus the keyboard will be much gripper!
* Add a foam layer between the plate and the case/base. This was almost a thing, but I couldn't find any consistent foam standards or wanted to compormise on the structural integrity.
    * <sup><sub>Plus I was hoping this keyboard would be somewhat recyclable - mixing materials stops a keyboard from being recyclable. Plus the people sorting would have probably thrown away the keyboard parts in the recycling/sorting centre anyway as they don't look like PETG-recyclable... And is 3D printable PETG even officially recyclabe, with the potential additives?</sub></sup>




## Modelling the Keyboard

I used [Autodesk Fusion360](https://www.autodesk.com/products/fusion-360/personal) because I was familar with Autodesk Inventor (a similar tool) & it was free for personal use, alongside [OpenSCAD](https://openscad.org/) due to the parametric key library that needed it.

I wish I had used [OnShape](https://www.onshape.com/en/), or maybe even FreeCad as both are free and don't have stupid editable file limiations like Fusion360, can accidentally generate .stl files through the cloud (why?).

### Process
This is the rough process. I thought about it a lot before.

1. Settle on design. I sketched out a rough idea.
2. Make layout in this tool.
3. Put the layout from the above tool into...


### Sketching out






## Assembly

### Key Stabalisers
The space, return, and required quite a lot of thought. To make your own, you need to measure the distance between the far ends of the stabalisers once they are in the board, then measure 11mm, and then about 5mm (this distance doesn't matter too much) and bend it in place.

For the space key stabaliser wire, I went through 4 different types. Turns out, just get the steel wire as jewlery wire is not strong enough (turns out the plated ones are not steel-core). You can adapt the key insert for the costar to make it work properly.



## Learnings / Reflection

### RP2040

The RP2040 has two I2C controllers (I2C0 and I2C1), avaliable only on certain pins! Moreover, it appearts the pinout is a lie, and pins 1, 2 (which claim I2C support), did not work for me. This is why the OLED display is on pins 4,5. I didn't try disabling UART, which may have been the issue.

#### USB C Breakout Board
I think it was a good idea. I didn't have to glue or screw the microcontroller in place to fix solder connections. I will likely continue this for future hand-built keyboards.

Due to my oversight, its missing the resistors required to make it work with a USB C to C cable.


### Keys

#### Stabalisers
Bending the wires was a pain. Getting the distances more so. Getting the wires flat even more.

I wish I had used one for the caps lock, as it bends more than I would like it to.