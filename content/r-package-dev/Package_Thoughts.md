---
author: Laura DeCicco
date: 9999-11-30
slug: packages
title: What Is a Package?
image: img/main/intro-icons-300px/r-logo.png
menu:
  main:
    parent: R Package Development
    weight: 5
---
By the end of the R-Package development course, the act of creating a package should be considered almost trivial. This lesson is intended to give developers topics to consider to decide if a group of work would make a thoughtful package.

Lesson Objectives
-----------------

1.  Distinguish scripts and packages.
2.  Compare benefits and challenges of package creation.
3.  Identify alternatives to packages.
4.  Recall USGS and DOI policies related to publishing and maintaining code.

Packages ARE Great!
-------------------

Packages are essentially a set of scripts that define functions. These functions can communicate to create powerful workflows. A simple install command can unlock a ton of functionality, and can simplify how you share your workflows.

There are a great many reasons to make an R package:

-   The "fundamental units of reproducible R code" (Hadley)
-   "Allow for easy, transparent and cross-platform extension of the R base system" (Leich)
-   Easy to distribute and share
-   Transparent workflows
-   Includes documentation
-   Can bundle data
-   Can bundle manuscripts
-   Good platform for collaboration, by enforcing standards and tests coverage

It **is** easy and convenient to create an R-package. So why is this course 4 days? There are many best-practices that will be taught along with the mechanics of building a package. This will greatly improve the odds that the package:

-   Works
-   Works in the future
-   Is user-friendly
-   Has a clear line of communication with users
-   Has a clear process for updating, fixing bugs

Considerations
--------------

We fully expect you leave this workshop with the information, tools, and practice to create and maintain a high-quality R-package. One of your first steps to creating a package is to carefully consider whether or not it makes sense to create a package. Things to think about:

### Does it already (mostly) exist?

As of May 4th, 2017...there were 10,547 packages available on CRAN, and more available on other repositories (GRAN, Bioconductor), and still more available exclusively on Github. It is clearly impossible to know the content and scope of every package. But, it is beneficial to do some investigation before beginning work on your package. If someone has already put in the effort to make a high-quality package, and it has 90% of the functionality you need, consider using that package. Perhaps you contribute the remaining 10% to that package.

The techniques taught in this workshop will be important for both creating your own package, and contributing to other packages. The skills demonstrated in this curriculum are currently common techniques and workflows for many open-source projects, not just USGS.

### Does the functionality outweigh the overhead of creating a package?

We **will** show that it's not too much work to create a package, but there still is some overhead to the workflow.

### Are there resources to maintain the package?

This is especially true if the package was going to be submitted to CRAN, but still a consideration for any package that is distributed. R versions increase, packages we depend on change, users find bugs and strange edge-cases, and new users bring enthusiasm for enhancements. All of these things take time. Unfortunately, we cannot always count on the community rallying around our package to do these tasks (it **could** happen....and we will show you techniques to encourage outside users to contribute, and testing techniques to ensure those contributes are safe).

If you submit your package to CRAN, you **have** to take care of new errors that arise from R or package dependencies updates. If you don't, the package will eventually be removed from CRAN.

### USGS Software Release Policy

When developing an R-package as a USGS employee, it is also important to understand the policies of the USGS.

[Federal Source Code](https://sourcecode.cio.gov/)

[USGS Software Release](https://www2.usgs.gov/usgs-manual/im/IM-OSQI-2016-01.html)

R-package development can be done in the open, for example on github. There needs to be a disclaimer on the readme and package-startup, this will be addressed in the next section.

A package is officially released with an accompanying peer-reviewed journal article or USGS-report. Once this has been approved and published, the package can remove the disclaimer on the package-startup. This is when it is acceptable to submit a USGS package to CRAN. USGS policy require that all software be available via an ".gov" server. Therefore, a package cannot only be available via CRAN. Therefore, we have the "US Geological Survey R Archive Network" - [GRAN](https://owi.usgs.gov/R/gran.html).

Packages can be available on GRAN, without having an accompanying published paper as long as they retain the disclaimer, and follow the guidelines listed [here](https://owi.usgs.gov/R/gran.html).

### Scripts and Blogs

"if all you have is a hammer, everything looks like a nail"...There are other ways to share workflows and code. If you don't want to be on the hook for answering questions, generalizing workflows, fixing bugs, consider the alternatives. Sharing a script with collaborators can be an acceptable process. Many of the techniques presented in this workshop will carry over to general best-practices for writing and sharing scripts as well.

`Rmarkdown` has made the act of bundling code, text, and figures a seamless process as well. If you have a particularly interesting topic or workflow you would like to share, consider putting it together via `Rmarkdown`. There are many ways to then share the bundled work. You could share a complied html file, a pdf file, you could post it as a blog.

Other useful resources
----------------------

There is no shortage of resources on R developers documenting how to create a package.

-   [Hadley's Creating a package](http://r-pkgs.had.co.nz/)
-   [Leisch's Creating a package](https://cran.r-project.org/doc/contrib/Leisch-CreatingPackages.pdf)
-   [Ripley's Creating a package](http://portal.stats.ox.ac.uk/userdata/ruth/APTS2012/Rcourse10.pdf)
-   [Broman's Creating a package](http://kbroman.org/pkg_primer/)
-   [Parker's Creating a package](https://hilaryparker.com/2014/04/29/writing-an-r-package-from-scratch/)
-   [Creating Environmental Tools](https://www.fba.org.uk/journals/index.php/IW/article/viewFile/889/675)
-   [Kaushik's Creating a package](https://www.analyticsvidhya.com/blog/2017/03/create-packages-r-cran-github/?utm_content=bufferd99fb&utm_medium=social&utm_source=twitter.com&utm_campaign=buffer)
-   [Chung's Creating a package](http://tinyheero.github.io/jekyll/update/2015/07/26/making-your-first-R-package.html)
-   [Best Practices for APIs](https://cran.r-project.org/web/packages/httr/vignettes/api-packages.html)
