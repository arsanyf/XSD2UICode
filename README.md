#XSD2Code
A work in progress. This piece of code aims to automate the process of reading the XML schema file(s), most likely to be big in volume and outputs some C# code for a data entry form. Aiming to be extensible to any UI, whether it's web, WPF or whatever.

###refactoredXSDReader.tt
This T4 reads the schema to output a code chunk containing the UI needed for a data entry form. This is where the XSD reading logic resides. Note: As this is still a work in progress, the chunk generated would need some post editing.

###UIWriter.ttinclude
Include file where all the UI code generation logic resides. Currently it generates WPF code, in order to extend it simply implement the interface and plug it into the first file.
