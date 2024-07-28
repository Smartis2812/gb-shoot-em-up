# GameBoy 'Shoot-em-up' Clone written in Assembly

Village Hero

Using [RGBDS](https://rgbds.gbdev.io/), base on the amazing second tutorial from [gbdev.io](https://gbdev.io/gb-asm-tutorial/part3/getting-started.html).

## How to build

```bash
make
```

## Folder structure


- libs - Two assembly files for input and sprites are located here.
- src
    - generated - the results of RGBGFX are stored here. *
    - resources - Here exist some PNGs and Aseprite files for usage with RGBGFX
    - main - All assembly files are located here, or in subfolders
         - states
             - gameplay - for gameplay related files
                 - objects - for gameplay objects like the player, bullets, and enemies
                     - collision - for collision among objects
             - story - for our story state’s related files
             - title-screen - for our title screen’s related files
         - utils - Extra functions includes to assist with development
             - macros
 - dist - The final ROM file will be created here. *
 - obj - Intermediate files from the compile process. *
 - Makefile - used to create the final ROM file and intermediate files
