
1.	Open Power BI Desktop.

2.	If the getting started window opens, at the top-right of the window, click **X**.

   ![ws name.](media/8.1.png)
 
3.	To save the Power BI Desktop solution, on the **File** tab (backstage view), select **Save**.

4.	Save the file as **Sale Report** to an easy-to-remember location in your file system.


### **Subtask 2: Create a Live Connection**

In this task, you will create a live connection to the **Sale Analysis** dataset.

1. On the **Home** ribbon, from inside the **Data** group, click **Get Data**, and then select Power **BI Datasets**.

   ![ws name.](media/8.2.png)
 
2. In the **Select a Dataset** window, notice that the **Sale Analysis** dataset is endorsed as a promoted dataset.

3.	Select the **Sale Analysis** dataset.

   ![ws name.](media/8.3.png)
 
4.	Click **Create**.
   
   ![ws name.](media/8.4.png)
   
5.	In the status bar, at the right, notice the live connection status.

   ![ws name.](media/8.5.png)
 
6.	Save the Power BI Desktop solution.


## **Task 2: Develop the Report Layout**

In this task, you will develop a two-page report.

### **Subtask 1: Develop Page 1**

In this task, you will develop the first report page.


The completed report page will look like the following:

   ![ws name.](media/8.6.png)
 
1.	To rename the report page, at the bottom-left, double-click **Page 1**.

2.	Replace the text with **Profit Analysis**, and then press **Enter**.
 
   ![ws name.](media/8.7.png)
 
3.	To format the page, in the **Visualizations** pane, select the **Format** pane (paint roller icon).

   ![ws name.](media/8.8.png)
 
   *You’ll format many report elements in this lab to produce a professional report layout. To format an element, you’ll select it, and then access formatting options in this pane. Formatting options are organized into sections*.
   
4.	Expand the **Page Background** section.

   ![ws name.](media/8.9.png)
 
5.	Open the **Color** palette, click **Custom Color**, and set the custom color **C5C5C5**.

6.	Set the **Transparency** property to **0%**.

7.	Add a slicer to the page.

   ![ws name.](media/8.10.png)
 
8.	Position and size the slicer at the top-left of the report page.

   ![ws name.](media/8.11.png)
 
9.	In the **Fields** pane, expand the **Date** table, and then drag the **Year** field (not the **Year** level of the hierarchy) into the slicer.

   ![ws name.](media/8.12.png)
 
10. Ensure that the slicer is selected, and then open the **Format** pane.

11. Turn the **Shadow** property on.

    ![ws name.](media/8.13.png)
 
    *For a consistent style, you’ll be instructed to add shadow to all elements you add to the report*.
 
12. In the slicer, select **CY2012**.

    ![ws name.](media/8.14.png)
 
13. To create a new visual, first select an empty area of the report canvas.

14. To add a table visual to the report canvas, in the **Visualizations** pane, click the table visual icon.

    ![ws name.](media/8.15.png)
 
15. Position the table visual at the right of the slicer, and resize it to fill the remaining page space.

    ![ws name.](media/8.16.png)
 
16. Add the following fields to the table visual:

-	**Geography** table **State-Province** field
-	**Sale** table **Profit Amount** field
-	**Product** table **Profit % All Geography**

17. Apply the following table visual formats:

-	In the **Style** section, set the **Style** to **Bold Header**.
-	In the **Grid** section, increase the **Text Size** property to **16** pt.
-	Turn **Shadow** on.

18. To sort the table visual rows, click the **Profit % All Geography** column header to sort by descending profitability.

    ![ws name.](media/8.17.png)
 
19. Save the Power BI Desktop solution.
 
## **Subtask 2: Develop Page 2**

In this task, you will develop the second report page.

The completed report page will look like the following:

   ![ws name.](media/8.18.png)
 
1.	To duplicate the report page, at the bottom-left, right-click the **Profit Analysis** page, and then select **Duplicate Page**.

   ![ws name.](media/8.19.png)
 
   *Tip: Duplicating the page copies the formatting options. It can be quicker to duplicate than to reapply formats. And, it’s likely to result in more design consistency.*

2.	Rename the new page as **Sale Chord**.

   ![ws name.](media/8.20.png)
 
3.	To delete the table visual, select the visual, and then press the **Delete key**.
 
4.	To sync the slicers, on the **View** ribbon tab, from inside the **Show Panes** group, select **Sync Slicers**.
 
   ![ws name.](media/8.21.png)
   
5.	In the report page, select the **Year** slicer.

6.	In the **Sync Slicers** pane (located at the left), check both pages to sync.

   ![ws name.](media/8.22.png)
 
   *When a report user changes either **Year** slicer, the filter will propagate between these pages. Both slicers will remain in sync.*
   
7.	In the **Sync Slicers** pane, at the top-left, click **X**.

   ![ws name.](media/8.23.png)
 
8.	To import a custom visual, in the **Visualizations** pane, click the ellipsis (…), and then select **Get More Visuals**.

   ![ws name.](media/8.24.png)
 
9.	In the **Power BI Visuals** window, in the **Search** box, enter **Chord**, and then press **Enter**.

   ![ws name.](media/8.25.png)
 
10. When the **Chord** search result appears, click **Add**.

    ![ws name.](media/8.26.png)
 
11. When the custom visual imports, click **OK**.

12. In the **Visualizations** pane, notice that the chord custom visual sits in an area beneath the core Power BI visuals.

    ![ws name.](media/8.27.png)
 
13. Add a chord visual to the report page.
 
14. Position the chord visual at the right of the slicer, and resize it to fill the remaining page space.

    ![ws name.](media/8.28.png)
 
15. Configure the following visual field wells:

-	**From: Geography** table **Sales Territory** field
-	**To: Customer** table **Buying Group** field
-	**Values: Sale** table **Sale Amount** field

   ![ws name.](media/8.29.png)
 
16. Format the chord visual to add shadow.

17. Change the **Year** slicer values, and notice how the chord visual animates.

18. Hover the cursor over the outer segments and the internal chords to reveal tooltips describing inter-relationships between sales territories and buying groups.

19. Set the **Year** slicer back to **CY2012**.

20. Save the Power BI Desktop solution.


## **Task 3: Develop a Drill Through Page**

In this exercise, you will develop a drill through page.

### **Subtask 1: Develop a Drill Through Page**

In this task, you will develop a drill through page allowing report users to see detail data for a state-province.

The completed report page will look like the following:

   ![ws name.](media/8.30.png)
 
1.	Create a new report page by duplicating the **Sale Chord** page.

2.	Rename the new page as **State-Province Details**.

   ![ws name.](media/8.31.png)
 
3.	Remove the slicer and chord visual.
 
4.	From the **Fields** pane, in the **Geography** table, drag the **State-Province** field to the **Drill Through** section (beneath the **Visualizations** pane), into the well.

   ![ws name.](media/8.32.png)
 
5.	Apply a filter to the first state, **Alabama**.

   ![ws name.](media/8.33.png)
 
   *The filter will be applied when the report user drills through. You applied this filter now to help design the page for a single state.*
   
6.	At the top-left of the report page, notice the back arrow button.

   *The button was added automatically when you added a drill through filter. It allows report users to navigate back to where they drilled.*
   
7.	Select the button, and the in the **Visualizations** pane, turn the **Background** off.

   ![ws name.](media/8.34.png)
 
8.	Add a multi-row card visual to the report page.

   ![ws name.](media/8.35.png)
 
9.	Position and size the multi-row card visual at the top-left of the report page.

   ![ws name.](media/8.36.png)
 
10. Add the following five fields to the multi-row card visual:

-	**Geography** table **State-Province** field
-	**Sale** table **Quantity** field
-	**Sale** table **Sale Amount** field
-	**Sale** table **Profit Amount** field
-	**Product** table **Profit % All Geography** field

11. Apply the following formats:

-	In the **Data Labels** section, set the **Text Size** to **16** pt.
-	In the **Card Title** section, set the **Text Size** property to **20** pt.
-	Turn **Shadow** on.

   ![ws name.](media/8.37.png)
 
12. Add a line and clustered column chart visual to the report page.

    ![ws name.](media/8.38.png)
 
13. Position the line and clustered column visual at the right of the slicer, and resize it to fill the remaining page space.

    ![ws name.](media/8.39.png)
 
14. Configure the following field mappings:

-	**Shared Axis: Date** table **Month** field
-	**Column Values: Sale** table **Sale Amount** field

    ![ws name.](media/8.40.png)
 
15. To add a report-level measure, in the **Fields** pane, right-click the **Sale** table, and then select **New Measure**.

    ![ws name.](media/8.41.png)
 
    *A report-level measure can be added by the report author. It allows them to define complex summarization logic that’s not already defined in the model.*
    
16. In the formula bar, enter the following measure definition:
    ```
      DAX
        Profitability =
          DIVIDE(
	     SUM(Sale[Profit Amount]),
	   SUM(Sale[Sale Amount])
       )
       ```


    *The formula divides the sum of the **Profit Amount** column by the sum of the **Sale Amount** column.*
 
17. On the **Measure Tools** contextual ribbon tab, set the format to percentage.

    ![ws name.](media/8.43.png)
 
18. Add the **Profitability** measure to the **Line Values** well of the line and clustered column visual.

    ![ws name.](media/8.44.png)
 
19. Format the line and clustered column visual to add shadow.

    *The design of the drill through page is now complete.*

20. Right-click the **State-Province Details** page tab, and then select **Hide Page**.

    ![ws name.](media/8.45.png)
 
    *Report users won’t see the page tab, but they’ll be able to drill through to the page. You’ll now test the drill through experience.*
 
### **Subtask 2: Explore Drill Through**

In this task, you will explore the drill through experience.

1.	Select the **Profit Analysis** page.

2.	Ensure the **Year** slicer is set to **CY2012**.

3.	In the table visual, right-click any state, and then select **Drill Through > State-Province Details**.

   ![ws name.](media/8.46.png)
 
   *Drill through is available from any report visual that groups by the State-Province field.*
   
4.	In the drill through page, notice the state you drilled from is the title of the multi-row card visual.

   ![ws name.](media/8.47.png)
 
5.	Hover the cursor over the top-left corner of the line and clustered column chart visual, and then hover over the filter (funnel) icon.

   ![ws name.](media/8.48.png)
 
   *The tooltip reveals all applied filters.*

6.	Notice that the **Year** slicer value was passed to the drill through page, too.

7.	To return back to where you drilled from, at the top-left corner, while pressing the **Ctrl** key, click the back button.

   *When editing a report, you must press the **Ctrl** key when clicking buttons. If you don’t press the **Ctrl** key, the designer understands you’re selecting it so it can be configured.*
   
8.	Save the Power BI Desktop solution.

## **Task 4: Work with Bookmarks**

In this exercise, you will superimpose visuals on the drill through page. You’ll then create bookmarks and assign them to buttons. This design will allow the report user to determine which visual to display.

### **Subtask 1: Create a New Visual**

In this task, you will add a new visual to the drill through page.

1.	Select the **State-Province Details** page.

2.	Select the line and clustered column chart visual.

3.	To clone the visual, press **Ctrl+C**, and then press **Ctrl+V**.

4.	Position the cloned visual precisely over the top of the original visual.

5.	Modify the top visual field **Shared Axis** field mappings by removing the **Month** field, and then replacing it with the **Salesperson** table **Salesperson** field.

   ![ws name.](media/8.49.png)
 
6.	Format the visual data color by setting the **Default Color** to purple.

   ![ws name.](media/8.50.png)
 
### **Subtask 2: Create Bookmarks**

In this task, you will create two bookmarks to show or hide the superimposed visuals.

1.	On the **View** ribbon tab, from inside the **Show Panes** group, select **Bookmarks** and **Selection**.

   ![ws name.](media/8.51.png)
 
2.	In the **Selection** pane, notice there are two similarly named report elements.

   ![ws name.](media/8.52.png)
 
3.	Hover the cursor over each to reveal a tooltip describing their full title.

4.	Notice that one ends in “by Month”, and the other ends in “by Salesperson”.

5.	Determine which of the visuals groups by salesperson, and then click the **Hide** icon.

   ![ws name.](media/8.53.png)
 
6.	Verify that the “by Month” visual is now visible.

7.	In the **Bookmarks** pane, click **Add**.

   ![ws name.](media/8.54.png)
 
8.	To rename the bookmark, double-click **Bookmark 1**.

9.	Rename the bookmark as **By Month**, and then press **Enter**.

10. Click the ellipsis at the right of the bookmark, and then select **Data**.

    ![ws name.](media/8.55.png)
 
    *By selecting Data, you’re disabling the bookmark from capturing any applied filters. It means that when the bookmark is applied, it’ll use the filters applied by the report user.*
    
11. Click the ellipsis again, and then select **Update**.

    ![ws name.](media/8.56.png)
 
12. In the **Selection** pane, unhide the visual, and then hide the visual that groups by month.

13. Create a second bookmark, and then name it **By Salesperson**.

14. Configure the bookmark to not override filters (turn off **Data**), and then update the bookmark.

15. Verify there are two bookmarks.

    ![ws name.](media/8.57.png)
 
16. Close the **Selection** pane.

    ![ws name.](media/8.58.png)
 
17. Close the **Bookmarks** pane.

    ![ws name.](media/8.59.png)
 
 
### **Subtask 3: Add Buttons**

In this task, you will add two buttons to the report page, and then configure each to select a bookmark.

1.	On the **Insert** ribbon tab, from inside the **Elements** group, click **Buttons**, and then select **Blank**.

   ![ws name.](media/8.60.png)
 
2.	Position and size the button as follows:

3.	Position and size the button so that it is directly beneath the multi-row card visual and it is the same width.

   ![ws name.](media/8.61.png)
 
4.	In the **Visualizations** pane, apply the following button formats:

-	Set the **Button Text** section to **On**.
-	Expand the **Button Text** section, and then set the **Button Text** to **By Month**.
-	Set the button text **Font Color** to **Black**.
-	Set the button text **Text Size** to **16** pt.
-	Set the **Fill** section to **On**.
-	Set the fill **Fill Color** to **Blue**.
-	Set the **Shadow** section to **On**.
-	Set the **Action** section to **On**.
-	Set the action **Type** to **Bookmark**.
-	Set the action **Bookmark** to **By Month**.

5.	Clone the button, and then position it directly beneath the first button.

   ![ws name.](media/8.62.png)
 
6.	Modify the button formats, as follows:

-	Set the **Button Text** to **By Salesperson**.
-	Set the fill **Fill Color** to **Purple**.
-	Set the action **Bookmark** to **By Salesperson**.
 
7.	Verify that the buttons looks like the following:
 
   ![ws name.](media/8.63.png)
 
8.	Test each button by pressing the **Ctrl** key and clicking a button.

 
   
## **Task 5: Publish the Report**

In this exercise, you will prepare the report for publication, and then publish it to Power BI.


### **Subtask 1: Prepare the Report**

In this task, you will prepare the report for publication.

1.	On the **State-Province Details** page, ensure the **By Month** visual is displayed.

2.	Select the **Profit Analysis** page.

3.	Ensure the **Year** slicer is set to **CY2012**.

   *It’s important to select the initial page and reset filters just before publishing the report. It will become the report state when report users first open the report.*

4.	Save the Power BI Desktop solution as **Sale Report**.


### **Subtask 2: Publish the Report**

In this task, you will publish the report to Power BI.

1.	On the **Home** ribbon tab, from inside the **Share** group, click **Publish**.

   ![ws name.](media/8.64.png)

 
2.	If prompted to save changes, click **Yes**.

3.	In the **Publish to Power BI** window, select the lab workspace (do not use **My Workspace**).

4.	Click **Select**.

   ![ws name.](media/8.65.png)
 
5.	When publication has completed, click **Got It**.

6.	Close Power BI Desktop.
 

### **Subtask 3: Explore the Report**

In this task, you will explore the report to determine root cause for low-profit earning state.

1.	Switch to the Power BI web session.

2.	Switch to the workspace where you published the report.

3.	Open the **Sale Report**.

4.	At the left, notice there are only two pages.

   ![ws name.](media/8.66.png)
 
   *The drill through page was hidden.*
   
5.	Set the **Year** slicer to **CY2014**.

6.	Understand that the page refreshed quickly because Power BI is querying the aggregation.

7.	To see low-profit states, modify the table sort to **Profit % All Geography** ascending.

8.	To understand **Hawaii** sales in more detail, right-click **Hawaii**, and then drill through to the details page.

9.	Review the monthly sales.

10. Click the **By Salesperson** button, and then review the result by salespeople.

### Summary

In this exercise, you used Power BI Desktop to connect to the **Sale Analysis** dataset published in **Exercise 06**. You then developed a multi-page report, which included synced slicers, a custom visual, page drill through, a report-level measure, bookmarks, and buttons. You then finalized the exercise by publishing the report to the Power BI service, and exploring it in the service.
