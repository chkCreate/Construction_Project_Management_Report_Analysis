# Construction_Project_Management_Report_Analysis

## Background 
Building construction projects generate huge amounts of data that can be leveraged to understand improvements in efficiency, cost savings, etc. There are several digital apps on the market that helps construction project managers keep track of the details of the process.  Analyze building construction projects using Python, perform statistical analyses, and present results in Tableau.

## Data Source
* Source data from [kaggle](https://www.kaggle.com/claytonmiller/construction-and-project-management-example-data).

This is a simple data set from a number of construction sites generated from project management field apps that are used for quality, safety and site management.

Essentially there are two files in this data set:
* Forms – generated from check list for quality/safety/site management
* Tasks – which is an action item typically used for quality snags/defects or safety issues.

### Acknowledgements
This data set was donated by Jason Rymer, a BIM Manager from Ireland who was keen to see more construction-related data online to be used to learn.

License CC BY-NC-SA 4.0

## Data Cleaning
* Extracted data from [zipfolder](Raw_Data/archive (1)), which had two csv files detailed above.

* Utilized python scripts (pandas, numpy) on Jupyter notebook to review and transform data types, normalize common categories per professional experience in AEC industry, and exported the two excel data files into folder [Cleaned_Data](Cleaned_Data).

## Data Visualization & Findings
* Tableau was selected for this project for showcase, but similar visualiazations can be performed in Power BI, and other BI tools as well.

* Forms dashboard was to demonstrate the various types of data visuals out there for training purposes only. [Forms_Dashboard](https://public.tableau.com/views/2022-0118Forms_Dashboard/Forms_Dashboard?:language=en-US&:display_count=n&:origin=viz_share_link).


![Forms.png](Readme_Images/Forms.PNG)


* Tasks dashboard delves into an elevated analysis of the Task dataset. Visit it here: [Tasks_Dashboard](https://public.tableau.com/views/2022-0118Tasks_Dashboard/Tasks_Dashboard?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link)

    * The various high-interest filters such as 'Over Due', 'Priority', 'Status', and 'Types' of Tasks available in this dataset. The viewer can play around with the filters for an interactive discovery of the two visuals presented on the dashboard.

    * 'Tasks_Type Priority_2' visual explores the 'Types' (count indicate by size) and 'Priority' (marked by color) from when the were 'Created' to when the 'Status Changed'. Use the filters or highlight the desired criteria to track the progress.

    * 'Tasks_Type Priority' visual displays the higher 'Priority' items that increase in size with the count of 'Types'. Findings suggest that Quality and Safety Notices make up the majority of the higher priority and volume size of the Tasks datase.t


![Tasks.png](Readme_Images/Tasks.PNG)


---

## Technical Elements

* Employed Python pandas and numpy skills, and data cleansing methods.

* Used Tableau to demonstrate exploratory insights.


## Notes

* As this data was sourced from Kaggle and there was no interview with the author of the data to gain a deeper understanding of the data such as 'Ref', 'Project', 'Location', and other data that was potentially masked as boolean code for anynomity, it would be interesting to have that level of data understanding to work on more analyses.

* If the two sets of files had unique values that formed a union for cross data insights, that would have been interesting to pursue as well.