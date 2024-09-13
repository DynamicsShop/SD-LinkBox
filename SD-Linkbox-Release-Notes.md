## SD Linkbox Releases

### 6.0.4

#### Enhancements

- AppSource App - User Groups are retired in 2024 release wave 2 and are replaced with Security Groups. A new SD LinkBox Security field was added to the SD LinkBox Drop Point Card.

- AppSource App - A change was made to the Assisted Setup data import functionality.

- AppSource App - The logo in the App was updated to the new logo.

### 6.0.3

#### Bug Fixes

AppSource App - A fix was made the SD LinkBox Extension Page where page extension names were identical due to the length of the original page name.

### 6.0.2

#### Enhancements

- AppSource App - New functionality was added to post files to LinkBox via json API. The API is called form an external source with a record type and record ID to allow a write of data into the specified SD LinkBox Drop Point.

- AppSource App - On creation of a new drop point the values entered in the Setup Card in the Azure Blob Storage FastTab are inserted into the Drop Point. If the Drop Point is already created and details on the Setup Card for Azure Blob Storage are changed, it is not best practice to automatically update values on existing Drop Points that are being used. Choose the Apply Shared Key to existing Drop Points action on the SD LinkBox Setup card to update the Shared Key to Drop Points with the same storage account name.

- AppSource App - The extension uploading dialog  in the SD LinkBox Extension page was updated.

- AppSource App - The links in the About page were updated.

### 6.0.1

#### Enhancements

- AppSource App - A change was made to limit the SD ISV Tenant Subscriptions page to display just our SD ISV AppSource Apps and not other SD PTE Apps.

#### Bug Fixes

- AppSource App - An error was raised on upload of files to a Drop Point that "A call to System.Security.Cryptography...failed with this error message...". SD Linkbox was using block size of 256 this has been restricted to 128 by Business Central. Passwords will need to be re-entered in the SD Linkbox Setup Card. 

- AppSource App - When selecting SD Linkbox activity pages in a the Tell Me/Search in a BCv22 environment, the activity pages were hanging.

- AppSource App - A change was made to the ISV Licence Notification procedure in SD Linkbox to fix an issue that would raise an error when the language is changed from English to another language.

- AppSource App - An error will raise in the Assisted Setup import if non sequential enum values exist in the imported data. This was fixed.

### 6.0.0

#### Enhancements

- BCv21 App - New functionality was added to SD LinkBox to allow a user to surface a Drop Point on a page without the need for a developer to create an extension. Users can create and publish a custom extension in the SD Linkbox Extension page.

- BCv21 App - The App Name field in the SD Linkbox Extension page was changed to default to SD Linkbox Extension and was set to non-editable. After choosing the Create App action, the Publisher field is also set to non-editable.

- BCv21 App - The Actions in the Related group on the SD Linkbox Setup were reordered and action names were updated.

- BCv21 App - A small typo in the SD Linkbox Extension page was fixed.

- BCv21 App - A change was made to the message displayed when the user chooses the Publish Package action in the SD Linkbox Extension page.

- BCv21 App - The action names in the SD Linkbox Extension page were changed to Create App, Download App and Publish App and the Runtime Version field was removed from the page.

- BCv21 App - The Change Type field in the Page Extensions list on the SD Linkbox Extensions page was changed to FactBox Position.

- BCv21 App - The Product Activation Page was updated to point to the new CRM URL.

- BCv21 App - The Licence Expiry Message/Notification was updated with the App Name.

- BCv21 App - A new page was created to display all Simply Dynamics Apps and Subscription details for the tenant.

- BCv21 App - The Licence Message displayed on first install of App was changed to prompt the user to activate a free trial and choose Assisted Setup to create demo data.

- BCv21 App - The URL links in the About page were updated to point at our new website.

- BCv21 App - The ToolTips were updated to look at our new website.

#### Bug Fixes

- BCv21 App - A fix was made to the code for licence key checks on the SD LinkBox Role Centre.

### 5.0.1

#### Enhancements

- BCv19 App - Added the Latest Version of the product and the AppSource URL to the About Page. 

- BCv19 App - Added the Latest ISV Licence Control with fix to Free Trials in Public Environments. 

#### Bug Fixes

- BCv19 App - The Product Activation page was updated to disable the Activate button until a Product Key is filled in. This will avoid an error being raised when Activate is chosen with no Product Key entered.

- BCv19 App - Fixed an issue where after getting a message that the Free Trials were exceeded and clicking on the Assisted Setup action an error was raised.

### 5.0.0

#### Enhancements

- BCv18 Public App - Made a change to allow Drop Point to be enabled only if a Table No. has been specified in the Table Links FastTab on the Drop Point Card.

- BCv18 Public App - The Actioned On field was added to the Checkout Log accessible from the Dropped Files FactBox. 

- BCv18 Public App - The Show Checked Out Files action was added to the Actions group in the SDY ULB Drop Point List.

- BCv18 Public App - A new Expiry Date List page was created and is accessible through the Expiry Dates cue from the SD Linkbox Role Centre.

- BCv18 Public App - Added the ISV Licence Controller to SD Linkbox.

- BCv18 Public App - The message displayed on import of the demo data xml file when the Assisted Setup action is chosen was updated.

- BCv18 Public App - A prompt was added to the SD Linkbox Setup on change of Azure Blob Storage Config, Dropbox Config or OneDrive Config to inform users that these changes will effect the storage and links of files on the Drop Points.

- BCv18 Public App - Drop Points with a Storage Type of OneDrive, Dropbox and Azure Blob Storage cannot have the Drop Point Code modified once files have been dropped to the DropPoint.

- BCv18 Public App - Rewrote the code to prevent and error being raised when adding a Client Secret for OneDrive and DocuSign to the Setup Card.

- BCv18 Public App - The order of Actions in the Actions group on the Dropped Files FactBox were regrouped and reordered.

- BCv18 Public App - The Drop Point, Drop Point Name and Drop Point Enabled fields were removed from the Template Files list in the Drop Point Card.

- BCv18 Public App - Renamed the All Drop Points cue on the SD Linkbox Role Centre to Active Drop Points.

- BCv18 Public App - BCv18 Public App - Changes were made to the SD Linkbox Setup - fields were recaptioned, order of FastTabs were changed and actions added to the menu.

- BCv18 Public App - The latest changes to the ISV Licence Controller were added to SD Linkbox.

- BCv18 Public App - SD Linkbox permissions were converted to permission set AL objects.

- BCv18 Public App - The option to Allow HTTP Request for SD Linkbox in the Extension Management is set to true by default on install of SD Linkbox.

- BCv18 Public App - Functionality was added to SD Linkbox to store dropped files on OneDrive.

- BCv18 Public App - Functionality was added to SD Linkbox to store dropped files to Azure Cloud Storage.

- BCv18 Public App - A change was made to the Role Centre to surface a cue with the count of files with Expiry Dates specified.

- BCv18 Public App - A change was made to handle the situation where users create an App on Dropbox, drop files to the Drop Point, delete the App on Dropbox and then delete the dropped files on the Drop Point.

- BCv18 Public App - Updates to the Dropbox API were reviewed. 

- BCv18 Public App - On install of SD Linkbox, an SD Linkbox File Check-In Reminders notification is added to the My Notifications list. This notification is set to enabled by default.

- BCv18 Public App - A small typo on the DocuSign Templates page was fixed.

- BCv18 Public App - The Rec ID filter was added to the Dropped Files list as selecting the Filename in the File Versions list opened a blank page.

- BCv18 Public App - Code to notify users of checked out files was reviewed and updated as the standard code for notifications has changed from the original C/AL code base.

- BCv18 Public App - A visual change was made to the Expiry States page - a group caption was removed.

- BCv18 Public App - Code reworked when adding Document Report No. to the Table Links FastTab. Only reports that have the related table as the current table link are displayed and when running the test report the request page is displayed.

- BCv18 Public App - Changes were made to the Drop Point list - menu groups were renamed and reordered.

- BCv18 Public App - API calls to Dropbox from SD Linkbox were updated to handle and throw an error if the file didn't sync to Dropbox correctly. 

- BCv18 Public App - API calls to Dropbox from SD Linkbox were updated to handle and throw an error if the file didn't upload to Dropbox correctly. 

- BCv18 Public App - The API Authentication FastTab was renamed to Dropbox Options.

- BCv18 Public App - Changes were made to the grouping of Actions in the Drop Point Card.

- BCv18 Public App - Changes were made to the Setup card - a typo was fixed and FastTabs were renamed.

- BCv18 Public App - Added Assisted Setup to SD Linkbox.

- BCv18 Public App - The Usage Category was updated for SD Linkbox pages so the pages are visible in the Tell Me search.

- BCv18 Public App - Code was reviewed to see if Name and Description fields needed to be changed from 50 to 100 characters as per standard Dynamics 365 Business Central.

- BCv18 Public App - Permission Sets SDY ULB ADMIN, SDY ULB USER and SDY ULB VIEW were added to the product.

- BCv18 Public App - Prepared the product for submission to AppSource.

- BCv18 Public App - Created a Role Centre for SD Linkbox.

- BCv18 Public App - Created functionality to handle the movement of record links on sales and purchase end of life transactions. Applicable for Sales Header to Posted Sales Invoice/Posted Sales Credit Memo transactions, for Purchase Header to Posted Purchase Invoice/Posted Purchase Credit Memo transactions.

- BCv18 Public App - Extensions to SD Linkbox were made for the following standard Dynamics 365 Business Central pages: Customer Card, Customer List, Vendor List, Item List, Sales Quote List, Sales Order List, Sales Invoice List, Posted Sales Invoice List, Sales Return Orders, Sales Credit Memo List, Posted Sales Credit Memo List, Purchase Quotes, Purchase Order List, Purchase Invoice List, Posted Purchase Invoice List, Purchase Return Order, Purchase Credit Memo, Posted Purchase Credit Memo.

- BCv18 Public App - Created a demo data xml file to import into SD Linkbox.

- BCv18 Public App - Added the ability to integrate SD Linkbox with OneDrive.

- BCv18 Public App - Added the ability to integrate SD Linkbox public app with Dropbox.

- BCv18 Public App - Converted version 4.0.0 of C/AL code base to AL for Public App build.

#### Bug Fixes

- Bcv18 Public App - Viewing files is now limited to pdf or text files only for a database storage type and pdf files for all other storage types. 

- BCv18 Public App - Fixed an issue where the report is generated if you choose cancel on the report filters after choosing the Test Report Action in the Drop Point Card. 

- BCv18 Public App - Fixed an issue where a blank report was generated and an error was raised on open of the report if the user chose the Test Report Action in the Drop Point Card and no report content was generated.

- BCv18 Public App - On selection of the Document Report No. in the Drop Point Card, the name of the chosen report did not default into the Document Generation Report Name.

- BCv18 Public App - The Report sent to DocuSign from the Drop Point was not the report that the user was prompted to sign when logging in to DocuSign.

- BCv18 Public App - Check in Reminders were only sending for a linked record once even if there were multiple drop points or dropped files linked to the record.

- BCv18 Public App - A file was successfully dropped and uploaded to a OneDrive Drop Point but when downloading or viewing the file an error was raised.

- BCv18 Public App - Fixed an issue where reverting a file was not logged in the Checkout Log.

- BCv18 Public App - Fixed an issue where the Send Check-In Reminder was enabled for the user who checked out the file but not for the user who needed to send the reminder to the person who had the file checked out.

- BCv18 Public App - Fixed an issue where renaming/modifying a Drop Point Code caused the system to hang. Also users are no longer allowed to modify a Drop Point code once files have been dropped to the Drop Point. An exception being Drop Points with a database storage type.

- BCv18 Public App - The option to check back in a checked out file was disabled.

- BCv18 Public App - The icon on the Drop Point Card was intermittently displaying the incorrect Icon chosen in the Drop Point Card.

- BCv18 Public App - Fixed an error that was raised when the Add Template File action chosen in the Dropped Files Factbox.

### 4.0.1

#### Enhancements

- BCv14 Private App - An SD Linkbox Permission Set was added to the App.

### 4.0.0

#### Enhancements

- BCv14 Private App - Recipients subpage not editable when sending DocuSign Templates.

- BCv14 Private App - Refactored code to prevent Error messages when adding Template file to Drop Point.

- BCv14 Private App - Reworked functionality to the Attach Report action on Drop Points.

- BCv14 Private App - Reworked functionality to fix the View Template File action in Drop Point Card.

- BCv14 Private App - The product activation/licensing setup was added to the product.

- BCv14 Private App - Converted version 4.0.0 C/AL code base to Private App AL Extensions.

- BCv14 C/AL - A C/AL Upgrade Path from v3.0.0 C/AL to v4.0.0 C/AL was developed.

- BCv14 C/AL - Setup tables were added to the XML Export files.

- BCv14 C/AL - Expiry Date format is now based on local settings.

- BCv14 C/AL - Changes were made to the Drop Point Types page.

- BCv14 C/AL - An action to access the Setup Card was added to the Drop Point Types List.

- BCv14 C/AL - Usage Categories were updated on pages.

- BCv14 C/AL - Changes were made to the Docusign functionality.

- BCv14 C/AL - Code was added for SANA Assisted Setup.

- BCv14 C/AL - Functionality was created to allow SANA Document Attachments.

- BCv14 C/AL - Changes were made to the Linkbox Setup Card and Tables.

- BCv14 C/AL - Created functionality to allow SANA Product Attachments.

- BCv14 C/AL - Created a SANA Product Images Codeunit.

#### Bug Fixes

- BCv14 C/AL - An issue was fixed were an error was raised when downloading a file from a Drop Point.

### 3.0.1

#### Enhancements

- Fixed an issue where users were unable to checkout files from the webclient browser.

- Fixed an issue where an error message was raised and users were unable to view or download files from Drop Point when run in the Web Client.

### 3.0.0

#### Enhancements

- A fix was made to checkout and view files in a Dynamics 365 BC environment. 

- Enabled the Deploy Templates Action in the Drop Point Card if there are Templates for the Drop Point.

- For Drop Points with Templates defined and Expiry Dates switched on, prompt users to enter a date formula when users choose the "Deploy Templates" Action.

- The default sorting In the Expiry Date Card was changed to the Expiry Date. Files that will expire the soonest are displayed at the top of the list.

- A change was made that when manually adding a template file to the Dropped Files, for a Drop Point with Expiry Date functionality switched on, the user is prompted to enter an Expiry Date as per dragging and dropping of files to the Drop Point in the Drop Area.

- A change was made to refresh the Drop Point Icon in the Drop Area on the Customer Demo Page after an invalid file type was dropped on the Drop Point.

- Update the visual on the Drop Point to Error When dropping a file to a Drop Point and entering an expiry date in the past.

- Made a change to add the Drop Point Name to the SD-ULB Expiry File State List page.

- Created functionality to implement Expiry Date Alerts.

- Added a Partner Menu and included in FOB.

- Made a change to the Dropped Files FactBox to enable the Attach Report Action.

- Made a change to ensure client supports SSL (TLS/TLS1.1/TL1.2).

- Created a factory pattern that tests the client connection before returning a valid connected client and allow users to test the DocuSign connection.

- Added additional validation to the Linbox DocuSgn Library.

- Made a change that when a DocuSign envelope is created, if an error is raised between 'draft' and 'sent' then the envelope is moved to the deleted folder.

- Added an envelope status for the DocuSign Item.

- Added DocusSign audit fields to the Setup Table.

- Cleaned up the Dropped File FactBox Page.

- The Customer Demo Action was moved from the Drop Point List Page to the SD-ULB Setup Card and promoted to Home tab of the ribbon.

- Integer flow fields for the Drop Points were surfaced on the SD-ULB Setup Card.

- On the SD-ULB Linkbox Customer Demo page the caption was changed from “Linkbox Customer Demo” to “SD Linkbox Customer Demo”.

- On the Linkbox Setup Card the caption was changed from “Setup” to “SD Linkbox Setup”.

- Added a partner menu object to the release.

- A Test Service Action was added to  the Setup for DocuSign URLs.

- Added Contact lookup on DocuSign recipients.

- Reordered the pages to accommodate the new setup pages.

- Integrated the Simply Dynamics DocuSign API into Linkbox.

- Created functionality to send a Document to DocuSign, from SD Linkbox, using a template API.

- Created a Simply Dynamics Add In Installer for Docusign.

- Created a DocuSign Envelope from the Template Handler.

- Added the standard Simply Dynamics import/export module to the product.

- Created a Docusign Template Handler.

- Created DocuSign Authentication Handler functionality.

- Functionality created to communicate with the DocuSign API.

- Cleaned up the Drop Point Card.

- Added default DocuSign template code to Drop Points.

- Created additional fields on the Linkbox Setup Table and Page.

- Added functionality to auto attach report to a Drop Point.

- Added a Default Report ID field to the Drop Point table.

- Updated the object version to include the module SD-UTLB.

- Added the Simply Dynamics About Action to the ribbon on the new SD Linkbox setup page.

#### Bug Fixes

- Fixed an issue in the Expiry State Card where an error is raised if the user chooses to sort on the Expiry Date field. The field was changed from a flowfield and table structure changed.

- Fixed an issue where the page was timing out when choosing to Execute Alerts in SD-ULB Expiry State Card or opening the SD-ULB Expiry State Card when the Drop Point contained files with no Expiry Date specified.

- Fixed an issue where an error was raised when trying to delete a file from a Drop Point.

- Fixed an issue where on the dropped files FactBox the DocuSign Audit Option was not enabled.

- Fixed an issue where if a security filter record exists on the drop point with a blank user group code, the security filter was still applied.

- Fixed an issue where errors were raised when trying to assign a report ID to a table link.

- Updated the URL in the About Page.

- Fixed an issue where the Caption was not displaying on the third Fasttab in the Drop Point Card.

- Fixed an intermittent error that was raised on a page that contained a number of Drop Points.

### 2.3.3

#### Enhancements

- Refactored controls to Simply Dynamics.

- Enhanced User Interface handling between FactBoxes.

### 2.3.2

#### Enhancements

- Refactored SD-UTLB objects and Add-In installer. Removed all references to Cebuella in Linkbox objects.

- Refactored controls to Simply Dynamics.

- Linkbox: Allow users to browse for the file to upload to a Linkbox Drop Point instead of having to drag and drop the file to the Drop Point.

- Linkbox: an installer for the Linkbox Control Add-In was created.

- Linkbox: Created new functionality to add a document counter, with click through ability, to Drop Points.

#### Bug Fixes

- Fixed an issue where the Drop Point Icons were not displaying on the Customer Demo Link page.

- Fixed a NAV 2017 Compatibility issue.

### 2.3.1

#### Enhancements

- Linkbox: 

- Add a setup field to specify document checkout to a default Drop Point check out path.

### 2.3.0

#### Enhancements

- Linkbox: 
- Created check in/check out functionality for Linkbox Version Control. 
- Added Edit Permission to Linkbox. 
- Cleaned up code. Launch: 
- Upgrade Launch to use Control Suite.

#### Bug Fixes

- Linkbox: 
- Fixed Error Message raised when viewing a file in the Drop Point or Versions List. 
- Fixed situation where the View Option was always displaying the same file.

### 2.1.2

#### Enhancements

- Updated readme.txt file. 
- Launch - applied Launch standardised document layouts to the Posted Purchase receipt report.
- Linkbox - enhanced Linkbox file overwrite confirmations.

#### Bug Fixes

- Linkbox - fixed a bug in the scrolling functionality when selecting an Icon for a Drop Point in the Drop Point Card. 
- Linkbox - fixed an issue where when choosing to Edit certain files from the Dropped Files Factbox an error is raised. 
- Linkbox - fixed an issue where Delete Permission on Dropped Files Fact Box not taken into account when you right-click on the Dropped Files Fact Box.
- Launch - fixed alignment issue on the SD-U Customer Payment Receipt Document.

### 2.1.1

#### Enhancements

- Linkbox - enhanced the Icon Scoller picker.
- Linkbox - enhanced the Template functionality - allow users to choose to push out the Templates to the Linked tables and select the template they want to attach to the records. 
- Launch - surface filters on SD-U Bank Acc. Recon. Stmt Document. 
- Launch - surface filters on the SD-U Bank Acc. Recon. Smt Test Document. 
- Launch - improvement in code to allow for barcode record type value. 
- Launch - optimised the image preview generation. 
- Launch - surfaced the newly added Documents to the Role Center. 
- Launch - applied Launch standardised document layouts to the SD-U Customer Payment Receipt Document.

#### Bug Fixes

- Launch - fixed alignment issue on SD-U Sales Return Order Document. 
- Launch - fixed alignment issue on SD-U Purchase Return Order Document.
- Launch - changed the Launch Documents to use the document currency code rather than customer/vendor currency code when deciding the bank details to use on the footer.
- Linkbox - fixed a bug in the auto linking functionality of a Template File to a record.
- Linkbox - fixed a bug in the Version History of Dropped Files Linked to a record. 
- Linkbox - fixed a bug in the Version History of auto-created Template Files. 
- Linkbox - fixed a bug where an error was raised on creation of a new record when a Drop Point (with Versioning turned on) is added to a Card Page. 
- Linkbox - fixed a bug where the Icon Scroller images were not updating. 
- Power BI - fixed an issue where the Return Sales Order as raising an error if there was no BI Setup.

### 2.1.0

#### Enhancements

- Launch: 
- All Launch Documents and Reports underwent a code clean up. 
- A Delivery Docket was added to Launch. 
- A Manifest Report was added to Launch. 
- A Bank Account Reconciliation Statement (Posted Entries) was added to Launch. 
- A Bank Account Reconciliation Statement (UnPosted Entries) was added to Launch.
- A Stock Take Report was added to Launch.
- A Sales Return Order was added to Launch.
- A Purchase Return Order was added to Launch. 
- A Balance Forward Statement was added to Launch. 
- A standardised layout was applied across all Launch Documents and Reports. 
- All Field Names and abbreviations were standardised. 
- Decimal formatting was standardised across all Launch Documents and Reports. 
- A new Footer totalling layout and a VAT Grid layout was applied and standardised across the Launch Documents. 
- Positioning of Logos was made consistent across all Launch Documents and Reports. 
- A standard Header and Footer layout and banner, for portrait and landscape layouts, was applied across all Launch Documents and Reports. 
- An enhancement was made to allow users to choose the Background and Foreground Header and Footer Banner Colours that would print on all Launch Documents and Reports using a Colour Picker.
- Enhancements were made to the Remittance Advice Reports in Launch. Captions were changed, fields were resized. 
- Functionality to define and display a Barcode on all Launch Documents and Reports was added to Launch. 
- A Report Info Box was applied to the layout of all Launch Documents and Reports.
- Functionality was added to allow users to dynamically add the fields to print in the Report Info Box. 
- Minor layout changes were made to existing individual Launch Documents and Reports.
- New functionality was added to allow users to select the Background and Foreground Header and Footer Banner Colours by using a colour picker. 
- Improved the resolution of the Report Info Box. 
- Fields and FastTabs for new functionality were added to the Launch Setup Card.

Linkbox: 
- New functionality added to Linkbox to Security Filter Tables and Pages enabling permissions to be set. 
- Updated the Linkbox Setup to include Security Filters 
- New Security Filters for Dropped Files applied. 
- New Security Filters for Drop Areas applied.
- Added Company to membership lookup in Linkbox Security Filters. 
- New Version Control functionality added to Linkbox. 
- Provided Version Edit functionality. 
- When viewing a file in the Drop Area, the file is set to read only. 
- Coded increments for Dropped File Entry No. 
- Created a new Table and Page to list, and provide, Dropped File Version functionality. 
- Created Template functionality for Linkbox.
- Changed functionality to retain the SD Linkbox - Orphan Link Files. 

Profiler: 
- An XMLPort was created to export and import Profile Select List. 

PowerBI: 
- Added Sales Quote Tracking Functionality to PowerBI. 
- Added functionality to provide for CSV Import/Export for BI Date data. 
- Added the PowerBI Setup Page to the SD Utilities Role Centre

#### Bug Fixes

- Launch: 
- Fixed bug where the Statement report overwrites any Date Filters that are passed into the report. 
- Fixed bug where colour choices picked using the colour picker were being re-set. 
- Fixed bug where the QR Barcode was not displaying correctly in the Report Information box. 
- Fixed bug in the Launch Report Setup whereby when a new record was added to the Report Info Box Fields for a specific report, the Field No. was not appearing in the order as specified but rather in the order as input. 
- Fix was made to the barcode generation to display as per Launch Report Setup. 
- Minor layout changes were made to existing individual Launch Documents and Reports.
- Fixed bug which allowed a Barcode to be setup on the Launch Report Setup with a DPI of zero. 
- Fixed bug where the List of Reports showing in the Launch Setup was being hard code filtered on an earlier version release. 
- Fixed bug where the InfoBox and Barcode were not being updated. 

Linkbox: 
- Drop Point Icons on List Pages are intermittently not displaying when the List Page is loaded from within the Role Centre.
- Fixed bug where a link is being created to records with no file attached when a record for a Template File that has no File Imported (a blank Filename field) is created. 
- Fixed error raised when an empty file is dragged and dropped into a Drop Point.

Profiler: 
- Remove irrelevant Actions from the Profile Selection List.

### 1.1.0

#### Enhancements

- Linkbox - created XMLPorts for Upgrade to NAVW19.00 - V2.1.0 
- Profiler - created Profiler Date export 
- Power BI - created BI Date XML PortXML Port

#### Bug Fixes

- Launch - fixed bug where statement report overwrites passed in Date Filter

### 1.0.2

#### Enhancements

- Linkbox - Drop Area was not displaying on the Role Center.
- Launch - Unable to run statement when specified from report selection.

### 1.0.1

#### Enhancements

-  Documentation fixes.

### 1.0.1

#### Enhancements
- Linkbox - Created an XmlPort for setting up control Add-in. 
- Profiler - Refactored the object selection. Rewrote the reports to loop on the questions and do basic formatting of them. 
- Profiler - Renumbered and reordered the Tables and Pages. 
- Cleaned up the objects. 
- Code upgraded to 2016.

