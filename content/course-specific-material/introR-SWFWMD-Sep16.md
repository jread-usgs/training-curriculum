---
date: 2016-09-13
slug: introR-SWFWMD-Sep16
title: SWFWMD
menu:
  main:
    parent: Course Specific Material
    weight: 1
---
September 13th - 15th in Tampa, FL

### Installation

See [Before the Workshop](/intro-curriculum/Before) for information on what software should be installed prior to the course.

### Tentative schedule

**Day 1**

-   08:00 am - 09:00 am -- Instructors available for questions
-   09:00 am - 10:30 am -- [Introduction](/intro-curriculum/Introduction)
-   10:30 am - 10:45 am -- *Break*
-   10:45 am - 12:15 pm -- [Get](/intro-curriculum/Get)
-   12:15 pm - 01:15 pm -- *Lunch*
-   01:15 pm - 03:15 pm -- [Clean](/intro-curriculum/Clean)
-   03:15 pm - 03:30 pm -- *Break*
-   03:30 pm - 04:30 pm -- [Clean](/intro-curriculum/Clean) continued
-   04:30 pm - 05:00 pm -- End of day wrap-up

**Day 2**

-   08:00 am - 08:30 am -- Instructors available for questions
-   08:30 am - 09:30 am -- [Explore](/intro-curriculum/Explore)
-   09:30 am - 10:30 am -- [Analyze: Base](/intro-curriculum/Analyze)
-   10:30 am - 10:45 am -- *Break*
-   10:45 am - 12:00 pm -- Analyze: [dataRetrieval](https://owi.usgs.gov/R/dataRetrieval.html) and [RODBC](https://cran.r-project.org/web/packages/RODBC/RODBC.pdf)
-   12:00 pm - 01:00 pm -- *Lunch*
-   01:00 pm - 02:30 pm -- Visualize: [base](/intro-curriculum/Visualize/) or [ggplot2](/intro-curriculum/ggplot2/)
-   02:30 pm - 02:45 pm -- *Break*
-   02:45 pm - 04:00 pm -- Visualize: [base](/intro-curriculum/Visualize/) or [ggplot2](/intro-curriculum/ggplot2/) continued
-   04:00 pm - 04:30 pm -- End of day wrap-up

**Day 3**

-   08:00 am - 08:30 am -- Instructors available for questions
-   08:30 am - 09:30 am -- [Repeat](/intro-curriculum/Reproduce/)
-   09:30 am - 11:30 am -- Practice: [USGS R packages](/intro-curriculum/USGS/), projects (group/individual), or [additional topics](/intro-curriculum/Additional/)

### Data files

Download data from the [Data page](/intro-curriculum/data/).

### Additional resources

-   [RStudio cheatsheets](https://www.rstudio.com/resources/cheatsheets/) (data wrangling, visualization, shiny, markdown, RStudio, etc)
-   [USGS-R GitHub](https://github.com/USGS-R) (package source code + bug/feature reporting)
-   [USGS-R blog](https://owi.usgs.gov/blog/tags/r)

### Instructors

Lindsay Carr (<lcarr@usgs.gov>) -- *primary contact*

Joe Mills (<tmills@usgs.gov>)

John Stamm (<jstamm@usgs.gov>)

### Lesson scripts

Rather than having all of the code available on this page for you to copy and paste, we've decided to give you the complete R project folder instead. This way, all examples will work because they reference the correct filepaths when you have the project open (and demonstrate why sharing Project folders is more convenient/efficient than sharing individual code files - people don't need to go through and change relative filepaths).

Download the project zip folder at [this link](https://drive.google.com/open?id=0B54YFPSk4XN8cEM0VDdpNS1WcWc). You should see the download button on the topright of your browser after you click the link. *Unzip the file!!!* Open RStudio, then go to File &gt;&gt; Open Project..., select the `introductionR_swfwmd.Rproj` file, and click "open". Now you should be in the project, and `introductionR_swfwmd` should be in the topright of your RStudio screen.

The R lesson scripts are all in the folder `R`. The `data` folder has the raw and cleaned up versions of `intro_df` that we worked with (before/during the `Clean` lesson, and then after). The files for the example we went through on the final day with creating functions, executing a simple data analysis, and using these same steps in R Markdown are in the `workflow` folder.

Note that we have commented out the Excel fix for loading in dates for `course_NWISdata_cleaned` (where we had to do an extra step to convert the `dateTime` column to dates because Excel changed the format). That is because the data saved in this project has not been opened in Excel -- so don't open our csv's in Excel! The code for the Excel date conversion remains so that you can reference it in the future.
