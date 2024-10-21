# ckau-book-custom-systems

<p>
<img align="right" width="200px" src="https://i.imgur.com/eCZPBDE.png">
Emulationstation Customized ES Systems for Batocera and Retrobat.<br/>
<br/>
</p>
<p>
      <a href="https://img.shields.io/github/stars/g-spawnPL/batocera-custom-es_systems" alt="stars">
        <img src="https://img.shields.io/github/stars/g-spawnPL/batocera-custom-es_systems" /></a>
      <a href="https://img.shields.io/github/forks/g-spawnPL/batocera-custom-es_systems" alt="Forks">
        <img src="https://img.shields.io/github/forks/g-spawnPL/batocera-custom-es_systems" /></a>
      <a href="https://img.shields.io/github/issues/g-spawnPL/batocera-custom-es_systems" alt="Issues">
        <img src="https://img.shields.io/github/issues/g-spawnPL/batocera-custom-es_systems" /></a>
      <a href="https://img.shields.io/github/issues-closed/g-spawnPL/batocera-custom-es_systems" alt="Issues Closed">
        <img src="https://img.shields.io/github/issues-closed/g-spawnPL/batocera-custom-es_systems" /></a>
      <a href="https://img.shields.io/github/issues-pr-closed/g-spawnPL/batocera-custom-es_systems" alt="Closed PR">
        <img src="https://img.shields.io/github/issues-pr-closed/g-spawnPL/batocera-custom-es_systems" /></a>
</p>

## Purpose

EmulationStation displays systems based on a file called es_systems.cfg. In other distributions, this is typically the only file. However, in Batocera FIXME and higher, and in Retrobat 5 and higher, one or more `es_systems_<custom_name>.cfg` files can be used as an overlay to the original `/usr/share/emulationstation/es_systems.cfg` file.

This repository contains .cfg files for adding additional systems to your Batocera or Retrobat installation, all supported by [Ckau Book](https://github.com/CkauNui/ckau-book) theme.

You must use a unique `<custom_name>` field when adding a new system if you wish to keep the old one in addition. However, if using duplicate shortnames is a necessity and you still want the new and old system to exist simultaneously, you can also put both systems in a single CFG file.

Once implemented in your system, you can use our Emulationstation Theme: https://github.com/CkauNui/ckau-book

## How to install new systems

### Batocera <img align="left" width="50px" src="https://batocera.org/images/head/logo-tri.png">

Additional .cfg files are located in two directories of this repository:

`/Batocera/Raspberry Pi 4 (base)/system`
`/Batocera/x86 64bit (additional)/system`

while .cfg files in `Raspberry Pi 4 (base)` can be used in any Batocera installation, the ones in `x86 64bit (additional)` can be only added in a x86 PC Batocera environment.

To add the new systems, the desired .cfg files must be copied in the same directory as `es_systems.cfg`, which for Batocera is

`/usr/share/emulationstation/`

When done, for each added system you should create the proper `/roms/<system_name>` directory and put your roms into it.
Please check the right name to create, following the examples located in `/Batocera/Raspberry Pi 4 (base)/roms` or `/Batocera/x86 64bit (additional)/roms` directories of this repository.

You'll also find a `_info.txt` file that explains which extensions are allowed for each system.
For some systems, there may be also the need to install additional emulators (check the same `_info.txt` file for instructions).

A newly added system, if there is at least one rom file, will automatically be recognized by Batocera at the next boot.

## Credits

- CFG autor:
  - g-spawn and RGS Team ([@g-spawnPL](https://github.com/g-spawnPL)), [@Lendersmark](https://github.com/Lendersmark)
  - Thanks to [@CkauNui](https://github.com/CkauNui) and [@n2qz](https://github.com/n2qz) for helping with the project
- Based on:
  - Batocera system wiki (https://wiki.batocera.org/emulationstation:customize_systems)
  - Retrobat system wiki (https://wiki.retrobat.org/systems-and-emulators/supported-game-systems)

## License

- ALLOWED
  - Share and duplicate as it is
  - Edit, alter, change it
- REQUIREMENTS:
  - Attribution, give credit to the creator
  - Indicate changes to it
  - Publish the changes under the same license
- PROHIBITED:
  - Commercial distribution

### Copyrights / Sources
- Each brand of hardware and software here represented as a tribute.<br/>
- All logos, trademarks and photos are copyright of their respective owners.<br/>
- es_systems_switch.cfg generate after install nintendo switch emulator from project: https://github.com/ordovice/batocera-switch.<br/>
- es_systems_makecode.cfg generate after install MakeCode Arcade emulator from project: https://github.com/Vegz78/McAirpos.<br/>

### Logo Notice

The used logos and trademarks are copyright of their respective owners.
  
Shield: [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
