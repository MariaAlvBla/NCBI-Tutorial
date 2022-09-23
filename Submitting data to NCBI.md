# Submitting 16S rRNA gene sequence data to NCBI's Sequence Read Archives
<br />

This instructive provides step-to-step instructions to deposit 16S rRNA gene amplicon sequence data at the National Center for Biotechnology Information (NCBI).

<br />

>## Table of contents
<br />

1. [Registering to NCBI](#registering)
2. [Accessing the Sequence Read Archive (SRA)](#accessingsra)
3. [Submitting data to SRA through the Submission Wizard](#submittingwizard)
	1. [Aspects to consider before submitting data](#aspects)
	2. [Submitting data](#steps)
		1. [Step 1. Submitter](#submitter)
		2. [Step 2. General Information](#general)
		3. [Step 3. Project (BioProject) information](#bioproject)
		4. [Step 4. BioSample type](#biotype)
		5. [Step 5. BioSample attributes](#bioattributes)
			1. [Possible Errors at this step](#errors1)
		6. [Step 6. SRA Metadata](#metadata)
			1. [Recommendations to avoid common errors when submitting SRA metadata](#avoiderrors)
			2. [Submitting in new BioSamples vs submitting to already existing ones](#newvs)
			3. [Explanation of the elements of a public display at a single SRA Sample](#elementssra)
		7. [Step 7. Files](#files)
			1. [Possible Errors or Warnings at this step](#errors2)
		8. [Step 8. Review and Submit](#review)
4. [Accessing an unfinished submission](#unfinished)
5. [Processing of the submission](#processing)
	1. [The Project is being reviewed by NCBI’s staff](#reviewed)
	2. [The Project has been accepted](#accepted)
		1. [Public display and searchable elements of a BioSample](#publicbiosample)
		2. [Public display and searchable elements of a SRA Experiment](#publicsra)
6. [Changing a submission](#changing)
7. [Downloading data](#downloading)
	1. [Downloading data corresponding to one accession number](#downloadingone)
	2. [Downloading data corresponding to several accession numbers](#downloadingmore)
<br />

>## Registering to NCBI <a name="registering"></a>
<br />
To register to NCBI follow the next steps:
<br />
<br />

---
1. [**Access NCBI's homepage**](https://external.ink?to=https://www.ncbi.nlm.nih.gov/) and click ***Log in***.
<br />
<img src=".\First time upload images\home-login.png">

<br />

____
2. A menu with several lo Login options will be displayed. You can choose whichever you prefer for setting your account.
<br />
<img src=".\First time upload images\login-options.PNG">


<br />


>## Accessing the Sequence Read Archive (SRA) <a name="accessingsra"></a>
<br />

For accessing the Sequence Read Archive (SRA) follow the next steps:
<br />
<br />
____
1. While being logged in, [**Access NCBI's homepage**](https://external.ink?to=https://www.ncbi.nlm.nih.gov/).

<br />

____
2. Click ***Submit***.
<br />
<img src=".\First time upload images\home-submit.png">

<br />

____
3. The main page of the Submission Portal will be displayed. For the occasion of the Datathon, ***write 16S rRNA*** in the search bar and ***click SRA***. 
<br />
<img src=".\First time upload images\portal-submit.png">
 
<br />

____
4. A webpage with information about the Sequence Read Archive (SRA) will be displayed. SRA specializes in high throughput sequence data, including 16S rRNA gene sequence data.Click ***Submit***.
<br />
<img src=".\First time upload images\sra-submit.png">


<br />


>## Submitting data to SRA Submission Wizard] <a name="submittingwizard"></a>
<br />

>### Aspects to consider before submitting data <a name="aspects"></a>
<br />

- If the data comes from a human study, donor consent is usually necessary.

- Each upload must be kept under 5 TB, if you have more, split the upload across multiple submissions.

- Submissions can be linked to the same BioProject to ensure all data are searchable with a single accession code.

- Every fastq file should be less than 100 GB in size. If compressed files are larger than 100 GB, please split them before submission.

<br />


>### Submitting data <a name="steps"></a>
<br />
This process requires several steps. To save your progress, click ***Continue***. You can review or make changes to your previous steps during submission by clicking on the preceding tabs.  

At any point after having saved your progress, you can leave NCBI and [continue the process of submission later](#unfinished). If, however, you click the ***Submit*** button at the [last step](#review), [making changes will require additional steps](#changing). 

You may get *Error* or *Warning* messages when saving your progress. Error messages describe the Error and suggest a solution that must be corrected before you can move to the next step of your submission. On the other hand, the Warning messages attempt to prevent you from making a possible mistake and do not block you from continuing your submission. 

<br />


>#### Step 1. Submitter <a name="submitter"></a>

<br />
<img src=".\First time upload images\submitter.png" width=90% height=90%>

<br />

Here, the data archiver will be asked to include professional information. We recommend using you institutional **e-mail** and writting the information of the **institution** you work for.

<br />


>#### Step 2. General Information <a name="general"></a>

<br />
<img src=".\First time upload images\general-info.png" width=80% height=80%>

<br />

The **BioProject** represents the research project from which the dataset originated. The information supplied in the **Biosample** provides context to your experimental data. Every metagenome, time point, tissue type, or treatment type must have its own Biosample; but biological and technical replicates are not unique BioSamples. _If the data you will submit is not linked to any previously submitted data, select **No** for the BioProject and BioSample categories in this step. 

*Note: most often, each sample will also be its own BioSample. If unsure, it is best to have each sample be a separate BioSample.*

<br />

<img src=".\First time upload images\diagram.png" width=80% height=80%>
<br />

Depending on your answers at this step, the next steps would follow one of these pathways:

<br />

<img src=".\First time upload images\pathway-map.png" width=80% height=80%>
<br />


The default **release date** is **Release immediately following processing**, but you can select a specific date for releasing your data. If you don’t know the exact data you can change it even after having finished the submission by clicking on the [***Manage tab*** at the Submission Portal](#changing).


<br />


>#### Step 3. Project (BioProject) information<a name="bioproject"></a>
<br />

<img src=".\First time upload images\bioproject-info.png" width=80% height=80%>

<br />


In the **Public description** provide information that best describes your research, which will become the description of your BioProject. If you have an **abstract** or research summary of your research project, you should add it here. Also, we recommend that at **URL** you add the DOI link to any publication of yours that is related to this data. 

<br />


>#### Step 4. BioSample type<a name="biotype"></a>
<br />
In this step, you will select a **Package** that best fits the nature of your Biosample. According to your selected package the Submission Portal will supply you with a customized **attribute table** for the [next step](#bioattributes) that best describes the context of your BioSamples.

Select the package ***MIMARKS Survey related***. In the displayed drop-down menu, select the sample type that better describes your sample.

<br />

<img src=".\First time upload images\biosample-type-section.png" width=70% height=70%>

<br />


>#### Step 5. BioSample attributes <a name="bioattributes"></a>
<br />

This step provides contextual information about your samples. 

<br />

<img src=".\First time upload images\biosample-attribute.png" width=80% height=80%>

<br />

For the **Datathon**, select ***Uploading a file using Excel format*** and use the following customed Excel table:
<br />
<br />

[**MIMARKS.survey.soil.5.0_Dathaton.xlsx**](https://external.ink?to=https://github.com/MariaAlvBla/NCBI-Tutorial/blob/main/Datathon%20tables/)

<br />
Please read the instructions included in the excel carefully before filling in the values. Remember that you can only upload the tab-delimited text file version of the sheet **MIMARKS.survey.soil.5.0**. If working in Excel, export this spreadsheet as a tab-delimited file

The **sample_name** you give each sample in the attribute table will be again used at the [**SRA metadata table**](#metadata) to link the sequence data and metadata. The sample names must be the same in both Excel files for them to be linked together.


<br />


>##### Possible Errors at this step <a name="errors1"></a>
<br />

***Error: Multiple BioSamples cannot have identical attributes***

<br />

**Problem**

After filling out values for attributes provided in the template, your individual samples are not distinguishable by at least one or a combination of attributes.
<br />

**Solution**

Make sure the combined value of all attributes is unique for each Biological sample. Note that **sample name**, **sample title**, and **description** are not included in this check for uniqueness of the sample's attributes. If this problem arises because of biological replicates, please add a replicate column to the sheet and record the replicate numbers to differentiate them.

<br />

***Error: Multiple BioSamples cannot have identical attributes***

<br />

**Problem**

Less often, this error may arise if you are attempting to deposit sequences that have already been deposited to NCBI, and the Submission Portal is preventing you from creating duplicates.
<br />

**Solution**

If you want to include an existing BioSample in the new BioProject, go back to the [General Info tab](#general) and select *Yes* to the question *Did you already register BioSamples for this data set?*. The SRA Submission Wizard will then skip the BioSample type and attributes steps.
<br />

If you are using the [**SRA_metadata_Datathon.xlsx**, in the SRA metadata step](#metadata), you need to change the name of the first column from **sample_name** to **biosample_accession**. Then you can add the existing BioSample's accession numbers **(SAMN#)** to link the new sequence files to the already existing BioSamples; and to include them in the new BioProject. 
<br />

To find the accession numbers of Biosamples you already registered go to the [Submission Portal](#accessingsra) and follow the next steps: 
<br />
<br />
____
1. Click ***My submissions***.
<br />
<img src=".\First time upload images\portal-submissions.png">
 
<br />

____
2. Click ***objects*** in the BioSample section of the Project. 
<br />
<img src=".\First time upload images\my-submissions.png">

<br />


>#### Step 6. SRA Metadata<a name="metadata"></a>
<br />

The SRA metadata describes the technical aspects of each sequencing experiment: the sequencing libraries, preparation techniques, and the names of the data files. 

<br />

<img src=".\First time upload images\sra-metadata.png" width=80% height=80%>
<br />

For the **Datathon**, select ***Uploading a file using Excel format*** and use the following customed Excel table:
<br />
<br />

[**SRA_metadata_Datathon.xlsx**](https://external.ink?to=https://github.com/MariaAlvBla/NCBI-Tutorial/blob/main/Datathon%20tables/)

<br />
Please read the instructions included in the spreadsheet carefully before filling in the values. You can only upload the tab-delimited text file version of the spreadsheet **SRA data**. If working in Excel, export that spreadsheet as a tab-delimited file. 

When submitting the project, SRA **Experiment** captures the unique combination of techniques that was used to sequence a particular sample (i.e., each combination of **library + sequencing strategy + layout + instrument model** represents a different experiment). 
_Note: most often, all samples within a project will be sequenced using the same combination of techniques, and will thus belong to a single Experiment. The most common exception is when two gene regions (e.g., 16S rRNA and ITS) are sequenced for the same project. 

<br />


>##### Recommendations to avoid common errors when submitting SRA metadata <a name="avoiderrors"></a>
<br />

- Paired-end data files (forward/reverse) must be listed together in the same **Run** (in the case of the spreadsheet in the same row) for the two files to be correctly processed as paired-end. All data files listed in a **Run** will be merged into a single **sra archive file**. Therefore, files from different samples or experiments should not be grouped in the same **Run**.

- File name(s) for the **Experiments** shouldn’t contain any sensitive information, because they will appear publicly on the Google and AWS clouds.

- Avoid submitting duplicated files because the Portal does not accept this, and such files may be suppressed without warning.

<br />


>##### Submitting new sequence data vs submitting new metadata to already existing ones <a name="newvs"></a>
<br />
When submitting new BioSamples, during the [BioSample attributes step](#bioattributes), a specific name for each sample is assigned in the **sample_name** column of the [**MIMARKS.survey.soil.5.0_Dathaton.xlsx** file](#bioattributes). In the SRA Metadata step, in the [**SRA_metadata_Dathaton.xlsx** spreadsheet](#metadata), the **sample_name** must match that given to the new BioSample, to correctly link the sequence data to the metadata.
<br />


>##### Explanation of the elements of a public display for each Sample in the SRA<a name="elementssra"></a>
<br />
<img src=".\First time upload images\experiment-display-long.png">

<br />

>#### Step 7. Files <a name="files"></a>
<br />

In this step, you will upload the files listed in the [**SRA Metadata excel file**](#metadata). Files can be compressed using gzip or bzip2 and may be submitted in a _tar archive, but archiving and/or compressing your files is not required. Uploading zip files is not permitted. If you are uploading a tar archive, list each file name within the archive, not the archive's name.

<br />

<img src=".\First time upload images\uploading-files.png">

<br />

We recommend you use the ***Web browser upload via HTTP or Aspera Connect plugin*** option to upload the files, unless you have more than 10 GB of data or more than 300 files to upload at once.

We recommend you select ***Autofinish submission*** once the files have been successfully uploaded. Take into consideration that depending on the size and number of files,  uploading may take from several minutes to a few hours. 

Don’t forget to press ***Continue*** to save your progress. Otherwise you have to upload the files again.

<br />

>##### Possible Errors or Warnings at this step <a name="errors2"></a>
<br />

***Warning: You uploaded one or more extra files that are not in your Metadata table***

<br />

**Problem**

You have uploaded files not listed in your SRA Metadata template. 
<br />

**Solution**

If you do not intend to include these files in your SRA submission, click ***Continue***. All files not included in the SRA Metadata will be ignored. If you intend to include these files in your SRA submission, return to the [SRA Metadata step](#metadata) and update their names.

<br />

***Error: Some files are missing. Upload missing files or fix metadata table***

<br />

**Problem**

The program does not find all files listed in the SRA Metadata table in your submission folder.
<br />

**Solution**

Upload files that are reported missing. Also, check that filenames listed in your metadata table, and make sure that the file extensions (.fq, .fastq, .sff, etc.) exactly match those of the files you want to upload. In the latter case, go back to the [SRA Metadata tab](#metadata), delete your metadata file and upload a new one with the correct filenames. Click ***Continue***. 

<br />

***Error: File <filename> is corrupted. Please re-upload the file...***

<br />
	
**Problem**

This Error occurs either because you have corrupt files on your side or the files became corrupted during transfer. 
<br />

**Solution**
	
Re-upload the files that were reported corrupt. For this, click the Fix button and follow the instructions. The filenames must be the same. Before re-uploading,  check the files for integrity on your side. If the gzip utility reported an error,  find and upload an uncorrupted version of this file before proceeding. If the file is OK, you can re-upload it.

<br />

	
>#### Step 8. Review and Submit <a name="review"></a>
<br />
	
During this step, you can review your submission's summary and make sure that everything is correct. You can still return to and change any step of your submission at this stage by clicking on the corresponding tabs at the top.

<br />
	
<img src=".\First time upload images\submission-finished.png">
<br />
	
Click ***Submit*** when you are sure everything is correct. After submitting, future changes to the BioProject are limited or can only be achieved by contacting NCBI's service desk.
	
If, on the other hand, you want to delete the whole submission click ***Delete submission***. This is the last chance to delete the submission without emailing NCBI’s service desk.

<br />

	
>## Accessing an unfinished submission <a name="unfinished"></a>
<br />
To access an unfinished submission follow the next steps:
<br />
<br />

---
1. While logged in, go to [**NCBI's homepage**](https://external.ink?to=https://www.ncbi.nlm.nih.gov/).

<br />

____
2. Click ***Submit***

<br />

____
3. In the Submission Portal click on ***My submissions***.
<br />
<img src=".\First time upload images\portal-submissions.png" width=80% height=80%>

<br />

____
4. Find the submission with the ***Unfinished Status*** that has the title of the submission or the **submission ID (SUB#)** you are looking for.
<br />
<img src=".\First time upload images\unfinished-submission.png">


<br />


>## Processing  the submission<a name="processing"></a>
<br />

>### The Project is being reviewed by NCBI’s staff<a name="reviewed"></a>
<br />

Once submitted, your submission will be queued for processing, and you will likely get feedback within 24 hour.If submitting through the SRA Wizard, you will  receive feedback from the Wizard first.

If your submission was successfully registered, you will receive the following email. 

<br />

<img src=".\First time upload images\email-1.PNG">
<br />


The project number you have been given **(PRJ#)** is permanent and unique,  but it will not appear to other users until NCBI's staff has fully processed it. We kindly ask you to provide the project number for the **Dathaton's database**.


<br />


>### The Project has been accepted<a name="accepted"></a>
<br />
	
After the submitted data has been processed, you will receive the following email.

<br />

<img src=".\First time upload images\email-2.PNG">

<br />

Once the Project has been accepted, when someone searches for your project, the following information will be displayed.

<br />

<img src=".\First time upload images\seach-prj.png">

<br />


>#### Public display and searchable elements of a BioSample<a name="publicbiosample"></a>
<br />
<img src=".\First time upload images\biosample-public.png">

<br />

The **BioSample (SAMN#)** is the identifier of specific Biosamples.
Clicking on ***Retrieve all samples from this project*** allows you to see all the other BioSamples associated to the BioProject.

<br />


>### Public display and searchable elements of a SRA Experiment<a name="publicsra"></a>

<br />
<img src=".\First time upload images\experiment-display-short.png">

<br />
	
The marked elements are:
<br />

- **Experiment (SRX#)**: identifier of instrument and library information of a specific sample (SRS#).

- **Study (SRP#)**: identifier of a study within a BioProject.

- **Sample (SRS#)**: identifier of a sample of sequence data.

- **Run (SRR#)**: identifier of the data file(s) derived from sequencing a library described by the associated Experiment.

<br />


>## Changing a submission<a name="changing"></a>
<br />

Follow the next steps:
<br />
<br />
____
1. While being logged in, go to [**NCBI's homepage**](https://external.ink?to=https://www.ncbi.nlm.nih.gov/).

<br />

____
2. Click ***Submit***

<br />

____
3. At the Submission Portal click on ***Manage data***.
<br />
<img src=".\First time upload images\portal-manage.png" width=80% height=80%>

<br />

____
4. Select the **BioProject (PRJNA#)** you want to update. You can also filter it by BioSamples at the ***BioSample tab*** or by Experiments at the ***SRA tab***. With these other filtering options the data shown by the Data Manager actually can't be edited. 
<br />
<img src=".\First time upload images\click-manage-data.png" width=80% height=80%>
<br />

The BioProject’s managing page allows you to:
<br />
	
- ***Edit*** fields that were written during the submission.
	
- ***Add*** information that was not written during the submission.
	
- ***Edit*** most fields of the SRA Metadata. You have to check the boxes for the Experiments you want to modify first.

<br />

<img src=".\First time upload images\manage-data.png" width=80% height=80%>
<br />

If you want to add more data to an existing BioProject or Biosample, [create a new SRA submission](#accessingsra) and enter the accession number of the BioProject **(PRJNA#)** or the Biosample **(SAMN#)** when asked. This will ensure that the new data is linked to the existing BioProject.

If you want to change the attributes or withdraw a BioProject or BioSample that has already been submitted and not necessarily accepted, you have to conact bioprojecthelp@ncbi.nlm.nih.gov or biosamplehelp@ncbi.nlm.nih.gov for assistance in updating your BioProject or BioSample submission respectively.

A Submission represents a discrete act of depositing data (a transaction). The submission has a temporary non-public ID as a **SUB#**. You cannot add more data to a completed submission. To update a submission, contact sra@ncbi.nlm.nih.gov.

After the **Run** is fully loaded, neither its files can be replaced, nor filenames can be changed. You will have to submit new files in a separate submission using [existing BioProject and BioSample accessions](#general) and request withdrawal of the **Run** containing the old files.


<br />


>## Downloading data<a name="downloading"></a>	
<br />

>### Downloading data corresponding to a project <a name="downloadingone"></a>
<br />

As we have seen, NCBI supports the inclusion of exhaustive metadata when uploading data. To download all sequence data corresponding to a specific project or accession number, we recommend using the portal from the European Bioinformatics Institute  as part of the European Molecular Biology Laboratory [**(EMBL-EBI)**](https://external.ink?to=https://www.ebi.ac.uk/). For this you would have to follow the next steps:
<br />
<br />
____
1. Access [**EMBL-EBI's homepage**](https://external.ink?to=https://www.ebi.ac.uk/)

<br />

____
2. Write the accession code of the BioProject, BioSample or SRA you are interested in, and click ***Search***.
<br />
<img src=".\First time upload images\european-portal-search.png">

<br />

____
3. Scroll down and select the entry corresponding to the accession number you were looking for.

<br />

____
4. A shortened version of the metadata will be shown, as well as the files belonging to this accession number. For accessing the file's download option, scroll to the right at the sections with the list of files.
<br />
<img src=".\First time upload images\dowload-ebi.png">

<br />

____
5. Click ***Download All*** if you want to dowload all the **Experiments (SRR)** under this accession number. If you want to dowload only specific Experiments, select the corresponding check-boxes and click ***Download selected files***
<br />
<img src=".\First time upload images\ebi-download-scroll.png">


<br />

	
>### Downloading data corresponding to several accession numbers<a name="downloadingmore"></a>
<br />
To download large amounts of SRA data we recommend you use the [**SRA Toolkit**](https://external.ink?to=https://github.com/ncbi/sra-tools/wiki).



