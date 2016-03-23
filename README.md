# Flash PHP samples

#### This repository contains the source code of examples for using Stimulsoft Reports.PHP with Stimulsoft Reports.FX components.

# Overview
This repository has website project with some examples.

# Running samples
Samples folder contains all application files, including the 'index.html' file. So all files from this folder are required to be copied on your PHP server (using ftp or http access interface - depending on your hosting provider). Then, in your browser, you can go to the following address: 
http://you_domain_name/index.html

If you use the PHP server installed on local developers computer: 
http://localhost/index.html

# Stimulsoft Reports.PHP
These examples are applicable for Stimulsoft Reports.PHP, the reporting tool designed for creating and rendering reports on your websites.

You can try the Live demo [here](http://js.stimulsoft.com/)

Read more about Stimulsoft Reports.PHP at [www.stimulsoft.com](https://www.stimulsoft.com/en/products/reports-php)

# Configuration of Stimulsoft Reports.Fx for PHP

The **config.xml** file is used to configure the **Designer.Fx** and **Viewer.Fx**. This file is automatically called by the designer of viewer immediately after loading.


The **Connection** section defines the connection settings:

Setting | Description
------------ | -------------
ClientRequestTimeout | Maximum time waiting for a response from the server (in seconds), after which the connection will be terminated
ClientRepeatCount |	The number of command repeats to the server when getting the erroneous data
ShowCancelButton	| Displaying the cancel button when performing any action (such as loading a report or data)


The **Localizations** section defines localization settings:

Setting | Description
------------ | -------------
Localization | Interface localization that will be loaded and applied by default. The value is the localization file name without extansion. For example, **<Localization>en</Localization>**. The following should be located in the localization folder on the server. If the **Default** value is specified to the localization then the previously selected localization will be applied.


The **Viewer / Toolbar** section defines settings of the viewer panels:

Setting | Description
------------ | -------------
ShowPrintButton | Shows the 'Print' button
ShowOpenButton | Shows the button for opening a report from the user's local disk
ShowSaveButton | Shows the button for saving a report to the user's local disk
ShowBookmarksButton | Shows the 'Bookmarks' button and panel
ShowThumbnailsButton | Shows 'Thumbnails' button and panel
ShowFindButton | Shows the 'Find' button
ShowFirstPageButton | Shows the button for switching over the first page of a report
ShowLastPageButton | Shows the button for switching over the last page of a report
ShowPreviousPageButton | Shows the button for switching over the previous page of a report
ShowNextPageButton | Shows the button for switching over the next page of a report
ShowGoToPageButton | Shows the button for switching over the page of a report indicated in the dialog window
ShowPageViewModeSingleButton | Shows the button for selecting the single page viewing mode
ShowPageViewModeContinuousButton | Shows the button for selecting the continuous page viewing mode
ShowPageViewModeMultipleButton | Shows the button for selecting the multiple pages viewing mode
ShowZoom | Shows the zoom slider
ZoomMode | Sets the report zoom mode while loading the viewer. It may have the following values: **Default, OnePage, TwoPages, PageWidth, Zoom25, Zoom50, Zoom75, Zoom100, Zoom150, Zoom200**. If the **Default** value is set then the latest zoom mode will be applied


The **Designer** section defines the report designer settings:

Setting | Description
------------ | -------------
Title | Defines the browser title that is set when loading the designer. If the parameter is not set then the defined report value or alias will be set as a title
ExitUrl | Defines the URL address to what there will be switching over when clicking the ‘Exit’ button in the main menu of the report designer
ShowWizardOnStartup | Calls the Startup report wizard when loading the designer


The **Designer / MainMenu** section defines settings of the main menu of the designer:

Setting | Description
------------ | -------------
New | Enables/disables the 'New' item of the main menu
NewReport | Enables/disables the 'NewReport' item of the main menu
NewReportWithWizard | Enables/disables the 'NewReportWithWizard' item of the main menu
NewPage | Enables/disables the 'NewPage' item of the main menu
OpenReport | Enables/disables the 'OpenReport' item of the main menu
SaveReport | Enables/disables the 'SaveReport' item of the main menu
SaveAs | Enables/disables the 'SaveAs' item of the main menu
DeletePage | Enables/disables the 'DeletePage' item of the main menu


The **Designer / Toolbar** section defines the settings of panels and other interface items of the designer:

Setting | Description
------------ | -------------
AllowModifyDictionary | Allows modyfing the data dictionary of a report
AllowModifyConnections | Allows modyfing connections of the data dictionary of a report
AllowModifyDataSources | Allows modyfing the data sources of a report
AllowModifyVariables | Allows modyfing the list of variables of a report
AllowModifyTemplate | Allows modyfing loaded components of a report
AllowScale | Allows page scaling
ShowCodeTab | Shows the 'Code' tab for showing the C#/VB.NET code of a report
ShowDictionaryTab | Shows the dictionary tab of the report data dictionary
ShowExitButton | Shows the 'Exit' button in the main menu of the designer
ZoomMode | Sets the report zoom mode while loading the designer. It may have the following values: **Default, OnePage, PageWidth, PageHeight, Zoom25, Zoom50, Zoom75, Zoom100, Zoom150, Zoom200**. If the **Default** value is set then the latest zoom mode will be applied


# Description of the Stimulsoft Reports.Fx files

These files are contained in the "stmilulsoft" folder:

Folder/File | Description
------------ | -------------
localization (folder) | This folder contains all localization files. The list of localization files is indicated automatically when loading the designer or viewer 
config.xml, designer.html, viewer.html, DesignerFx_PHP.swf, ViewerFx_PHP.swf | Client side application files of the Designer.Fx and Viewer.Fx 
index.php, handler.php, localization.php, database_xml, database_mssql.php, database_mysql.php, database_odbc.php, database_pg.php | Server side PHP scripts for the Designer.Fx and Viewer.Fx applications 
