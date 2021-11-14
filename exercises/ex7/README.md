# Exercise 7 - Integration to Financial Planning
In this exercise, we will create...

## Description

After completing these steps you will have created...

1. Navigate to **Files** in the main menu.
2. Type in HXM in the search field.
3. Click on the model **HXM Integrated Workforce Planning**.
<br>![](/exercises/ex7/images/07_0001.png)
4. Click on the **SAP_HR_COSTTYPE** to open the maintenance view for the dimension.
<br>![](/exercises/ex7/images/07_0002.png)
5. The dimension Cost Type has an attribute **GL_Account** which maps the cost type for HR planning to a GL account in the financial planning model. Make sure that you maintain the GL account attribute as shown in the screenshot.
<br>![](/exercises/ex7/images/07_0003.png)
6. Click on the back icon to navigate back to the search results.
<br>![](/exercises/ex7/images/07_0004.png)
7. Click on **SAP HXM Workforce Planning** to open the folder.
<br>![](/exercises/ex7/images/07_0005.png)
8. Click on the item **WFP – Overview page** to open the application in the analytics designer.
<br>![](/exercises/ex7/images/07_0006.png)
9. Select the item **hyperlink_publish** in the Outline window.
10. Click on **Designer** to open the Styling panel.
11. Make sure that the check box **Show this item at view time** is active.
<br>![](/exercises/ex7/images/07_0007.png)
12. Click on **Run Analytic Application** to start the application.
<br>![](/exercises/ex7/images/07_0008.png)
13.	On the overview page, you will see the entry Publish **Result To Financial Plan for SAP S/4HANA**.
14.	Click on **Publish Result To Financial Plan for SAP S/4HANA** to open the application.
<br>![](/exercises/ex7/images/07_0009.png)
15.	In this application, you can derive the corresponding G/L accounts for the planned HR costs and transfer the data to the financial planning model.
<br>![](/exercises/ex7/images/07_0010.png)
16.	Add a filter by clicking on the **filter** icon at the top left corner of the page.
17.	Select **Company Code** from the list of available dimensions.
<br>![](/exercises/ex7/images/07_0011.png)
18.	From the member selector, pick **BestRun Germany**. Click on **OK** to confirm your selection.
<br>![](/exercises/ex7/images/07_0012.png)
19.	Click on **General Settings** to set some parameters for the data transfer to the financial plan.
<br>![](/exercises/ex7/images/07_0013.png)
20.	In the settings dialog, you can specify the source version in the WFP model as well as the planning level. In addition, you can define the target version in the financial planning model.
21.	Click on **OK** to confirm the settings.
<br>![](/exercises/ex7/images/07_0014.png)
22.	Click on **G/L Mapping** to derive the G/L accounts.
<br>![](/exercises/ex7/images/07_0015.png)
23.	Click on **OK** to confirm the mapping parameters and start the derivation.
<br>![](/exercises/ex7/images/07_0016.png)
24.	In the Cost Overview table, you will see the planned cost types together with the corresponding G/L accounts.
<br>![](/exercises/ex7/images/07_0017.png)
25.	Click on the button **PUBLISH TO P&L** to transfer the data to the financial planning model.
<br>![](/exercises/ex7/images/07_0019.png)
26.	Click on **OK** to confirm the settings and start the transfer.
<br>![](/exercises/ex7/images/07_0020.png)
27.	In the table **Financial Plan Overview** you can see the result of the transfer.
<br>![](/exercises/ex7/images/07_0021.png)


## Summary

You've now ...

Continue to - [Exercise 8 - Add additional cost types](../ex8/README.md)
