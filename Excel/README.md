# Trading Economics - Excel Add-In
This add-in provides to Trading Economics API users easiest way to load different kind of data directly to Excel spreadsheet.
**Note:** This add-in support only  32-bit version of the Excel  

## Installation
If you never downloaded MSCOMCT2.OCX file, do it: 

1. Download file from  https://www.ocxme.com/files/mscomct2_ocx

2. Extract the .ocx file from the zip file.

3. Copy to the system folder (c:\windows\sysWOW64 for 64 bit systems and c:\windows\system32 for 32 bit)

4. Run the command prompt as an administrator (from Start menu, type "cmd", then right click the cmd.exe file and choose "Run as Administrator"),
then use regsvr32 through the command prompt to register the file (e.g. "regsvr32 c:\windows\sysWOW64\mscomct2.ocx") 

Message "DllRegisterServer in mscomct2.ocx succeeded." should appear.  
Information source http://stackoverflow.com/questions/15816014/how-to-install-mscomct2-ocx-file-from-cab-file-excel-user-form-and-vba.

#### To activate an Excel add-in    

1. Download Trading Economics.xlam from https://github.com/ieconomics/open-api/raw/master/Excel/Trading%20Economics.xlam

2. In Excel workbook click the File tab, click Options, and then click the Add-Ins category.

3. In the Manage box, click Excel Add-ins, and then click Go. The Add-Ins dialog box appears.

4. Click the Browse... button then find a Trading Economics.xlam file  and select it.              

5. Click OK.  

Information source https://support.office.com/en-us/article/Add-or-remove-add-ins-0af570c4-5cf3-4fa9-9b88-403625a0b460.

#### Add a button to your own group on the ribbon

1. Click File > Options > Customize Ribbon.

2. Under Customize the Ribbon, in the Main Tabs list, check the Developer box if it is not already checked.

3. Pick the tab where you want to add your own group.  
For example, pick Home, to add your group to the Home tab.

4. Select New Group.  
That adds New Group (Custom) to the tab you picked.

5. To use a better name for your new group, click Rename, type the name you want in the Display name box, and then click OK. You can enter a space in the name.  
For example, type Trading Economics.

6. To add a macro to the group, in the Choose commands from list, click Macros.

7. Select the next macros Calendar, Forecast, Historical, Indicators, Markets to add to your new group, and then click Add. The macro is added to the Trading Economics group.

8. To select a button icon for your macro, click Rename, and Under Symbol, select a button icon.

9. Click OK twice.

Information source https://support.office.com/en-us/article/Assign-a-macro-to-a-button-728c83ec-61d0-40bd-b6ba-927f84eb5d2c. 

##Using Trading Economics Add-In

**Notes:**

1. Red cross button of the popup windows is disabled for the moment, to exit click Cancel button.
2. Clicking on one of the buttons, for the first time, will appear a window to insert credentials, if you don't have them just click OK.
3. Fields "Sheet name" and "Cell name" are optional, you can left them in blanc, so data will start from selected cell.

**Markets:** In Category field click on drop down button(triangle) and then choose one of four available options.  
**Indicators:** To get all indicators for some specific country just choose the country in Country field and click OK.  
To get specific indicator for some country, first choose the country in Country field then choose available indicator in Indicator field and click OK.  
**Historical:** Select country and indicator in respective fields, multiple selection is available. By defaulte you will get historical data for a year starting on the current day. You can change time range in Start Date and End Date fields.  
**Forecast:** You can choose only country to get forecasted values for all indicators of the chosen country. You can choose only indicator to get forecasted values for specific indicator for all countries.Or you can choose country and indicator to get forecasted value for specific indicator of the chosen country.  
**Calendar:** To get Calendar events for all countries just click OK. To get Calendar events for specific country, select country (multiple selection is available) and click Add button then click OK. You can change time range in Start Date and End Date fields. 
