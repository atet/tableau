# [atet](https://github.com/atet) / [learn](https://github.com/atet/learn) / [tableau](https://github.com/atet/learn/tree/master/tableau)

![.img/logo_tableau.png](.img/logo_tableau.png)

# Introduction to Tableau

* Estimated time to completion: 15 minutes.
* This quick introduction to [Tableau software](https://en.wikipedia.org/wiki/Tableau_Software) is meant to cover only the absolute necessary material to get you up and running in a minimal amount of time.
* You are here because you want to use Tableau to visualize data from a data source (e.g. database, spreadsheet, etc.).
* We will be using [Tableau Public (Free)](https://public.tableau.com/en-us/s/) to perform basic operations, advanced material is not covered here.

--------------------------------------------------------------------------------------------------

### Table of Contents

#### Introduction
* [1. Installation](#1-installation)
* [2. Example Data](#2-example-data)
* [3. Loading Data](#3-loading-data)
* [4. Tabs](#4-tabs)
* [5. Your First Visualization](#5-your-first-visualization)
* [6. Saving and Publishing](#6-saving-and-publishing)
* [7. Customization](#7-customization)

#### Supplemental
* [Limitations of Tableau Public](#limitations-of-tableau-public)
* [Acknowledgements](#acknowledgements)

--------------------------------------------------------------------------------------------------

### 1. Installation

* Download and install Tableau Public from: [https://public.tableau.com/en-us/s/download](https://public.tableau.com/en-us/s/download)
* I am using Tableau Public version 2019.3 for this tutorial.
* You must sign up for a free account with Tableau Public (https://public.tableau.com) to save and publish your work.
   * NOTE: A regular Tableau account will not work with Tableau Public, they are two separate accounts.

#### After downloading and installing Tableau Public and registering for an account, you should be able to publish your first Tableau visualization within the next 10 minutes.

[Back to Top](#table-of-contents)

--------------------------------------------------------------------------------------------------

### 2. Example Data

* We will use a small dataset of vehicles as an example[[1]](#acknowledgements).
* Click here for the dataset (right-click and "Save as..." then save as _mtcars.csv_): [https://raw.githubusercontent.com/atet/learn/master/tableau/data/mtcars.csv](https://raw.githubusercontent.com/atet/learn/master/tableau/data/mtcars.csv)
* This Comma Separated Values (CSV) file contains 32 records of vehicles and 12 attributes describing them (e.g. "id" = name, "mpg" = miles per gallon, etc.):

![.img/step02.png](.img/step02.png)

[Back to Top](#table-of-contents)

--------------------------------------------------------------------------------------------------

### 3. Loading Data

* Open Tableau Public.
* On left-hand side, click on "Text file".
* Navigate to where you saved _mtcars.csv_ and open it.

![.img/step03.png](.img/step03.png)

[Back to Top](#table-of-contents)

--------------------------------------------------------------------------------------------------

### 4. Tabs

* Once the _mtcars.csv_ data is loaded, you will be looking at the Source Data tab.
* Navigate to worksheet **Sheet1** at the bottom to make our first visualization.

![.img/step04.png](.img/step04.png)

[Back to Top](#table-of-contents)

--------------------------------------------------------------------------------------------------

### 5. Your First Visualization

* Tableau has organized the data on the left-hand side as **Dimensions** or **Measures**.
* The 32 individual records are represented by just the attribute's column name here for simplicity.
* This worksheet is where visualizations are made.

![.img/step05a.png](.img/step05a.png)

* Let's make a **scatter plot** to explore the relationship between a vehicle's weight ("wt") and its fuel efficiency ("mpg").
* Drag "wt" into Columns.

![.img/step05b.png](.img/step05b.png)

* Drag "mpg" into Rows.
* Tableau automatically made a useless visualization by using the _sum_ of "wt" and "mpg" (which results in a single data point).
* **This is not how we wanted to visualize this**: Right-click on both "wt" and "mpg" and change from *Measure (Sum)* to *Dimension*.
* After those changes, Tableau has automatically resized the window to fit all 35 data points.

![.img/step05c.png](.img/step05c.png)

[Back to Top](#table-of-contents)

--------------------------------------------------------------------------------------------------

### 6. Saving and Publishing

* Tableau Public will only allow you to save your analyses and visualization to their public cloud (everyone can see your work). This is the only option for the free Tableau Public software.
* Go to "Save to Tableau Public As..."
* A window will pop up to log into your account if you have not done so already.

![.img/step06a.png](.img/step06a.png)

* Once you save, your work will automatically be published to your cloud account and accessible to the public.
* My example here has been published to: [https://public.tableau.com/profile/atet.kao#!/vizhome/mtcars_15711875697030/Sheet1?publish=yes](https://public.tableau.com/profile/atet.kao#!/vizhome/mtcars_15711875697030/Sheet1?publish=yes)

![.img/step06b.png](.img/step06b.png)

[Back to Top](#table-of-contents)

--------------------------------------------------------------------------------------------------

### 7. Customization

* Tableau will allow you to add a title, rename axes, change colors, add a trend line, etc.

![.img/step07.png](.img/step07.png)

[Back to Top](#table-of-contents)

--------------------------------------------------------------------------------------------------

### 8. Experiment

* Play around with the software, make new worksheets with interesting visualizations.
* Find new data on the internet and learn new ways to use Tableau.
* If you are an Excel and/or R user, think about how your analysis workflow would be different using Tableau.
* Resources:

Description | Link
--- | ---
Sample Data | [https://public.tableau.com/en-us/s/resources?qt-overview_resources=1#qt-overview_resources](https://public.tableau.com/en-us/s/resources?qt-overview_resources=1#qt-overview_resources)
How-To Videos | [https://public.tableau.com/en-us/s/resources?qt-overview_resources=0#qt-overview_resources](https://public.tableau.com/en-us/s/resources?qt-overview_resources=0#qt-overview_resources)

[Back to Top](#table-of-contents)

--------------------------------------------------------------------------------------------------

### Limitations of Tableau Public

* Tableau Public is a free version of the subscription-based Tableau Desktop and does not have full functionality. Limitations include:
   * Data can only be uploaded as a spreadsheet (e.g. Excel files). Database connections are disabled.
   * Limit of 10 million rows.
   * Automation is disabled.
   * Everything is saved/published to their cloud and can be seen by the public. Local "save to desktop" is disabled.
* For a details of limitations: [https://community.tableau.com/docs/DOC-9135](https://community.tableau.com/docs/DOC-9135).

[Back to Top](#table-of-contents)

--------------------------------------------------------------------------------------------------

### Acknowledgements

1. mtcars data set from R: [Henderson and Velleman (1981), Building multiple regression models interactively. Biometrics, 37, 391–411.](https://stat.ethz.ch/R-manual/R-devel/library/datasets/html/mtcars.html)

[Back to Top](#table-of-contents)

--------------------------------------------------------------------------------------------------

<center>Copyright © 2019-∞ Athit Kao, <a href="http://www.athitkao.com/tos.html">Terms and Conditions</a></center>