# NXDK-Menu-Example
An example of how you would create a menu with controller support using [NXDK](https://github.com/XboxDev/nxdk)

You can use this as a base or reference for your own projects!

This used the [sdl_gamecontroller sample](https://github.com/XboxDev/nxdk/tree/master/samples/sdl_gamecontroller) as a base!


## Prerequisites
This requires the [NXDK](https://github.com/XboxDev/nxdk) tool chain to compile to .XBE

You will also need the following tools:
- GNU make
- [clang](http://clang.llvm.org/)
- [GNU bison](https://www.gnu.org/software/bison/) and [flex](http://flex.sourceforge.net/)
- [lld](http://lld.llvm.org/)
- [Git](http://git-scm.com/)
- [CMake](https://cmake.org/)

OS-specific instructions for installing these prerequisites can be found in the [Wiki](https://github.com/XboxDev/nxdk/wiki/Install-the-Prerequisites)


## Info
This menu serves as a proof of concept on how you could create a menu with controller support. The menu comes with a main menu and 3 sub menus.

This is the menu break down:

Main menu (Menu 1)
- Option 1 ---------------------- Pressing A on this option will load Menu 2
- Option 2 ---------------------- Pressing A on this option will load Menu 3
- Option 3 ---------------------- Pressing A on this option will load Menu 4
- Quit ---------------------------- Pressing A on this option will Quit and return to launcher.

Menu 2
- Option 4
- Option 5
- Option 6
- Back ---------------------------- Pressing A on this option will return to Main Menu (Menu 1)

Menu 3
- Option 7
- Option 8
- Option 9
- Option 10
- Back ---------------------------- Pressing A on this option will return to Main Menu (Menu 1)

Menu 4
- Option 11
- Option 12
- Back ---------------------------- Pressing A on this option will return to Main Menu (Menu 1)

Pressing B anywhere in any of the menus will return to the Main Menu (Menu 1)

Options 4,5,6,7,8,9,10,11,12 don't have any functions as they serve to provide an example of sub menus. You can easily program those options to have functionality. You can also add and remove menus and menu options, just read the code and add or remove menus or menu options based on how the other menus and menu options are programmed; it's pretty straight forward!
