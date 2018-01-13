> ![](media/image1.jpeg){width="7.124305555555556in"
> height="1.7805555555555554in"}

![](media/image2.png){width="1.0694444444444444in"
height="0.4027777777777778in"}

> **Lab 3 – The High Powered Integrated Analytics System for Data
> Science**
>
> *Modified and Presented by:*
>
> *Paulinda Pangaldan*
>
> *Original Asset developed by:*
>
> *IBM NA Big Data Science Technical Team *
>
> **Contents**
>
> **INTRO IBM DATA SCIENCE EXPERIENCE LOCAL ON IBM INTEGRATED ANALYTICS
> SYSTEM** **3**
>
> PART 1 JUPYTER NOTEBOOK THAT PREDICTS OUTDOOR EQUIPMENT PURCHASES 3
>
> PART 2 USING THE MACHINE LEARNING BUILDER 6

Intro IBM Data Science Experience Local on IBM Integrated Analytics System
==========================================================================

> IBM Data Science Experience (DSX) Local is an out-of-the box on
> premises enterprise solution for data scientists and data engineers.
> It offers a suite of data science tools that are integrated with
> proprietary IBM technologies. It also seamlessly integrates with
> RStudio, Spark, Jupyter and Zeppelin notebook technologies. The
> intuitive user interface provides a collaborative Projects space for
> teams and individuals to reduce the time to value.

Part 1 Jupyter Notebook that Predicts Outdoor Equipment Purchases
-----------------------------------------------------------------

> This part of the lab will import a Jupyter notebook that will predict
> product line purchases based on a consumer’s gender, age, marital
> status and job. This notebook will show you how to load and explore
> data, create a machine learning model, persist the model, predict
> locally and visualize, deploy and score the model.

a)  Open your browser and navigate . You will be assigned a group number
    and team number. Each group will have a different web link. Use your
    ‘team\#\#’ with a password of ‘sailfish\#\#’, where \#\# is your
    team number. Example: username: team01 password: sailfish01

> Group \#1
> <https://amazingkalam.bluedemos.skytapdns.com/auth/login/login.html>
> to access the DSX Local sign in screen.
>
> ![](media/image3.tiff){width="6.80625in" height="3.475in"}

a)  From this point on, each group will have the same content. After a
    successful sign in, the following screen will appear

    -   Sample Notebooks

![](media/image4.tiff){width="6.5in" height="3.9680555555555554in"}

-   Click the ‘More’ button on the top right to get additional Community
    Notebooks. Please take a few moments to view the various assets
    available to get started quickly.

> ![](media/image5.jpeg){width="7.120833333333334in"
> height="3.313888888888889in"}

a)  Now click on the hamburger icon ![](media/image6.png){width="0.5in"
    height="0.36944444444444446in"} on the top left, then click on
    ‘Projects’ and ‘View all Projects’.

b)  ![](media/image7.png){width="7.120833333333334in"
    height="1.2243055555555555in"}Click on ‘create project’.

c)  Then enter your team name, ‘Team\#\#’ for ‘Name’ and click on
    ‘Create’. Note: Project names are unique. If ‘teamxx’ already exist,
    create a different name. Be sure you remember the new project name .

![](media/image8.jpeg){width="3.74375in" height="2.4743055555555555in"}

> Sample screen
>
> ![](media/image9.tiff){width="3.6395833333333334in"
> height="2.822516404199475in"}

a)  Create a notebook’ from the pull down in the top right ‘+’ icon.
    Click on ‘Create’

> ![](media/image10.jpeg){width="4.1375in"
> height="1.2708333333333333in"}

a)  In the ‘Create Notebook’ page, click on ‘From URL’, then enter
    ‘DSXLocalSailfish’ for the ‘Name’, select ‘Jupyter’ for ‘Tool’, and
    enter the following for the ‘Notebook URL’.
    <https://raw.githubusercontent.com/pepangaldan/DSXLabNotebook/master/DSXLocalSailfish-20180109.ipynb>

    ![](media/image11.jpeg){width="4.997222222222222in"
    height="3.7604166666666665in"}

    *Backup Github site:*

    *https://raw.githubusercontent.com/dxkikuchi/DSX/master/DSXLocalSailfish/DSXLocalSFBU.ipynb
    *

b)  ![](media/image13.jpeg){width="7.120833333333334in"
    height="2.720833333333333in"}This will import a Jupyter notebook
    from GitHub into your DSX Local environment.

c)  Please walk through the notebook by reading and executing the code
    cells to understand what is being accomplished.

d)  

Part 2 Using the Machine Learning Builder
-----------------------------------------

> The following will walk through the steps to use the machine learning
> builder wizard.

a)  Click on the hamburger icon on the top left and select ‘Projects’
    then your team project, ‘TeamXX’.

![](media/image14.png){width="7.555555555555555in"
height="4.029861111111111in"}

a)  First create a data source that will be recognized by the machine
    learning builder. Click on ‘Data sources’ from the above screen

b)  ![](media/image16.jpeg){width="7.120833333333334in"
    height="1.5604166666666666in"}Click on ‘add data source’ and you
    will see this screen

c)  On the first part of this screen enter: ‘GOSales’ for the ‘Data
    Source Name’

> ‘Remote Data from DB2 Warehouse on Cloud’ for Description

a)  dashDB for the ‘Data Source Type’

> jdbc:db2://dashdb-entry-yp-dal09-09.services.dal.bluemix.net:50000/BLUDB
> for the ‘JDBC URL’ dash7268 for the ‘Username’
>
> mV@\$e7q4RPzL for the ‘Password’ and Keep ‘Shared’ UNCHECKED.
>
> When you’re done – the screen should look like this. DO NOT click
> ‘Create’ yet – Scroll down to Define the remote data set (Next
> section)
>
> ![](media/image17.png){width="7.444444444444445in"
> height="5.378472222222222in"}

a)  Now scroll down, click on ‘Add Remote Data Set’ and enter the
    following: ‘GOSales’ for the ‘Remote Data Set Name’

> Leave ‘Schema’ blank.
>
> ‘dash7268.GOSALES’ for the ‘Table’
>
> ![](media/image18.png){width="7.444444444444445in" height="4.2875in"}
>
> Now click ‘Create’.

a)  The ‘GOSales’ data source should now appear.

> ![](media/image19.png){width="7.05625in"
> height="2.9611111111111112in"}
>
> Click on ‘Add model’ under ‘+’ pull down on the top right NOT the drop
> down arrow
>
> ![](media/image20.tiff){width="7.250694444444444in"
> height="3.040277777777778in"}

a)  On the ‘Add Model’ screen, enter your team name ‘TeamXX’ for the
    ‘Name’ and select ‘Manual’. Now click on ‘Create’.

> ![](media/image21.tiff){width="4.55625in"
> height="2.8777777777777778in"}

a)  ![](media/image22.jpeg){width="5.870138888888889in"
    height="1.867361111111111in"}Now we need to select the data to run
    the model. Select the ‘GOSales’ data source that we just created and
    click on ‘Next’.

b)  Wait until the data is loaded. A small sample of the data will be
    displayed. Please keep ‘Auto Data Preparation’ and click on
    ‘**Next**’ to select the data. Note: The data displayed on your
    screen will be different from the screen print
    below![](media/image24.jpeg){width="7.120833333333334in"
    height="2.884027777777778in"}

c)  Now select the column to predict ‘Column value to predict (Label
    Col)’. From the drop down list select ‘PRODUCT\_LINE’ . DSX will
    suggest the best technique to train. Notice that a ‘Multiclass
    Classification’ is selected for the ‘Suggested technique’.
    Estimators are used to train on the data and produce a model for
    each one. Now click on ‘Add Estimators’.

> ![](media/image27.jpeg){width="7.120833333333334in"
> height="2.7805555555555554in"}

a)  ![](media/image28.jpeg){width="3.7506944444444446in"
    height="1.4770833333333333in"}Next screen will be displayed. Leave
    the Search blank (magnifying glass ) to let DSX decide whar
    estimator to use. Select all three estimators (Decision Tree
    Classifier, Random Forest Classifier, Naïve Bayes) to compare
    results between all 3 , by clicking on the
    ![](media/image30.png){width="0.33402777777777776in"
    height="0.36944444444444446in"} for each technique. Now click ‘Add’.

b)  ![](media/image31.jpeg){width="4.334027777777778in"
    height="2.584722222222222in"}The list of configured estimators will
    be listed. Click **Next** to train and evaluate the model

c)  ![](media/image33.jpeg){width="4.747222222222222in"
    height="1.1076388888888888in"}The models will now be trained. This
    may take some time so please be patient.

d)  The results of the 3 estimators will be listed. In this case, the
    ‘Decision Tree Classifier’ provided the best results. Please select
    the estimator with the best performance and click on ‘Save’. Note:
    The accuracy of each of these models is ‘Poor’ or ‘Fair’. Greater
    accuracy may be achieved by using a notebook as in ‘Part 1’ and
    provide more data, regularization, normalization or other
    techniques. For purposes of this lab to show the process, we will
    continue with the best of the 3.

> ![](media/image34.jpeg){width="7.120833333333334in"
> height="2.4604166666666667in"}
>
> You will be prompted to Save the model. Each time you save a the same
> model, its version will be incremented. Click Save
>
> ![](media/image35.png){width="4.132638888888889in"
> height="1.1069444444444445in"}
>
> The Model will be processed
>
> ![](media/image36.png){width="4.549305555555556in"
> height="1.4194444444444445in"}
>
> The list of Models will be displayed. Your list of Models will be
> different from the screen print below.
>
> ![](media/image37.png){width="7.541666666666667in"
> height="3.004166666666667in"}

a)  Now it’s time to deploy the model. Click on the 3 dots next to the
    model you just created, and select **Deploy**

> ![](media/image38.png){width="5.660416666666666in"
> height="2.6131944444444444in"}

a)  In the ‘Create deployment’ screen – Name is your team name ‘TeamXX’.
    For DSX on IIAS , the only supported deployment type is online. For
    Type select ‘Online’ for ‘Deployment Type’ Now click on **Create**.

> ![](media/image39.png){width="3.5493055555555557in"
> height="2.4194444444444443in"}

a)  ![](media/image41.jpeg){width="5.61875in"
    height="3.0944444444444446in"}The model will be deployed. When it
    completes, a list of deployed models will be listed under
    Deployments tab. Under ‘Deployments’, look for your team name e.g.
    ‘Team00’ and Click. Notice that the scoring endpoints are displayed.
    You can score models outside DSX using these ML scoring endpoints
    via REST APIs using curl for example. For this lab, Click on
    ‘**TestAPI**’.

> bb) Use the provided input or specify something different, then click
> on ‘Predict’. The scoring results will be displayed. This means that
> for this customer demographic : Gender : Female, Age: 28, Marital
> Status:Single, Profession : Other, 42.09 will buy Personal
> Accessories, 31.52% will buy Camping Equipment, 16.85% will buy
> Mountaineering Equipment, 5.56% will buy Golf Equipment and 1.03% will
> buy Outdoor Protection.
>
> ![](media/image43.png){width="6.702083333333333in"
> height="3.433333333333333in"}

Congratulations !! - You have completed this lab
================================================

![](media/image44.png){width="6.903472222222222in"
height="1.6201388888888888in"}

> ![](media/image48.png){width="7.1in" height="0.44375in"}
>
> ![](media/image2.png){width="1.0833333333333333in"
> height="0.4027777777777778in"}
>
> © Copyright IBM Corporation 2016. Author: Daniel Kikuchi
>
> The information contained in these materials is provided for
> informational purposes only, and is provided AS IS without warranty of
> any kind, express or implied. IBM shall not be responsible for any
> damages arising out of the use of, or otherwise related to, these
> materials. Nothing contained in these materials is intended to, nor
> shall have the effect of, creating any warranties or representations
> from IBM or its suppliers or licensors, or altering the terms and
> conditions of the applicable license agreement governing the use of
> IBM software. References in these materials to IBM products, programs,
> or services do not imply that they will be available in all countries
> in which IBM operates. This information is based on current IBM
> product plans and strategy, which are subject to change by IBM without
> notice. Product release dates and/or capabilities referenced in these
> materials may change at any time at IBM’s sole discretion based on
> market opportunities or other factors, and are not intended to be a
> commitment to future product or feature availability in any way.
>
> ![](media/image50.png){width="1.1111111111111112in"
> height="0.2777777777777778in"}IBM, the IBM logo and ibm.com are
> trademarks of International Business Machines Corp., registered in
> many jurisdictions worldwide. Other product and service names might be
> trademarks of IBM or other companies. A current list of IBM trademarks
> is available on the Web at “Copyright and trademark information” at
> [www.ibm.com/legal/copytrade.shtml.](http://www.ibm.com/legal/copytrade.shtml)
