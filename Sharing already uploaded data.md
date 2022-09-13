# Sharing data that has already been uploaded to NCBI

Whenever data has been submitted, NCBI can create a summary table of the attribute and metadata information of all the genetic data included in a BioProject or BioSample. The problem with this table is that many of the fields don't need to follow a consistent format in order to be submitted to NCBI. For example, the word amplicon can be written as *amplicon*, *Amplicon* or *AMPLICON*. This can signify a problem when wanting to combine the summary data of several projects in which the authors wrote the values differently. It hinders large scale analyses of genetic data.

For the Datathon we have created a custom table with fixed values for some categories that are essential for large scale analysis. By following this homogenized format is easier for researcher to share and combine their data. This tutorial will guide you on how to access and transform the tables given by NCBI to the homogenized format we propose.

## Table of contents
1. [Accessing the genetic data associated to a BioProject](#accessing)
  1. [By searching the accession code](#searching)
  2. [By tracking it in "my submissions"](#tracking)
2. [Downloading the summary table of a BioProject or a BioSample](#summary)
3. [Filling in the Datathon's customized excel table](#filling)
  
## Accessing the genetic data associated to a BioProject <a name="accessing"></a>

When you want to access the genetic data of either an entire **BioProject** or a specific **BioSample within a BioProject**, you always have to access the BioProject containing the data first. From the BioProject you can choose to access all the **Experiments** of either the BioProject or the BioSample, this will be further explained in [**the section about downloading the summary table**](#summary).

Accessing the data associated to a **BioProject** can be achieved by two paths: one if you [**remember the accession code**](#searching) and one in which you [**don't remember it**](#tracking). Please select the option that better suits your case. 

### By searching the accession code <a name="searching"></a>

To find the public display of the genetic data of your **BioProject** follow the next steps:

1. [**Access NCBI's homepage**](https://www.ncbi.nlm.nih.gov/) and write the **accession code** of the BioProject **(PRJNA#)** you are looking for.

<img src=".\Sharing already uploaded data images\search-accession.png">

2. Click on the BioProject you are looking for from the displayed list.

<img src=".\Sharing already uploaded data images\select-bioproject.png">

3. The BioProject public information will be displayed. To find the genetic information related to the BioProject click the ***number on the right of the SRA Experiments*** 

<img src=".\Sharing already uploaded data images\bioproject-public.png">

The explanation continues in the section [**Downloading the BioProject's summary table**](#summary).

### By tracking it in "my submissions" <a name="tracking"></a>

To find the public display of the genetic data of your **BioProject** follow the next steps:

1. While being logged in, go to [**NCBI's homepage**](https://www.ncbi.nlm.nih.gov/).

2. Click ***Submit***

<img src=".\Sharing already uploaded data images\home-submit.png">

3. At the Submission Portal click on ***My submissions***.

<img src=".\Sharing already uploaded data images\portal-submissions.png" width=80% height=80%>

4. Find the submission with the title corresponding to the BioProject you are looking for and click the accession code **(PRJNA#)**.

<img src=".\Sharing already uploaded data images\my-submissions.png">

5. The BioProject public information will be displayed. To find the genetic information related to the BioProject click the ***number on the right of the SRA Experiments***

<img src=".\Sharing already uploaded data images\bioproject-public.png">

The explanation continues in the section [**Downloading the BioProject's summary table**](#summary)

## Downloading the summary table of a BioProject or a BioSample <a name="summary"></a>

Follow the next steps to access and download the summary table of the attribute and metadata information of all the genetic data included in a BioProject or BioSample.

1. Click at the name of any of the **Experiments** displayed after having accessed the **SRA Experiments** in the previous section.

<img src=".\Sharing already uploaded data images\click-experiment.png">

2. At the public display of the **Experiment** click ***All Runs*** for either the **BioProject (A)** or the **BioSample (B)** you are interested in. If you select the Runs of the BioSample, the summary table will include the information of the selected experiment as well as any other experiments included in the same BioSample.

<img src=".\Sharing already uploaded data images\all-runs.png">

3. To download all the runs contained in the BioProject or BioSample, click on ***Metadata*** 
at the the **Total** option.

<img src=".\Sharing already uploaded data images\download-all-metadata.png">

Alternatively you can download specific **Runs** by checking on the boxes corresponding to the runs you want to download, and clicking on ***Metadata*** at the the **Selected** option.

<img src=".\Sharing already uploaded data images\download-some-metadata.png">

## Filling in the Datathon's customized excel table <a name="filling"></a>

If you followed the steps in the [previous section](#summary), you would now have a text file (.txt) with the name **SraRunTable**. Instead of opening it with a text procesor, open it with **Open Office Calc** or **Excel**.



When people finish a submission you can download an excel that includes metadata and attribute information. We want the people that already uploaded data to copy and paste their information to our own version of the merged excel file that will also have the drop-down menus from the other excel files.
Just tell them:
1.	We want them to give us the accession numbers of the runs (srr) and the PRJ number
2.	I need to make a new excel data, use the one sent from Stephanie (NCBI).

*Drop down menus must still work (the spelling should all be the same to make sure the coding works). The metadata 

