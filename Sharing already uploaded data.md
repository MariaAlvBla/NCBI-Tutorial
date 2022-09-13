# Sharing data that has already been uploaded to NCBI

Whenever data has been submitted, NCBI can create a summary table of the attribute and metadata information of all the genetic data included in a BioProject or BioSample. The problem with this table is that many of the fields don't need to follow a consistent format in order to be submitted to NCBI. For example, the word amplicon can be written as *amplicon*, *Amplicon* or *AMPLICON*. This can signify a problem when wanting to combine the summary data of several projects in which the authors wrote the values differently. It hinders large scale analyses of genetic data.

For the Datathon we have created a custom table with fixed values for some categories that are essential for large scale analysis. By following this homogenized format is easier for researcher to share and combine their data. This tutorial will guide you on how to access and transform the tables given by NCBI to the homogenized format we propose.

## Table of contents
1. [Accessing a BioProject](#accessing)
  1. [By searching the accession code](#searching)
  2. [By tracking it in "my submissions"](#tracking)
  
## Accessing a BioProject <a name="accessing"></a>

Accessing a **BioProject** can be achieved by two paths: one if you [**remember the accession code**](#searching) and one in which you [**don't remember it**](#tracking). Please select the option that better suits your case. 

### By searching the accession code <a name="searching"></a>

To find the public display of the genetic data of your **BioProject** follow the next steps:

1. [**Access NCBI's homepage**](https://www.ncbi.nlm.nih.gov/) and write the **accession code** of the BioProject **(PRJNA#)** you are looking for.

<img src=".\Sharing already uploaded data images\search-accession.png">

2. Click on the BioProject you are looking for from the displayed list.

<img src=".\Sharing already uploaded data images\select-bioproject.png">

3. The BioProject public information will be displayed. To find the genetic information related to the BioProject click the number on the right side of ***SRA Experiments*** 

<img src=".\Sharing already uploaded data images\bioproject-public.png">

### By tracking it in "my submissions" <a name="tracking"></a>

To find the public display of the genetic data of your **BioProject** follow the next steps:

1. While being logged in, go to [**access NCBI's homepage**](https://www.ncbi.nlm.nih.gov/).

2. Click ***Submit***

<img src=".\Sharing already uploaded data images\home-submit.png">

3. At the Submission Portal click on ***My submissions***.

<img src=".\Sharing already uploaded data images\portal-submissions.png" width=80% height=80%>

4. Find the submission with the title corresponding to the BioProject you are looking for and click the accession code (PRJNA#).

<img src=".\Sharing already uploaded data images\my-submissions.png">


When people finish a submission you can download an excel that includes metadata and attribute information. We want the people that already uploaded data to copy and paste their information to our own version of the merged excel file that will also have the drop-down menus from the other excel files.
Just tell them:
1.	We want them to give us the accession numbers of the runs (srr) and the PRJ number
2.	I need to make a new excel data, use the one sent from Stephanie (NCBI).

*Drop down menus must still work (the spelling should all be the same to make sure the coding works). The metadata 

