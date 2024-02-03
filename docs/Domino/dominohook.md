# Dominohook

[Dominohook](https://github.com/khang06/dominohook) is a hook DLL for Domino that uses the [QuickHook](https://github.com/CPunch/QuickHook) library by CPunch.

Dominohook adds new features like replaced zoom handling functions, string patching framework with translated strings and some other stuff.

> TODO: Add images

## Installing Dominohook

!!! warning "Only tested with english translation"

    Dominohook has been tested with the english translation, the japanese versions haven't been tested for this guide. If you get dominohook working with the japanese 32-bit version [submit an issue to the github repository](https://github.com/OvertureMIDI/Guides/issues).

To install Dominohook, download the latest release [here](https://github.com/khang06/dominohook/releases/download/3.0.1/dominohook.dll), then install [Stud_PE](https://www.cgsoftlabs.ro/studpe.html).

After you installed the necessary files, open Stud_PE and drag your `Domino.exe` into the window.
Next, click the "Functions" tab, right click the dll list, add new import and select your `dominohook.exe` file, add "dummyexport" to the list and copy the dll file next to your `Domino.exe` file.

Now, launch domino and it should launch fine, or crash. If it crashes, either try again or [submit an issue explaining your problem](https://github.com/OvertureMIDI/Guides/issues) so that we can help and improve this guide.
