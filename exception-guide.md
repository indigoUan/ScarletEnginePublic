# Scarlet Engine Exception Guide
This file contains some exceptions you might meet.

## [file_contents,(path)]
This occurs when the file in (path) is either being used and cannot be overwritten, or id doesn't exist and cannot be opened.

## [lime.utils.Assets]
Similar to `file_content`. The body of the exception tells you what's wrong.

## Null Object Reference
The last line of the "Calls" list tries to use a `null` object.  
It might be trying to use the object before it's initialized, or the object is simply `null` for whatever reason.

## Null Function Reference
The last line of the "Calls" list tries to use a null function. See the [Null Object Reference](https://github.com/indigoUan/ScarletEnginePublic/blob/main/exception-guide.md#null-object-reference) entry.

## Chart Reading Error: OutsideBounds
There's no fixing this (sorry!). Discard the chart file and use JSON chart files instead (here's praying for your sake that you have a backup🙏).
