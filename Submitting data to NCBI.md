# Submitting 16S rRNA sequence data to the National Library of Medicine (NCBI) 

**Authors:** María José Álvarez Blanco & Stephanie Jurburg
<br />
<br />
**Contact MICODA Team:** <contact.micoda@gmail.com>
<br />
<br />
**Associated institutions:**
<br />
<br />
<br />
<img src=".\First time upload images\logo MiCoDa empty.png" width=30% height=30%>
<br />
<br />
<img src=".\First time upload images\iDivLogo-short.png" width=30% height=30%>
<br />
<br />
<img src=".\First time upload images\ufz_logo.png" width=35% height=35%>
<br />
## Table of content

1. [Registering to NCBI](#registering)
2. [Accessing the Sequence Read Archive (SRA)](#accessingsra)
3. [Submitting data to SRA Submission Wizard](#submittingwizard)
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
			1. [Possible Errors or Warnings at this step] (#errors2)
		8. [Step 8. Review and Submit](#review)
4. [Accessing an unfinished submission](#unfinished)
5. [Processing of the submission](#processing)
	1. [The Project is being reviewed by NCBI’s staff](#reviewed)
	2. [The Project has been accepted](#accepted)
		1. [Public display and searchable elements of a BioSample](#publicbiosample)
		2. [Public display and searchable elements of a SRA Experiment](#publicsra)
6. [Changing a submission](#changing)
7. [Downloading data](#dowloading)
	1.[Downloading data corresponding to one accession number](#dowloadingone#)
	2.[Downloading data corresponding to several accession numbers](#dowloadingmore)

## Registering to NCBI <a name="registering"></a>

Follow the next steps:

1. [**Access NCBI's homepage**](https://www.ncbi.nlm.nih.gov/) and click ***Log in***.

<img src=".\First time upload images\home-login.png">

2. A menu with several lo Login options will be displayed. You can choose whichever you prefer for setting your account.

<img src=".\First time upload images\login-options.PNG">

## Accessing the Sequence Read Archive (SRA) <a name="accessingsra"></a>

For accessing the Sequence Read Archive (SRA) follow the next steps:

1. While being logged in, [**Access NCBI's homepage**](https://www.ncbi.nlm.nih.gov/). ***write 16S rRNA*** 

2. Click ***Submit***.

<img src=".\First time upload images\home-submit.png">

3. The main page of the Submission Portal will be displayed. For the occasion of the Datathon, ***write 16S rRNA*** in the search bar and ***click SRA***. This leads to the Sequence Read Archive, which specializing in managing data such 16S rRNA.

<img src=".\First time upload images\portal-submit.png">
 
4. A webpage with information on the Sequence Read Archive (SRA) will be displayed. Click ***Submit***.

<img src=".\First time upload images\sra-submit.png">

## Submitting data to SRA Submission Wizard] <a name="submittingwizard"></a>

### Aspects to consider before submitting data <a name="aspects"></a>

- If human data comes from a metagenomic study, donor consent is necessary.

- Each upload must be kept under 5 TB, if you have more, split the upload across multiple submissions.

- Submissions can be linked to the same BioProject to ensure all data are searchable with a single accession code.

- Every fastq file should be less than 100 GB in size. If compressed files are larger than 100 GB, please split them before submission.

### Submitting data <a name="steps"></a>

For every step, you will have to add information or files; whenever you want to save your progress, you must press ***Continue***. You can review or make changes to your previous steps during submission by clicking on the preceding tabs.  

At any point, after having saved your progress, you can leave NCBI and [continue the process of submission later](#unfinished). If, however, you click the ***Submit*** button at the [last step](#review), [making changes would follow other routes](#changing). 

You may get *Error* or *Warning* messages when saving your progress. Error messages describe the Error and suggest a solution that must be corrected before you can move to the next step of your submission. On the other hand, the Warning messages attempt to prevent you from making a possible mistake and do not block you from continuing your submission. 

#### Step 1. Submitter <a name="submitter"></a>

<img src=".\First time upload images\submitter.png" width=90% height=90%>

At this step, the submitting person will be asked for personal information at this step. At the fields signaled in the following picture we recommend using you institutional **e-mail** and writting the information of the **institution** you work for.

#### Step 2. General Information <a name="general"></a>

<img src=".\First time upload images\general-info.png" width=80% height=80%>

The **BioProject** represents the research project from which the sequence originated.The information supplied in the **Biosample** provides context to your experimental data. Every metagenome, time point, tissue type, or treatment type must has its Biosample; but biological and technical replicates are not unique BioSamples.

> For example, 23 000 unique 16S amplicons from a single seawater collection point would constitute one BioSample because they all share the same biological and physical properties.

The default **release date** is **Release immediately following processing**, but you can select a specific date for releasing your data. If you don’t know the exact data you can change it even after having finished the submission by clicking on the [***Manage tab*** at the Submission Portal](#changing).

A BioProject can share BioSamples with others BioProjects and BioSamples can belong to more than one BioProject. You would choose to have a BioSample in several BioProjects if, for example, the sequences were used to answer different research questions/goals which are described in separate BioProjects. You may also have a BioProject to which you already deposited data but want to deposite new BioSamples.

<img src=".\First time upload images\diagram.png" width=80% height=80%>

Depending on your answers at this step, the next steps would follow one of these pathways:

<img src=".\First time upload images\pathway-map.png" width=80% height=80%>

#### Step 3. Project (BioProject) information<a name="bioproject"></a>

<img src=".\First time upload images\bioproject-info.png" width=80% height=80%>

At the **Public description** provide information that best describes your research, which will become the description of your BioProject. If you have an **abstract** or research summary of your research project, you should add it here. Also, we recommend that at **URL** you add the DOI link to any publication of yours that is related to this data. 

#### Step 4. BioSample type<a name="biotype"></a>

In this step, you will select a **Package** that best fits the nature of your Biosample. According to your selected package the Submission Portal will supply you with a customized **attribute table** for the [next step](#bioattributes) that best describes the context of your BioSamples.

For the **Datathon**, please select the package ***MIMARKS Survey related***. At the displayed drop-down menu, select the sample type that better describes your sample.

<img src=".\First time upload images\biosample-type-section.png" width=70% height=70%>

#### Step 5. BioSample attributes <a name="bioattributes"></a>

At this step, you will provide contextual information about your BioSamples. 

<img src=".\First time upload images\biosample-attribute.png" width=80% height=80%>

For the **Datathon**, select ***Uploading a file using Excel format*** and use the custom Excel File we will provide called ***MIMARKS.survey.soil.5.0_Dathaton.xlsx***. Please read the instructions included in the excel carefully before filling in the values. Remember that you can only upload the tab-delimited text file version of the tab **MIMARKS.survey.soil.5.0**.

> Remember that, if for example, you have amplicon sequences from a single seawater collection point, that constitutes a single BioSample. In this example, at the **attribute table**, you would add the contextual information for the single BioSample.

The **sample_name** you give each Biosample in the attribute table will be again used at the **SRA metadata table** to link the specific sequences to the BioSample they come from. The sample name must be the same in both Excel files for them to be linked together.

##### Possible Errors at this step <a name="errors1"></a>

> ***Error: Multiple BioSamples cannot have identical attributes***

**Problem**

After filling out values for attributes provided in the template, your samples are not distinguishable by at least one or a combination of attributes.

**Solution**

Make sure the combined value of all attributes is unique for each Biological sample while taking into account that **sample name**, **sample title**, and **description** are not included in this check for uniqueness of the sample's attributes. If this problem arises because of biological replicates, please add a replicate column to the sheet and record the replicate numbers to differentiate them.

>***Error: Multiple BioSamples cannot have identical attributes***

**Problem**

In your current SRA submission, you have re-created samples that duplicate samples you already registered elsewhere, and the Submission Portal is preventing you from creating duplicates.

**Solution**

This would be the case if you had already deposited the BioSample under another BioProject. If you want to include an existing BioSample in the new BioProject, go back to the [General Info tab](#general) and select *Yes* to the question *Did you already register BioSamples for this data set?*. The SRA Submission Wizard will then skip the BioSample type and attributes steps.

At the [SRA metadata step](#metadata), and if you are using the **SRA_metadata_Datathon.xlsx**, you need to change the name of the first column from **sample_name** to **biosample_accession**. Then you can add the existing BioSample's accession numbers **(SAMN#)** to link the new sequence files to the already existing BioSamples; and to include them in the new BioProject. 

To find the accession numbers of Biosamples you already registered go to the [Submission Portal](#accessingsra) and follow the next steps: 

1. Click ***My submissions***.

<img src=".\First time upload images\portal-submissions.png">

2. Click at ***objects*** in the BioSample section of the Project. 

<img src=".\First time upload images\my-submissions.png">

#### Step 6. SRA Metadata<a name="metadata"></a>

The SRA metadata describes the technical aspects of each sequencing experiment: the sequencing libraries, preparation techniques, and the names of the data files. 

<img src=".\First time upload images\sra-metadata.png" width=80% height=80%>

For the **Datathon**, select ***Uploading a file using Excel format*** and use the custom Excel File called **SRA_metadata_Dathaton.xlsx**. Please read the instructions included in the excel carefully before filling in the values. You can only upload thetab-delimited text file version of the tab **SRA data**.

When submitting the project, the most descriptive information is captured at the level of the SRA **Experiment** for each separated sequence and is displayed in the public record. Here is an example to better understand the organization of the sequence data in excel:

> Six sequencing libraries were prepared from a single biological sample (the Biosample). Three were single-end libraries, and three were paired-end, although the paired-end libraries were sequenced using both paired and unidirectional sequencing. Two single-end libraries were treated using a targeted selection approach for some runs. Libraries were sequenced on two different instruments at three sequencing labs. There are 13 combinations of **library + sequencing strategy + layout + instrument model**. Each combination represents a unique **Experiment**.

##### Recommendations to avoid common errors when submitting SRA metadata <a name="avoiderrors"></a>

- Paired-end data files (forward/reverse) must be listed together in the same **Run** (in the case of the excel in the same row) for the two files to be correctly processed as paired-end. All data files listed in a **Run** will be merged into a single **sra archive file**. Therefore, files from different samples or experiments should not be grouped in the same **Run**.

- File name(s) for the **Experiments** shouldn’t contain any sensitive information, because they will appear publicly on the Google and AWS clouds.

- Avoid submitting duplicated files because the Portal does not accept this, and such files may be suppressed without warning.

##### Submitting in new BioSamples vs submitting to already existing ones <a name="newvs"></a>

When submitting new BioSamples, at the [BioSample attributes step](#bioattributes), a specific name for each Biosample was given on the **sample_name** column on the **MIMARKS.survey.soil.5.0_Dathaton.xlsx** file. At SRA Metadata step, on the **SRA_metadata_Dathaton.xlsx** excel file, the **sample_name** must match that given to the new BioSample, to correctly link the sequence data to the BioSample that describes their biophysical context.

If, on the other hand, you want to submit new sequences to already existing BioSamples, you have to change the first’s column name on the **SRA_metadata_Dathaton.xlsx** file from **sample_name** to **biosample_accession**. Then you can add the existing BioSample's accession numbers **(SAMN#)** to link the new sequence files to the already existing BioSamples; and to include them in the new BioProject. How to find the accession numbers of your BioSamples was explained at the [BioSample attributes step](#bioattributes).

##### Explanation of the elements of a public display at a single SRA Sample <a name="elementssra"></a>

<img src=".\First time upload images\experiment-display-long.png">

#### Step 7. Files <a name="files"></a>

In the step, you will upload the files listed in the **SRA Metadata excel file**. Files can be compressed using gzip or bzip2 and may be submitted in a tar archive, but archiving and/or compressing your files is not required. Uploading zip files is not permitted. If you are uploading a tar archive, list each file name, not the archive name.

<img src=".\First time upload images\uploading-files.png">

We recommend you use the ***Web browser upload via HTTP or Aspera Connect plugin*** option to upload the files, unless you have more than 10 GB of data or more than 300 files.

Also, we recommend you select ***Autofinish submission*** once the files have been successfully uploaded. Take into consideration that depending on the size and number of files, the uploading may take from several minutes to a few hours to get uploaded. 

Don’t forget to press ***Continue*** to save your progress. Otherwise you have to upload the files again.

##### Possible Errors or Warnings at this step <a name="errors2"></a>

> ***Warning: You uploaded one or more extra files that are not in your Metadata table***

**Problem**

You have uploaded files not listed in your SRA Metadata template. 

**Solution**

If you do not intend to include these files in your SRA submission, click ***Continue***. All files not included in the SRA Metadata will be ignored. If you intend to include these files in your SRA submission, return to the [SRA Metadata step](#metadata) and update their names.

> ***Error: Some files are missing. Upload missing files or fix metadata table***

**Problem**

The program does not find all files listed in the SRA Metadata table in your submission folder.

**Solution**

Upload files that are reported missing. Also, check that filenames listed in your metadata table, and make sure that the file extensions (.fq, .fastq, .sff, etc.) exactly match those of the files you want to upload. In the latter case, go back to the [SRA Metadata tab](#metadata), delete your metadata file and upload a new one with the correct filenames. Click ***Continue***. 

> ***Error: File <filename> is corrupted. Please re-upload the file...***

**Problem**

This Error occurs either because you have corrupt files on your side or the files became corrupted during transfer. 

**Solution**
	
Re-upload the files that were reported corrupt. For this, click the Fix button and follow the instructions. The filenames must be the same. Before re-uploading, please check the files for integrity on your side. If the gzip utility reported an error, please find and upload an uncorrupted version of this file before proceeding. If the file is OK, please re-upload it.
	
#### Step 8. Review and Submit <a name="review"></a>
	
At this step you get to review your submission's summary and make sure that everything is correct. You can still return to and change any step of your submission at this stage by clicking on the corresponding tabs at the top.
	
<img src=".\First time upload images\submission-finished.png">
	
Click ***Submit*** when you are sure everything is correct. After submitting, future changes to the BioProject are limited or can only be achieved by contacting NCBI's service desk.
	
If, on the other hand, you want to delete the whole submission click ***Delete submission***. This is the only opportunity you will get for deleting the submission without having to email NCBI’s service desk.
	
## Accessing an unfinished submission <a name="unfinished"></a>

Follow the next steps:

1. While being logged in, go to [**NCBI's homepage**](https://www.ncbi.nlm.nih.gov/).

2. Click ***Submit***

3. At the Submission Portal click on ***My submissions***.

<img src=".\First time upload images\portal-submissions.png" width=80% height=80%>

4. Find the submission with the ***Unfinished Status*** that has the title of the submission or the **submission ID (SUB#)** you are looking for.

<img src=".\First time upload images\unfinished-submission.png">

## Processing of the submission<a name="processing"></a>

### The Project is being reviewed by NCBI’s staff<a name="reviewed"></a>

Once submitted, your submission is queued for processing, and you will get feedback probably 24 hours after submitting it. Note that if you created a BioProject or/and a BioSample submissions within the SRA Wizard, you would receive feedback from these first.

If your submission was successfully registered, you will receive the following email. 

<img src=".\First time upload images\email-1.PNG">

The project number you have been given **(PRJ#)** will remain the same from now on, but it will not appear to other users until NCBI's staff has fully processed it. We kindly ask you to provide the project number for the **Dathaton's database**.

### The Project has been accepted<a name="accepted"></a>

After the submitted data has been processed, you will receive the following email.

<img src=".\First time upload images\email-2.PNG">

Once the Project has been accepted, when someone searches for your project, the following information will be displayed.

<img src=".\First time upload images\seach-prj.png">

#### Public display and searchable elements of a BioSample<a name="publicbiosample"></a>

<img src=".\First time upload images\biosample-public.png">

The **BioSample (SAMN#)** is the identifier of specific Biosamples.
Clicking on ***Retrieve all samples from this project*** allows you to see all the other BioSamples associated to the BioProject.

### Public display and searchable elements of a SRA Experiment<a name="publicsra"></a>

<img src=".\First time upload images\experiment-display-short.png">

The marked elements are:

- **Experiment (SRX#)**: identifier of instrument and library information of a specific sample (SRS#).

- **Study (SRP#)**: identifier of a study within a BioProject.

- **Sample (SRS#)**: identifier of a sample of sequence data.

- **Run (SRR#)**: identifier of the data file(s) derived from sequencing a library described by the associated Experiment.

## Changing a submission<a name="changing"></a>

Follow the next steps:

1. While being logged in, go to [**NCBI's homepage**](https://www.ncbi.nlm.nih.gov/).

2.  Click ***Submit***

3. At the Submission Portal click on ***Manage data***.

<img src=".\First time upload images\portal-manage.png" width=80% height=80%>

4. Select the **BioProject (PRJNA#)** you want to update. You can also filter it by BioSamples at the ***BioSample tab*** or by Experiments at the ***SRA tab***. With these other filtering options the data shown by the Data Manager actually can't be edited. 

<img src=".\First time upload images\click-manage-data.png" width=80% height=80%>

The BioProject’s managing page allows you to:
	
- ***Edit*** fields that were written during the submission.
	
- ***Add*** information that was not written during the submission.
	
-***Edit*** most fields of the SRA Metadata. You have to check the boxes for the Experiments you want to modify first.

<img src=".\First time upload images\manage-data.png" width=80% height=80%>

If you want to add more data to an existing BioProject or Biosample, [create a new SRA submission](#accessingsra) and enter the accession number of the BioProject **(PRJNA#)** or the Biosample **(SAMN#)** when asked. This will ensure that the new data is linked to the existing BioProject.

If you want to change the attributes or withdraw a BioProject or BioSample that has already been submitted and not necessarily accepted, you have to conact bioprojecthelp@ncbi.nlm.nih.gov or biosamplehelp@ncbi.nlm.nih.gov for assistance in updating your BioProject or BioSample submission respectively.

A Submission represents a discrete act of depositing data (a transaction). The submission has a temporary non-public ID as a **SUB#**. You cannot add more data to a completed submission. To update a submission, contact sra@ncbi.nlm.nih.gov.

After the **Run** is fully loaded, neither its files can be replaced, nor filenames can be changed. You will have to submit new files in a separate submission using [existing BioProject and BioSample accessions](#general) and request withdrawal of the **Run** containing the old files.

## Downloading data<a name="dowloading"></a>	
	
# Downloading data corresponding to one accession number<a name="dowloadingone"></a>

As we have seen, NCBI supports the inclusion of exhaustive metadata when uploading data. Unfortunatly, it's not so easy to download all the files of a BioSample or BioProject in one go, you would usually have to dowload the Experiments one by one. For this reason, for downloading all data corresponding to an specific accession number, we recommend using the portal from the European Bioinformatics Institute  as part of the European Molecular Biology Laboratory [**(EMBL-EBI)**](https://www.ebi.ac.uk/). For this you would have to follow the next steps:

1. Access [**EMBL-EBI's homepage**](https://www.ebi.ac.uk/)

2. Write the accession code of the BioProject, BioSample or SRA you are interested in, and click ***Search***.

<img src=".\First time upload images\european-portal-search.png">

3. Scroll down and select the entry corresponding to the accession number you were looking for.

4. A shortened version of the metadata will be shown, as well as the files belonging to this accession number. For accessing the file's download option, scroll to the right at the sections with the list of files.

<img src=".\First time upload images\dowload-ebi.png">

5. Click ***Download All*** if you want to dowload all the **Experiments (SRR)** under this accession number. If you want to dowload only specific Experiments, select the corresponding check-boxes and click ***Download selected files***

<img src=".\First time upload images\ebi-download-scroll.png">
	
# Downloading data corresponding to several accession numbers<a name="dowloadingmore"></a>

To download large amounts of SRA data we recommend you use the [**SRA Toolkit**](https://github.com/ncbi/sra-tools/wiki).



