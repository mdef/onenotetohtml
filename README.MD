**Description**

Here is the way how you can migrate from 
Microsoft Onenote to [tagspaces](http://www.tagspaces.org "").
In my case I had 3 notebooks with 1500 notes.
It absolutely no way to recreate them manually.
I've did it with Onenote 2010, if you have later version I believe that you are able downgrade notebooks to 2010.

**Migration**

You have to run Excel and Onenote simultaneously.

1. In Excel open onetohtml.xlsm

2. On the Developer tab, click Visual Basic. This opens the Visual Basic Editor. (If you do not see the Developer tab in Excel, click the File tab, and then click Options. In the categories pane, click Customize Ribbon, select Developer, and then click OK. [msdn](https://msdn.microsoft.com/en-us/library/hh377185.aspx ""))

3. Change *FILE_PATH* variable to appropriate place where you have write permissions.  

4. Switch to OneNote. In OneNote you have to choose your first notebook to export. (If you have only one notebook, then you are done with this step.) If you have multiple notebooks you have to proceed all the steps with for every notebook you have and every time you have to change *FILE_PATH* according to the name of your notebook, then notes in notebooks will be separated as they been in Onenote.

5. Switch to Visual basic for Applications  and click play button  :)  or F5. For me it was not very fast, but you can control the process observing file creation in *FILE_PATH* location.

As result you should have bunch of html files with your notes together with hierarchy, as in Onenote.


**Note:**

If for some reason onetohtml.xlsm is not working for you, it still could be done. You have to proceed all the steps in [Publishing to a PDF file in OneNote 2010 from msdn](https://msdn.microsoft.com/en-us/library/hh377185.aspx "")
Here are the steps:


**Add Library References to the Excel Workbook**

To add references to the workbook
1. Start Excel 2010.
2. On the Developer tab, click Visual Basic. This opens the Visual Basic Editor.

**Note**

If you do not see the Developer tab in Excel, click the File tab, and then click Options. In the categories pane, click Customize Ribbon, select Developer, and then click OK.

3. On the Tools menu, click References.
Scroll to Microsoft OneNote 14.0 Object Library, and then select it.
4. Next, scroll to Microsoft XML, 6.0, select it, and then click OK.

**Add a Standard Module to the Excel Workbook**

In this task, you insert a standard module into the Excel workbook.

To add a standard module to the Excel workbook
    
On the Insert menu, click Module. This adds Module1 to the Projects pane on the left side of the Visual Basic Editor.
    
Add the Code to the Visual Basic Editor
In this task, you add programming code to the Visual Basic Editor.
To add code to the Visual Basic Editor
In the Projects pane, click Module1.
Paste or type the following Microsoft Visual Basic for Applications (VBA) code into the module window.

Use code from onenotetohtml.bas.

And and click play button  :)  or F5.
