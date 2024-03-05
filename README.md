# Acrobat Custom Info Panels
Custom Info Panels for Adobe Acrobat that display XMP metadata information in more friendly ways. This is poorly documented in Adobe's "XMP Custom Panels", dated October 2003, which I can no longer find on the Adobe website but which still works in Acrobat. Here is [a link to the documentation](http://metadatadeluxe.pbworks.com/f/XMP_CustomPanels.pdf).

Copy these files to the following locations:

Mac OS X:
- `{Root Volume}/Library/Application Support/Adobe/XMP/Custom File Info Panels` - for all users on the machine
- `{Home Directory}/Library/Application Support/Adobe/XMP/Custom File Info Panels` - for each user

Windows:
- `C:\Program Files\Common Files\Adobe\XMP\Custom File Info Panels` - for all users on the machine
- `C:\Documents and Settings\<user>\Application Data\Adobe\XMP\Custom File Info Panels` - for each user

## Debugging and Issues
Note that you can edit these files while Acrobat is running - just click the "Additional Metadata" button on the File Properties dialog to reload all custom panels each time. As far as I know, there is no easy way to debug beyond if your panel is not listed then it has an issue.

- I've never been able to get the `picture` feature working as I don't know how to reference the asset (file? URL? formats?)
- I struggle to understand how to use XMP `bags` (such as needed by PDF Declarations) since it seems you can only use fixed (hard-coded) XMP paths
- I don't believe there is any way to easily comment out stuff (I normally move blocks of code to the XML portion and then use XML comments `<!-- ... -->

# ISO Standards
Displays the conformance data related to PDF subset ISO standards for PDF/A, PDF/UA, PDF/X, PDF/VT, PDF/E and PDF/VCR. PDF/R does not use any custom XMP metadata.
Note that the early PDF/X standards did not use XMP metadata but only the Document Information dictionary. 

# PDF Declarations
The PDF Association defines extensions to XMP metadata that allow documents to declare conformance to external industry and third-party specifications such as WCAG and HIPAA. See https://pdfa.org/declarations. 
