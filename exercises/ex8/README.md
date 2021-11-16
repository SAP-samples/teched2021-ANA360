# Exercise 8 - Add additional cost types

In this exercise, you will learn how you can adjust the content to your individual needs. As an example you will add an additional cost type to your model and enhance the cost calculation to take this new cost type into consideration.

## Description

Follow this step-by-step guid to complete the exercise.


1. In the main menu, click on **Files**.
2. Type in HXM in the **search bar** to see the related objects in the file repository.
3. Click on the model **HXM Integrated Workforce Planning**.
<br>![](/exercises/ex8/images/08_0001.png)
4. In the Model Structure, click on the dimension **SAP_HR_COSTTYPE** to open the master data maintenance view.
<br>![](/exercises/ex8/images/08_0002.png)
5. Add an additional entry at the bottom of the table with the following information:
    - Member ID: **TRAINING**
    - Description: **Training**
    - Hierarchy: **COMPANY_COST**
    - GL_Account: **6140000**
    - Row_Source: **SAC**
<br>![](/exercises/ex8/images/08_0003.png)
6. Click on the hierarchy icon in the toolbar to open the hierarchy view.
<br>![](/exercises/ex8/images/08_0004.png)
7. If you expand the hierarchy tree, you should see the new cost type **TRAINING** as a child element of **Company Costs Sum**.
<br>![](/exercises/ex8/images/08_0005.png)
8.	Click on the hierarchy icon again to close the hierarchy view.
<br>![](/exercises/ex8/images/08_0006.png)
9.	Click on the back icon to navigate back to the Model Structure workspace.
<br>![](/exercises/ex8/images/08_0007.png)
10.	Switch to the Calculations workspace by selecting the workspace from the drop-down box at the top left.
11.	Add another calculated measure by clicking the **+**-icon.
<br>![](/exercises/ex8/images/08_0008.png)
12.	Provide the information for the new calculated measure:
    - Name: **CM_TrainingCosts**
    - Description: **Training Costs Absolute Rate**
    - Aggregation Type: **Sum**
    - Scale: **Thousand**
    - Decimal Places: **0**
13.	This measure will serve as a restricted measure for the training costs.
<br>![](/exercises/ex8/images/08_0009.png)
<br>![](/exercises/ex8/images/08_0010.png)
14.	In the formula window, enter the formula to define the restricted measure:
    ``RESTRICT( [Rate_Absolute], [d/SAP_HR_COSTTYPE] = “TRAINING”)``
<br>![](/exercises/ex8/images/08_0011.png)
15. Click on the **Save** icon in the toolbar to save the model changes.
<br>![](/exercises/ex8/images/08_0012.png)
16. Next, you need to adjust the calculation logic for cost calculation to include the cost for training. Click on **Data Actions** in the main menu.
<br>![](/exercises/ex8/images/08_0013.png)
17.	Click on the entry for the data action **Calculation of Costs for Plan Level PL2 in Aggregated Planning**.
**Note**: PL2 refers to the Planning level Company Code / Business Unit.
<br>![](/exercises/ex8/images/08_0014.png)
18.	The design time for defining data actions is opened. This data action has one step of type Advanced Formula. The script of this steps recalculates the total workforce cost based on planned head count and central cost drivers.
<br>![](/exercises/ex8/images/08_0015.png)
19.	At the end of the existing script, add the code snippet you see in the screenshot. You can also find this as a text file in the download section of the session.
20.	Click on **Validate** to check that the script is correct.
<br>![](/exercises/ex8/images/08_0016.png)
21.	If there are no mistakes, the system will prompt **No errors found**.
<br>![](/exercises/ex8/images/08_0017.png)
22.	Click on the **Save** icon in the toolbar to save your changes.
<br>![](/exercises/ex8/images/08_0018.png)
23.	Click on **Files** in the main menu.
24.	Type in **HXM** in the search bar to show the relevant objects.
25.	Click on the folder **SAP HXM Workforce Planning** to open the folder.
<br>![](/exercises/ex8/images/08_0019.png)
26.	Click on the analytic application **WFP – Central Assumptions** to open the app in the analytics designer.
<br>![](/exercises/ex8/images/08_0020.png)
27.	In the Outline view, click on the icon **fx** next to the script object named **configureTables**.
<br>![](/exercises/ex8/images/08_0021.png)
28.	The script editor is opened. Adjust line 7 in the script to include the item **CM_TrainingCosts** in the list of measures. 
29.	Make sure that you insert commas in an appropriate way to get a valid list.
30.	This list of measure names will be used to set the filters of the table. As a result, you will see the measure to plan the average amount of per-employee training expenses.
<br>![](/exercises/ex8/images/08_0022.png)
31.	Click on the **Save** icon in the toolbar.
<br>![](/exercises/ex8/images/08_0023.png)
32.	Click on **Run Analytic Application** to start the app.
<br>![](/exercises/ex8/images/08_0024.png)
33.	Click on the **filter** icon at the top left corner of the page and select **Company Code** from the list of available dimensions.
<br>![](/exercises/ex8/images/08_0025.png)
34.	Select BestRun Germany to filter the data shown in the application.
<br>![](/exercises/ex8/images/08_0026.png)
35.	Click on the button **General Settings**.
<br>![](/exercises/ex8/images/08_0027.png)
36.	Select the version **Aggregated_Plan** and the planning level **CompanyCode / BusinessUnit**.
37.	Click on Done to confirm your selection.
<br>![](/exercises/ex8/images/08_0028.png)
38.	Scroll the table to see the column **Training Costs Absolute Rate**.
39.	Enter some values.
<br>![](/exercises/ex8/images/08_0029.png)
40.	Click on **Confirm** to publish your plan version.
<br>![](/exercises/ex8/images/08_0030.png)
41.	Click on the **Home** icon to navigate to the Overview page.
<br>![](/exercises/ex8/images/08_0031.png)
42.	On the Overview page, click on **Aggregated Internal HC Plan** to open the application for aggregated planning.
<br>![](/exercises/ex8/images/08_0032.png)
43.	In the planning application, set the filter for the dimension **Company Code** to **BestRun Germany**.
44.	Click on the button **General Settings**. 
<br>![](/exercises/ex8/images/08_0033.png)
45.	Select **Company Code, Business Unit** as the planning level.
46.	Click on **Done** to confirm your selection.
<br>![](/exercises/ex8/images/08_0034.png)
47.	Click on the button **Calculate Costs** to recalculate the costs and include training expenses.
<br>![](/exercises/ex8/images/08_0035.png)
48.	In the Cost Overview table, drill down in the dimension Plan Cost Type and check that you can see a new line **Training**.
<br>![](/exercises/ex8/images/08_0036.png)


## Summary

You've now learned how you can adjust the business content to your individual requirements.

You can continue your learning about SAP Analytics Cloud by visiting the [SAP Community](https://community.sap.com/topics/cloud-analytics) pages.

