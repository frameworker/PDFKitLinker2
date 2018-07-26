# PDFKitLinker2
PDFKit sample

PDFKitLinker2 presents many features of (Tiger) PDFKit. 

This application allows the user to annotate a PDF document by embedding links or editing existing ones. The destination of a link may be another page in the document, or an external URL.

PDFAnnotationLink was the one interactive annotation that was properly implemented for Tiger. So that's why this sample was written; at the time, links were the only game in town :-)

PDF Linker also shows how to create and display a PDFOutline of the opened document.

If the opened PDFDocument has an outline, PDF Linker will create and display the outline in an NSDrawer. This is a very useful recipe — and worth the price of admission, all by itself :-)

Familiarity with NSTableView would be very helpful in understanding the code for this, but lacking that, it would still be possible to use PDF Linker as a "Rosetta Stone" to figure Table Views out.

Original Info:

Many features of PDFKit are presented in this application. Ostensibly the application allows you to open PDF's and edit existing Link annotations or create your own.
 
 The code itself demonstrates two different means of searching a PDF.
 It presents an NSToolbar to control various aspects of PDF display and navigation.
 It subclasses PDFView to allow custom drawing and interaction.
 It makes heavy use of the PDFAnnotationLink class.
 It demonstrates the loading and saving of PDF's with PDFKit.

Revision History

2005-08-10 Version 1.1
Fixed broken links to files. Updated to produce a universal binary. No code changes were required.

2018-07-25 Version 2.0
Brought up-to-date in macOS 10.13.5 with Xcode 9.2
Base SDK 10.13
macOS Deployment Target 10.13
Repaired warnings and updated Deprecated APIs
Updated API usage for new PDFKit
Fixed bug that kept tableView from working
Added Read Me with Revision History and Eratta

Errata

"Overridden deprecated methods" warning needs to be turned on and warnings repaired.

Turn on other warnings and fix issues that crop up.
   https://github.com/boredzo/Warnings-xcconfig/wiki/Warnings-Explained

Serious bug when myDocument.nib is touched:
(Project contains zipped version so original can be replaced if it’s corrupted by Xcode)

THIS IS THE WARNING:

￼The document "my document.nib" had an internal inconsistency that was found and repaired.

This may be due to an SCM operation such as merging.
Please save document to fix the inconsistency.

The box with object ID 120 was configured as a separator line, but had a subview with the object ID 121. The view has been moved to the top level of the document.

WHEN YOU SEE THIS WARNING THE DOCUMENT HAS ALREADY BEEN CORRUPTED. REPLACE THE NIB WITH THE ZIPPED COPY.

NSDrawer has been deprecated in 10.13.

