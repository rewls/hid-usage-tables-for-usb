# 1 Introduction

- Usages are part of the HID Report descriptor and supply an application developer with information about what a control is actually measuring or reporting.

- In addition, a Usage tag can be used to indicate the vendor's suggested use for a specific control or group of controls.

- While most of the items within a Report descriptor describe the format of the data the Usage tag define what should be done with the data.

- This feature allows a vendor to ensure that the user sees consistent function assignments to controls across applications.

- It is also the key feature within HID Report descriptors that allows system or application software to know the meaning of data items, or collections of data items, so the data items can be correctly interpreted or routed to the system or application software that consumes them.

## Purpose

- This document defines constants that can be interpreted by an application to identify the purpose and meaning of a data field in a HID report.

<br>

- Usages are also used to define the meaning of groups of related data items.

- This is accomplished by the hierarchical assignment of Usage information to collections.

- Usages identify the purpose of a collection and the items it contains.

- Each Input, Output, Feature, and/or Collection data item within a Collection item can be assigned a purpose with its own Usage item.

- Usages assigned to a collection apply to the items within the collection.

<br>

- In some cases a Usage applied to a collection can redefine the meaning of the Usages it contains.

<br>

- Usages are also used to specify the meaning of each element within an Array data item.

## Terms and Abbreviations

### Application

- A software program that consumes the data generated by the HID device Input reports, or that controls the HID device through Feature or Output reports.

### Array Field

- The bit field created by an Input, Output, or Feature main item which is declared as an Array.

- An array field contains the index of a Usage, not the Usage value.

### Control

- A control is used to operate or regulate a particular aspect of a device.

- In this document a control refers broadly to the physical entity on the device that the Usage identifies.

### Field

- The Input, Output, and Feature main items create a bit field in a report.

- The Report Size determines the field's width and the associated Usage determines the field's purpose.

- The offset of a field in a report is determined by the fields that are declared before it.

### Pad

- If a field is marked as a constant and there is no Usage associated with it, the field will be treated as pad bits and ignored by host software.

### Usage

- Defines the purpose or meaning of an item.