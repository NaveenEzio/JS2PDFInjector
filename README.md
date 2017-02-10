# JS2PDFInjector
Use this tool to Inject a JavaScript file into a PDF file.

To do this you will need an existing PDF file, and a ".js" file which contains the commands you would like to run when the document is opened.
I use this to create PDFs with some active code in there that I can email to customers, or download through their proxies, to check for the JavaScript being removed or blocked.
When you open the produced PDF with the JavaScript injected in Adobe you should see your code execute. Mileage varys in other viewers and for certain Edge in Windows 10 does not execute.

## JavaScript API available in PDF

The following URL contains the JavaScript API details:

http://www.adobe.com/content/dam/Adobe/en/devnet/acrobat/pdfs/js_api_reference.pdf

These are different from browser based JavaScript so reading that to achieve anything advanced is recommended.

## Example JavaScript

Who doesn't love a simple alert message? I know I do. The following code is all you will need for your hello world alert message:

```app.alert("Hello world!");```

A little different from just "alert". Your alert method now lives attached to the "app" object. Nothing too crazy.

## How to use

Follow the steps below to create your PDF:

* Execute the jar in the "dist" folder. 
* This will open a GUI prompt that asks you to point it at a PDF file. 
* Select the PDF file you would like to inject in to.
* Another prompt will appear looking for the file containing your JavaScript.
* Select that file.
* This will create a new file in the same directory as the PDF with "js_injected_" prepended in the name.


