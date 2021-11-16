# Exercise 2 - Configure Planning Parameters

In this exercise, you will learn how to set central planning parameters like midpoint salaries, allowances and other cost drivers for different planning levels.

## Description

Follow the step-by-step guide to complete the exercise.

1. Open the application **WFP – Overview Page**.

<br>![](/exercises/ex2/images/02_0001.png)

2. The Overview Page contains some KPI’s and allows to navigate to other applications:
    - Configuration
    - FTE & Cost Planning
    - Reports
3.	Click on **Application Configuration** to open the configuration.
<br>![](/exercises/ex2/images/02_0002.png)

4. In the main screen of the **Application Configuration**, you can adjust the values of the central planning parameters, e.g., midpoint salaries, merit increase or life insurance contributions. You can enter the values directly into the table.
<br>![](/exercises/ex2/images/02_0003.png)

5. At the top, you can click on **Learn More** to get more information.
<br>![](/exercises/ex2/images/02_0004.png)

6. You will be re-directed to the **SAP Community** pages for Enterprise Planning Content. There you can find more detailed information about the content Operational Workforce Planning.
<br>![](/exercises/ex2/images/02_0005.png)

7. In the Application Configuration, click on **Guide Me!** This will start a wizard which helps you setting up the planning parameters.
<br>![](/exercises/ex2/images/02_0006.png)

8. The central parameters which you can maintain are always related to a specific **version** and a **planning level**. The Planning Level defines the organizational granularity for which the planning parameters are stored and at which level you will plan.
9. In the drop-down box Version select **Aggregated_Plan** and for Planning Level select **Company Code / Business Unit**.
<br>![](/exercises/ex2/images/02_0007.png)

10.	In the second step, **Data Input**, of the wizard, you can define how the parameter values are initialized:
    - **Manual**: Parameter values are manually initialized
    - **Copy Data From**: Parameter values are copied from an existing version
11.	Click **Done**. The central assumptions data will be copied into your chosen plan level/version combination.
<br>![](/exercises/ex2/images/02_0008.png)

12. The input table for the parameters will be adjusted according to the settings.
13. Click on the filter icon to apply filters to the table.
<br>![](/exercises/ex2/images/02_0009.png)

14.	Select **Company Code** from the list of available dimensions.
<br>![](/exercises/ex2/images/02_0010.png)

15.	From the member selector, pick **BestRun Germany**. Click on **OK** to confirm your selection.
<br>![](/exercises/ex2/images/02_0011.png)

16.	The table is filtered according to the filter settings. You can expand the hierarchy node for the Date dimension and drill down to the quarters or periods.
<br>![](/exercises/ex2/images/02_0012.png)

17. Click on **External Workforce** to switch the view and maintain cost drivers for external workforce.
<br>![](/exercises/ex2/images/02_0012a.png)
18. The layout of the table is adjusted to include the dimension **Location** and only one measure for the total cost rate for external workers.
19.	Change some values in the table.
<br>![](/exercises/ex2/images/02_0012b.png)


20. Once you are done with your changes, you can click the **Confirm** button to publish your changes.
<br>![](/exercises/ex2/images/02_0013.png)
21. You will see a confirmation dialog which summarizes the main settings. Toggle-on **Initialise Plan Data After Publish** to populate the plan version with initial data.
22. Click **OK** to publish the version.
<br>![](/exercises/ex2/images/02_0014.png)
23. Click on the **Home** icon at the top left of the screen to return to the overview page.
<br>![](/exercises/ex2/images/02_0015.png)





## Summary

You've now learned how you can define central planning parameters.

Continue to [Exercise 3 - Aggregated External HC Plan ](../ex3/README.md)
