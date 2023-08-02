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
There are two possible causes:  
* The ATRO file was created for a version of the engine that uses a different ATRO format. If that's the case use the version that created the ATRO file to export a JSON equivalent and convert it back to ATRO on your version.
* String values of the source JSON cannot go above 255 in length and will result in a corrupt ATRO file. In that case there's no fixing this. Discard the ATRO file and use JSON chart files instead (here's praying for your sake that you have a backup🙏).
