# Acrobat Custom Info Panels
Custom Info Panels for Adobe Acrobat that display XMP metadata information in more friendly ways.

Copy these files to the following locations:

Mac OS X:
- `{Root Volume}/Library/Application Support/Adobe/XMP/Custom File Info Panels` - for all users on the machine
- `{Home Directory}/Library/Application Support/Adobe/XMP/Custom File Info Panels` - for each user

Windows:
- `C:\Program Files\Common Files\Adobe\XMP\Custom File Info Panels` - for all users on the machine
- `C:\Documents and Settings\<user>\Application Data\Adobe\XMP\Custom File Info Panels` - for each user

Note that you can edit these files while Acrobat is running - just click the "Additional Metadata" button on the File Properties dialog to reload each time. As far as I know there is no easy way to debug beyond if your panel is not listed it has an issue.

## ISO Standards
Displays the conformance data related to PDF subset ISO standards for PDF/A, PDF/UA, PDF/X, PDF/VT, PDF/E and PDF/VCR.
Note that very early PDF/X standards did not use XMP metadata but only the Document Information dictionary. 

# PDF Declarations
The PDF Association defines extensions to XMP metadata that allow documents to declare conformance to external industry and third-party specifications such as WCAG and HIPAA. See https://pdfa.org/declarations. 
