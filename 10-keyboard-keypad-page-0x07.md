# 10 Keyboard/Keypad Page (0x07)

- This section is the Usage Page for key codes to be used in implementing a USB keyboard.

- A Boot Keyboard (84-, 101- or 104-key) should at a minimum support all associated usage codes as indicated in the *Boot* column below.

<br>

- The usage type of all key codes is Selectors (Sel), except for the modifier keys Keyboard Left Control (0x224) to Keyboard Right GUI (0x231) which are Dynamic Flags (DV).

> ##### Note
>
> - A general note on Usages and languages:
>
>   - Due to the variation of keyboards from language to language, it is not feasible to specify exact key mappings for every language.

|Usage ID|Usage Name|Usage Type|PC-AT|Unix|Boot|
|-|-|-|-|-|-|
|00-00|*Reserved*|||||
|...|||||||
|04|Keyboard a and A|Sel|✓|✓|✓|4/101/104|
|05|Keyboard b and B|Sel|✓|✓|✓|4/101/104|
|06|Keyboard c and C|Sel|✓|✓|✓|4/101/104|
|...|||||||
|1D|Keyboard z and Z|Sel|✓|✓|✓|4/101/104|
|...|||||||
|2A|Keyboard DELETE (Backspace)|Sel|✓|✓|✓|4/101/104|
|...|||||||
|2C|Keyboard Spacebar|Sel|✓|✓|✓|4/101/104|
|...|||||||
|E0|Keyboard LeftControl|DV|✓|✓|✓|4/101/104|
|E1|Keyboard LeftShift|DV|✓|✓|✓|4/101/104|
|E2|Keyboard LeftAlt|DV|✓|✓|✓|4/101/104|
|E3|Keyboard Left GUI|DV|✓|✓|✓|104|
|E4|Keyboard RightControl|DV|✓|✓|✓|101/104|
|E5|Keyboard RightShift|DV|✓|✓|✓|4/101/104|
|E6|Keyboard RightAlt|DV|✓|✓|✓|101/104|
|E7|Keyboard Right GUI|DV|✓|✓|✓|104|
|E8-FFFF|*Reserved*|||||||
