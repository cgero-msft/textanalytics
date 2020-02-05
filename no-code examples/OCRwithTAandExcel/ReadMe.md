# Extract text and write to Excel when an image is added to SharePoint

## Overview
This example shows how to use Power Automate to extract text from an image and write to an Excel file. The workflow is triggered when a file is added to a SharePoint folder.

If the file is a jpeg image, then Azure OCR is called to extract the text. Then the text is passed to Text Analytics to extract the key phrases.

The output is then written to an Excel file. The sample file is in this folder called [Text from OCR.xlsx](Text%20from%20OCR.xlsx).

Here is the example's workflow:
![alt text](images/steps.JPG "example's steps")

## Pre-requisites

1. A valid Azure subscription - if you don't have one, create one for [free](https://azure.microsoft.com/en-us/free/services/cognitive-services/).
2. Create a Text Analytics resource (if you don't already have one)
- Start [here](https://docs.microsoft.com/en-us/azure/cognitive-services/cognitive-services-apis-create-account?tabs=singleservice%2Cwindows#create-a-new-azure-cognitive-services-resource)
- Select Text Analytics in step 1. Then create the resource.
- Get the key and endpoint 
- Skip the Configure the environment and Clean up sections
3. Power Automate - if you haven't already, sign up for free [here](https://docs.microsoft.com/en-us/power-automate/sign-up-sign-in)
4. OneDrive for Business (thru Office 365)[more info here](https://onedrive.live.com/about/en-US/business/)
- Upload the example Excel file (found in this folder) to your OneDrive for Business folder

## Create the flow in Power Automate
The entire flow is shown below. 
![alt text](images/OCRwithTAtoExcelSteps.png "complete flow")

