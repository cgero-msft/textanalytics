# Extract text and write to Excel when an image is added to SharePoint
This example shows how to use Power Automate to extract text from an image and write to an Excel file. The workflow is triggered when a file is added to a SharePoint folder.

If the file is a jpeg image, then Azure OCR is called to extract the text. Then the text is passed to Text Analytics to extract the key phrases.

The output is then written to an Excel file. The sample file is in this folder call [Text from OCR.xlsx](Text%20from%20OCR.xlsx).

