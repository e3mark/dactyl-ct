# Dactyl CT - The Cute Thumb Dactyl Keyboard

Check the guide:
> ### [How to Make a Dactyl Manuform Keyboard](guide/index.md)

## 3D Models
A fork of [Dactyl-Mini-Thumb](https://github.com/aleung/mini-thumb-dactyl-keyboard)

The Dactyl-Mini-Thumb is a fork of [Dactyl-ManuForm](https://github.com/tshort/dactyl-keyboard), a parameterized, split-hand, concave, columnar, ergonomic keyboard.

The Dactyl-Manuform is a fork of the [Dactyl](https://github.com/adereth/dactyl-keyboard) with the thumb cluster from [ManuForm](https://github.com/jeffgran/ManuForm).

### Cute-Thumb-Dactyl

File: [`mini_thumb_dactyl.clj`](src/dactyl_keyboard/mini_thumb_dactyl.clj)

I'm comfortable with the concave curve of Dactyl-ManuForm keyboard. But I don't need so many thumb keys. This version reduces thumb keys to three on each hand.

![](resources/mini-thumb-dactyl.jpg)

### Generating a Design
**Generating the design**
* Run `lein repl`
* Load the file `(load-file "src/dactyl_keyboard/dactyl-ct.clj")` 
* This will regenerate the `things/*.scad` files
* Use OpenSCAD to open a `.scad` file.
* Make changes to design, repeat `load-file`, OpenSCAD will watch for changes and rerender.
* When done, use OpenSCAD to export STL files

### Printing
Fix the model before printing if it has defects. I use [Netfabb Free](https://github.com/3DprintFIT/netfabb-basic-download) to and it's automatically done.

### Wiring & Firmware

Please read the guide: [How to Make a Dactyl Manuform Keyboard](./guide/index.md)

## License

Copyright © 2015-2017 Matthew Adereth, Tom Short and Leo Liang.

The source code for generating the models (everything excluding the [things/](things/), [guide/](guide/) and [resources/](resources/) directories is distributed under the [GNU AFFERO GENERAL PUBLIC LICENSE Version 3](LICENSE).  The generated models and PCB designs are distributed under the [Creative Commons Attribution-NonCommercial-ShareAlike License Version 3.0](LICENSE-models).
