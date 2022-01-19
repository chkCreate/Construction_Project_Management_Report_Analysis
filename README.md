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

* Forms dashboard was to demonstrate the various types of data visuals out there for training purposes only. [Forms_Dashboard](<div class='tableauPlaceholder' id='viz1642567313126' style='position: relative'><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='2022-0118Forms_Dashboard&#47;Forms_Dashboard' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>                <script type='text/javascript'>                    var divElement = document.getElementById('viz1642567313126');                    var vizElement = divElement.getElementsByTagName('object')[0];                    if ( divElement.offsetWidth > 800 ) { vizElement.style.minWidth='420px';vizElement.style.maxWidth='100%';vizElement.style.minHeight='587px';vizElement.style.maxHeight=(divElement.offsetWidth*0.75)+'px';} else if ( divElement.offsetWidth > 500 ) { vizElement.style.minWidth='420px';vizElement.style.maxWidth='100%';vizElement.style.minHeight='587px';vizElement.style.maxHeight=(divElement.offsetWidth*0.75)+'px';} else { vizElement.style.width='100%';vizElement.style.height='2027px';}                     var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>).

* Tasks dashboard delves into an elevated analysis of the Task dataset. Visit it here: [Tasks_Dashboard](https://public.tableau.com/views/2022-0118Tasks_Dashboard/Tasks_Dashboard?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link)

    * The various high-interest filters such as 'Over Due', 'Priority', 'Status', and 'Types' of Tasks available in this dataset. The viewer can play around with the filters for an interactive discovery of the two visuals presented on the dashboard.

    * 'Tasks_Type Priority_2' visual explores the 'Types' (count indicate by size) and 'Priority' (marked by color) from when the were 'Created' to when the 'Status Changed'. Use the filters or highlight the desired criteria to track the progress.

    * 'Tasks_Type Priority' visual displays the higher 'Priority' items that increase in size with the count of 'Types'. Findings suggest that Quality and Safety Notices make up the majority of the higher priority and volume size of the Tasks datase.t

