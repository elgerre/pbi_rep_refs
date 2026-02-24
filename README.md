# PBI RepRefs
Power BI Report (Template) to check referenced columns and measures in other PBI reports

# How to use
1. Save your report as a .pbip file with the pbir enhanced metadata option enabled (https://learn.microsoft.com/en-us/power-bi/developer/embedded/projects-enhanced-report-format)
2. This should create a .pbip file as well as a subfolder 'Your Report Name'.Report
3. In this subfolder navigate to the "pages" folder and copy the path, should look like this: 'Your Report Name'.Report\definition\pages
4. Enter this path as the "Folder Path" parameter value of the template, leave all other parameters as they are
5. This should now load everything automatically. You can then modify the report and customise it

# Notes
So far the extracted information is fairly minimal. The "Visual Query Reference" field doesn't show all potential refrences on a visual, so I created additional queries to get other things, like Columns and Rows on a PivotTable visual (a matrix in PBI). Because of this I will add more information one visual type at a time. So far, just using the PageID+PageTitle and VisualID+VisualType+VisualTitle fields should already provide a good overview on how many visuals there are and what a specific page might be used for.