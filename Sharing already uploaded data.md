# Sharing data that has already been uploaded to NCBI's SRA
<br />

Once data is archived, NCBI's SRA creates summary metadata table of the sample metadata (e.g., the sample's geographic location and sample type) and technical metadata (e.g., the sequencer used) for all samples in that BioProject or BioSample. As there are no standard nomenclatures for many of these fields, integrating metadata from different projects is difficult. For example, the word amplicon can be written as *amplicon*, *Amplicon* or *AMPLICON*, and this creates a problem when combining  several projects where the meaning of these values is identical, but they are named differently, hindering the large scale analysis of genetic data.

For the Datathon, we have created a custom table with fixed nomenclatures for categories that are essential for large scale analysis. Following this standard nomenclature facilitates the sharing and combining of data by researchers. *This tutorial will guide users on how to access and transform existing NCBI SRA metadata tables to this standard nomenclature.

<br />

>## Table of contents
<br />

1. [Accessing the metadata associated to a BioProject](#accessing)
	1. [By searching the accession code](#searching)
	2. [By tracking it in "my submissions"](#tracking)
2. [Downloading the summary table of a BioProject or a BioSample](#summary)
3. [Transfering metadata to the Datathon's customized table](#transfering)
	1. [Opening NCBI's summary table](#opening)
	2. [Filling in the customized table](#filling)
<br />
  
>## Accessing the metadata associated to a BioProject <a name="accessing"></a>
<br />

To access the genetic data of either an entire **BioProject** or a specific **BioSample within a BioProject**, one must access the BioProject containing the data first. From the BioProject, one can choose to access all the **Experiments** of either the BioProject or the BioSample, this will be further explained below ([**jump to downloading the summary table**](#summary)).

Accessing the data associated to a **BioProject** can be achieved in two ways: 1) if you [**remember the accession code**](#searching) and 2) if you [**don't remember it**](#tracking). Please select the option that better suits your case. 

<br />

>### By searching the accession code <a name="searching"></a>
<br />

To find the public display of the genetic data of your **BioProject** follow the next steps:
<br />
<br />
____
1. [**Access NCBI's homepage**](https://external.ink?to=https://www.ncbi.nlm.nih.gov/) and write the **accession code** of the BioProject **(PRJNA#)** you are looking for.
<br />
<img src=".\Sharing already uploaded data images\search-accession.png">

<br />

____
2. Click on the correct BioProject in the displayed list.
<br />
<img src=".\Sharing already uploaded data images\select-bioproject.png">

<br />

____
3. The BioProject's public information will be displayed. To find the genetic information related to the BioProject click the ***number on the right of the SRA Experiments*** 
<br />
<img src=".\Sharing already uploaded data images\bioproject-public.png" width=80% height=80%>

<br />


Jump to [**Downloading the BioProject's summary table**](#summary).


<br />


>### By tracking it in "my submissions" <a name="tracking"></a>
<br />

To find the public display of the genetic data of your **BioProject** follow the next steps:
<br />
<br />
____
1. While being logged in, go to [**NCBI's homepage**](https://external.ink?to=https://www.ncbi.nlm.nih.gov/).

<br />

____
2. Click ***Submit***
<br />
<img src=".\Sharing already uploaded data images\home-submit.png">

<br />

____
3. At the Submission Portal click on ***My submissions***.
<br />
<img src=".\Sharing already uploaded data images\portal-submissions.png">

<br />

____
4. Find the submission with the title corresponding to the BioProject you are looking for and click the accession code **(PRJNA#)**.
<br />
<img src=".\Sharing already uploaded data images\my-submissions.png" width=90% height=90%>

<br />

____
5. The BioProject public information will be displayed. To find the genetic information related to the BioProject click the ***number on the right of the SRA Experiments***
<br />
<img src=".\Sharing already uploaded data images\bioproject-public.png" width=80% height=80%>

<br />


Jump to [**Downloading the BioProject's summary table**](#summary)

<br />


>## Downloading the summary table of a BioProject or a BioSample <a name="summary"></a>
<br />

Follow these steps to access and download the summary table of the attribute and metadata information of all the genetic data included in a BioProject or BioSample.
<br />
<br />
____
1. Click at the name of any of the **Experiments** displayed after having accessed the **SRA Experiments** in the previous section.
<br />
<img src=".\Sharing already uploaded data images\click-experiment.png">

<br />

____
2. At the public display of the **Experiment** click ***All Runs*** for either the **BioProject** or the **BioSample** you are interested in. If you select the Runs of the BiopProject or BioSample, the summary table will include the information of the selected experiment as well as any other experiments included in the same BioProject or BioSample.
<br />
<img src=".\Sharing already uploaded data images\all-runs.png" width=80% height=80%>

<br />

____
3. To download all the runs contained in the BioProject or BioSample, click on ***Metadata*** 
at the the **Total** option.
<br />
<img src=".\Sharing already uploaded data images\download-all-metadata.png" width=90% height=90%>

<br />

____
Alternatively you can download specific **Runs** by checking on the boxes corresponding to the runs you want to download, and clicking on ***Metadata*** at the the **Selected** option.

<br />

<img src=".\Sharing already uploaded data images\download-some-metadata.png" width=90% height=90%>

<br />


>## Transfering metadata to the Datathon's customized table <a name="transfering"></a>
<br />
After having download NCBI's summary table, it must be opened with [specific settings](#opening) to display it's information correctly. After having opened it, some of it's data needs to be [transfered to a customized table](#filling) created for the Datathon, to ensure that all shared data has a consistent format. 

<br />

>### Opening NCBI's summary table <a name="opening"></a>
<br />

If you followed the steps in the [previous section](#summary), you will now have a text file (.txt) with the name **SraRunTable**. Instead of opening it with a text procesor, open it with software such as  **Open Office Calc**, or **Excel**.

When using **Open Office Calc** you need to check the settings of the **Separator Options** to avoid the shifting of the column's values.

In the following picture the settings are wrong and the columns that had values with spaces on them have been separated and shifted to the right. Instead of *University of Copenhagen* in one cell it has been splitted between three columns:

<br />

<img src=".\Sharing already uploaded data images\wrong-setting.png" width=90% height=90%>

After you corrected the separation options, which will depend on the import's lenguage, the columns with values that had spaces on them shouldn't be separated anymore. In our example, now the university's full name is in one cell.

<br />

<img src=".\Sharing already uploaded data images\right-setting.png" width=90% height=90%>


<br />


>### Filling in the customized table <a name="filling"></a>
<br />
Now you can dowload and open the following customed table:
<br />
<br />

[**Metadata_table_Datathon.xlsx**](https://external.ink?to=https://github.com/MariaAlvBla/NCBI-Tutorial/blob/main/Datathon%20tables/)

<br />
This table includes the names of selected columns from NCBI's summary table. Please transfer only the information from these selected columns; and contact the MICODA team if you would like to add more columns to the file. Makes sure you have carefully read the instructions provided in the table before filling in the data, and keep in mind that some of the columns have drop down menus.

