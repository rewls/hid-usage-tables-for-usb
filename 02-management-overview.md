# 2 Management Overview

- This document provides list of Usages and their descriptions that significantly extend the list of Usages provided in the HID Specification.

- A HID Usage communicates the intended function or meaning of a particular control.

- Usages provide a description of the data items in a HID device's Input, Output, and Feature reports.

- The existence of a defined Usage does not guarantee that system or application software will recognize or utilize the data item.

- Although Usages can be very powerful, there is a potential for misuse.

- The detail provided in this document will help minimize the misuse or misinterpretation of Usages when they are applied by a device developer.

<br>

- Usages have been organized into pages of related controls.

- Each Usage has a Usage ID, Usage name and a detailed description.

- The Usage names are mnemonics, not definitions.

- To avoid misleading interpretations based on the Usage name, it is very important that a developer review a Usage's description in detail to ensure that it properly identifies the purpose of the control or device that the Usage is attached to.

<br>

- In theory, a Usage can be attached to any type of HID control, variable, array, collection, and so forth.

- In reality, Usages only make sense when they are attached to particular controls and used in certain ways.

- A relatively small set of Usage types have been defined to help the application software developer better understand what to expect when a particular Usage is found.

- Each Usage has a Usage type associated with it.

- The Usage type identifies the item types, flag settings and bit fields organizations that are found with a particular Usage.

<br>

- Usages can also identify functional devices as a whole, thus providing an easy method for an application to identify devices that provide functions of interest.

- Such Usages are found attached to application collections that are wrapped around all the items that describe a particular functional device, or a particular function in a complex device.

- Generally an application will query the HID driver for all application collection Usages that it knows pertain to it.

- For example, a gaming device driver might look for Joystick and Game Pad Usages, while a system mouse driver might look for Mouse, Digitizer Tablet and Touch Screen Usages.

<br>

- As a general rule, the Usages selected by a device developer should be specific enough to dissuade inappropriate use by applications while remaining general enough to allow applications to take advantage of device features if they can.

- If uncertain, favor the more general Usage to encourage broader application support for your device.

- An alternative is to use delimiters to define multiple Usage associated with a single control or a device.

<br>

- Some Usage pages that are in the HID Specification are also found in this documentation.

- They are included here because either additional text has been provided to clarify how the Usages are to be used, new Usages have been added to the page, or both.

- No changes have been made to the Usage values assigned in the HID Specification.
