# Exercise 7 - Integration to Financial Planning
In this exercise, you will learn how you can integrate the business content for SAP HXM Workforce Planning with another content package, Integrated Financial Planning for SAP S/4HANA. This business content is also delivered with the business content network and covers all major financial planning processes. 

## Description

Follow the step-by-step instructions to complete the exercise.
1. For this exercise, the business content **Integrated Financial Planning for SAP S/4HANA** needs to be imported as a pre-requisite.
2. Navigate to **Files** in the main menu.
3. Type in HXM in the search field.
4. Click on the model **HXM Integrated Workforce Planning**.
<br>![](/exercises/ex7/images/07_0001.png)
5. Click on the **SAP_HR_COSTTYPE** to open the maintenance view for the dimension.
<br>![](/exercises/ex7/images/07_0002.png)
6. The dimension Cost Type has an attribute **GL_Account** which maps the cost type for HR planning to a GL account in the financial planning model. Make sure that you maintain the GL account attribute as shown in the screenshot.
<br>![](/exercises/ex7/images/07_0003.png)
7. Click on the back icon to navigate back to the search results.
<br>![](/exercises/ex7/images/07_0004.png)
8. Click on **SAP HXM Workforce Planning** to open the folder.
<br>![](/exercises/ex7/images/07_0005.png)
9. Click on the item **WFP – Overview page** to open the application in the analytics designer.
<br>![](/exercises/ex7/images/07_0006.png)
10. Select the item **hyperlink_publish** in the Outline window.
11. Click on **Designer** to open the Styling panel.
12. Make sure that the check box **Show this item at view time** is active.
<br>![](/exercises/ex7/images/07_0007.png)
13.	Click on the **fx** icon next to the **hyperlink_publish** element to open the script editor.
<br>![](/exercises/ex7/images/07_0007a.png)

14. Uncomment the lines 8 and 9 to activate the code.
15. As a result, the user will navigate to the application which transfers the plan data to the financial planning model.
<br>![](/exercises/ex7/images/07_0007b.png)
16. Click on the **Save** icon in the toolbar to save your changes.
<br>![](/exercises/ex7/images/07_0007c.png)

17. Click on **Run Analytic Application** to start the application.
<br>![](/exercises/ex7/images/07_0008.png)
18.	On the overview page, you will see the entry Publish **Result To Financial Plan for SAP S/4HANA**.
19.	Click on **Publish Result To Financial Plan for SAP S/4HANA** to open the application.
<br>![](/exercises/ex7/images/07_0009.png)
20.	In this application, you can derive the corresponding G/L accounts for the planned HR costs and transfer the data to the financial planning model.
<br>![](/exercises/ex7/images/07_0010.png)
21.	Add a filter by clicking on the **filter** icon at the top left corner of the page.
22.	Select **Company Code** from the list of available dimensions.
<br>![](/exercises/ex7/images/07_0011.png)
23.	From the member selector, pick **BestRun Germany**. Click on **OK** to confirm your selection.
<br>![](/exercises/ex7/images/07_0012.png)
24.	Click on **General Settings** to set some parameters for the data transfer to the financial plan.
<br>![](/exercises/ex7/images/07_0013.png)
25.	In the settings dialog, you can specify the source version in the WFP model as well as the planning level. In addition, you can define the target version in the financial planning model.
26.	Click on **OK** to confirm the settings.
<br>![](/exercises/ex7/images/07_0014.png)
27.	Click on **G/L Mapping** to derive the G/L accounts.
<br>![](/exercises/ex7/images/07_0015.png)
28.	Click on **OK** to confirm the mapping parameters and start the derivation.
<br>![](/exercises/ex7/images/07_0016.png)
29.	In the Cost Overview table, you will see the planned cost types together with the corresponding G/L accounts.
<br>![](/exercises/ex7/images/07_0017.png)
30.	Click on the button **PUBLISH TO P&L** to transfer the data to the financial planning model.
<br>![](/exercises/ex7/images/07_0018.png)
31.	Click on **OK** to confirm the settings and start the transfer.
<br>![](/exercises/ex7/images/07_0019.png)
32.	In the table **Financial Plan Overview** you can see the result of the transfer.
<br>![](/exercises/ex7/images/07_0020.png)


## Summary

You've now learned how you can integrate workforce planning with financial planning.

Continue to [Exercise 8 - Add additional cost types](../ex8/README.md)
