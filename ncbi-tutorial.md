# Submitting 16S rRNA sequence data to the National Library of Medicine (NCBI) for the first time

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
		8. [Step 8. Review and Submit](#review)
4. [Accessing an unfinished submission](#unfinished)
5. [Processing of the submission](#processing)
	1. [The Project is being reviewed by NCBI’s staff](#reviewed)
	2. [The Project has been accepted](#accepted)
		1. [Public display and searchable elements of a BioSample](#publicbiosample)
		2. [Public display and searchable elements of a SRA Experiment](#publicsra)
6. [Changing a submission](#changing)
7. [Downloading data](#dowloading)

## Registering to NCBI <a name="registering"></a>

To register to NCBI follow the next process:

- [**Access NCBI's homepage**](https://www.ncbi.nlm.nih.gov/) and select ***Log in***.

<img src=".\First time upload images\home-login.png">

- A menu with several lo Login options will be displayed. You can choose whichever you prefer for setting your account.

<img src=".\First time upload images\login-options.PNG">

## Accessing the Sequence Read Archive (SRA) <a name="accessingsra"></a>

For accessing the Sequence Read Archive (SRA) follow the next steps:

- While being logged in, [**Access NCBI's homepage**](https://www.ncbi.nlm.nih.gov/). ***write 16S rRNA*** 

- Select ***Submit***.

<img src=".\First time upload images\home-submit.png">

- The main page of the Submission Portal will be displayed. For the occasion of the Datathon, ***write 16S rRNA*** in the search bar and ***select SRA***. This leads to the Sequence Read Archive, which specializing in managing data such 16S rRNA.

<img src=".\First time upload images\portal-submit.png">
 
-  A webpage with information on the Sequence Read Archive (SRA) will be displayed. Select ***Submit***.

<img src=".\First time upload images\sra-submit.png">

## Submitting data to SRA Submission Wizard] <a name="submittingwizard"></a>

### Aspects to consider before submitting data <a name="aspects"></a>

- If human data comes from a metagenomic study, donor consent is necessary.

- Each upload must be kept under 5 TB, if you have more, split the upload across multiple submissions.

- Submissions can be linked to the same BioProject to ensure all data are searchable with a single accession code.

- Every fastq file should be less than 100 GB in size. If compressed files are larger than 100 GB, please split them before submission.

### Submitting data <a name="steps"></a>

For every step, you will have to add information or files; whenever you want to save your progress, you must press ***Continue***. You can review or make changes to your previous steps during submission by clicking on the preceding tabs.  

At any point, after having saved your progress, you can leave NCBI and [continue the process of submission later](#unfinished). If, however, you click the ***Submit*** button at the last step, [making changes would follow other routes](#changing). 

You may get *Error* or *Warning* messages when saving your progress. Error messages describe the Error and suggest a solution that must be corrected before you can move to the next step of your submission. On the other hand, the Warning messages attempt to prevent you from making a possible mistake and do not block you from continuing your submission. 

#### Step 1. Submitter <a name="submitter"></a>

The submitting person will be asked for personal information at this step. At the fields signaled in the following picture we recommend using you institutional **e-mail** and writting the name of the **institution** you work for.

<img src=".\First time upload images\submitter.png" width=70% height=70%>

#### Step 2. General Information <a name="general"></a>

<img src=".\First time upload images\general-info.png" width=60% height=60%>

The **BioProject** represents the research project from which the sequence originated.The information supplied in the **Biosample** provides context to your experimental data. Every metagenome, time point, tissue type, or treatment type must has its Biosample; but biological and technical replicates are not unique BioSamples.
> For example, 23 000 unique 16S amplicons from a single seawater collection point would constitute one BioSample because they all share the same biological and physical properties.

The default **release date** is “Release immediately following processing”, but you can select a specific date for releasing your data. If you don’t know the exact data you can change it even after having finished the submission by clicking on the [***Manage tab*** at the Submission Portal](#changing).

A BioProject can share BioSamples with others BioProjects and BioSamples can belong to more than one BioProject. You would choose to have a BioSample in several BioProjects if, for example, the sequences were used to answer different research questions/goals which are described in separate BioProjects. You may also have a BioProject to which you already deposited data but want to deposite new BioSamples.

<img src=".\First time upload images\diagram.png" width=60% height=60%>

Depending on your answers at this step, the next steps would follow one of these pathways:

<img src=".\First time upload images\pathway-map.png" width=70% height=70%>

#### Step 3. Project (BioProject) information<a name="bioproject"></a>

<img src=".\First time upload images\bioproject-info.png" width=70% height=70%>

At the **Public description** provide information that best describes your research, which will become the description of your BioProject. If you have an **abstract** or research summary of your research project, you should add it here. Also, we recommend that at **URL** you add the DOI link to any publication of yours that is related to this data. 

#### Step 4. BioSample type<a name="biotype"></a>

In this step, you will select a **Package** that best fits the nature of your Biosample. According to your selected package the Submission Portal will supply you with an *attribute table* for the [next step](#bioattributes) that best describes the context of your BioSamples.

For the Datathon, we kindly ask you to select the package ***MIMARKS Survey related***. You can select the sample type from the drop-down menu that better describes your sample.

<img src=".\First time upload images\biosample-type-section.png" width=50% height=50%>

#### Step 5. BioSample attributes <a name="bioattributes"></a>

At this step, you will provide contextual information about your BioSamples. 
> If for example, you have 23000 16S amplicons from a single seawater collection point, they would constitute a single BioSample because 1 sample was collected and then analyzed to deduce 16S diversity.

In this example, at the attribute table, you would add the contextual information for the single BioSample. The **sample_name** you give each Biosample in the attribute table will be again used at the **SRA metadata table** to link the specific sequences to the BioSample they come from. The sample name must be the same in both Excel files for them to be linked together.

<img src=".\First time upload images\biosample-attribute.png" width=80% height=80%>

For the Datathon, select ***Uploading a file using Excel format*** and use the custom Excel File we will provide called ***MIMARKS.survey.soil.5.0_Dathaton.xlsx***. Please read the instructions included in the excel carefully before filling in the values. *Remember that you can only upload the tab-delimited text file version of the tab "MIMARKS.survey.soil.5.0".*

##### Possible Errors at this step <a name="errors1"></a>

> ***Error: Multiple BioSamples cannot have identical attributes***

**Problem**

After filling out values for attributes provided in the template, your samples are not distinguishable by at least one or a combination of attributes.

**Solution**

Make sure the combined value of all attributes is unique for each Biological sample while taking into account that "sample name," "sample title," and "description" are not included in this check for "uniqueness" of the sample's attributes. If this problem arises because of biological replicates, please add a replicate column to the sheet and record the replicate numbers to differentiate them.

>***Error: Multiple BioSamples cannot have identical attributes***

**Problem**

In your current SRA submission, you have re-created samples that duplicate samples you already registered elsewhere, and the Submission Portal is preventing you from creating duplicates." 

**Solution**

This would be the case if you had already deposited the BioSample under another BioProject. If you want to include them inside the new BioProject, go back to the General Info tab and select “Yes” to the question “Did you already register BioSamples for this data set?” . The SRA Submission Wizard will then skip the BioSample type and attributes steps.

At the SRA metadata step, and if you are using the “SRA_metadata_Datathon.xlsx”, you need to change the name of the first column from "*sample_name" to "biosample_accession”. Then you can add the existing BioSample's accession numbers (SAMN#) to link the new sequence files to the already existing BioSamples; and to include them in the new BioProject. 

To find the accession numbers of Biosamples you already registered go to the Submission Portal and follow the next steps: 

1. Click ***My submissions***.

2. Click at ***objects*** in the BioSample section of the Project. 

<img src=".\First time upload images\my-submissions.png">

#### Step 6. SRA Metadata<a name="metadata"></a>

The SRA metadata describes the technical aspects of each sequencing experiment: the sequencing libraries, preparation techniques, and the names of the data files. 

For the Datathon, select ***Uploading a file using Excel format*** and use the custom Excel File called **SRA_metadata_Dathaton.xlsx**. Please read the instructions included in the excel carefully before filling in the values. You can only upload thetab-delimited text file version of the tab "SRA data".

<img src=".\First time upload images\sra-metadata.png" width=80% height=80%>

When submitting the project, most descriptive information is captured at the level of the SRA **Experiment** for each separated sequence and is displayed in the public record. Here is an example to better understand the organization of the sequence data in excel:

> Six sequencing libraries were prepared from a single biological sample (the Biosample). Three were single-end libraries, and three were paired-end, although the paired-end libraries were sequenced using both paired and unidirectional sequencing. Two single-end libraries were treated using a targeted selection approach for some runs. Libraries were sequenced on two different instruments at three sequencing labs. There are 13 combinations of **library + sequencing strategy + layout + instrument model**. Each combination represents a unique **Experiment**.

##### Recommendations to avoid common errors when submitting SRA metadata <a name="avoiderrors"></a>

- Paired-end data files (forward/reverse) must be listed together in the same **Run** (in the case of the excel in the same row) for the two files to be correctly processed as paired-end. All data files listed in a **Run** will be merged into a single .sra archive file. Therefore, files from different samples or experiments should not be grouped in the same **Run**.

- File name(s) for the **Experiments** shouldn’t contain any sensitive information, because they will appear publicly on the Google and AWS clouds.

- Avoid submitting duplicated files because the Portal does not accept this, and such files may be suppressed without warning.

##### Submitting in new BioSamples vs submitting to already existing ones <a name="newvs"></a>

When submitting new BioSamples, at the “BioSample attributes” step, a specific name for each Biosample was given on the “sample_name” column on the MIMARKS.survey.soil.5.0_Dathaton.xlsx Excel file. At SRA Metadata step, on the SRA_metadata_Dathaton.xlsx Excel file, the “sample_name” must match that given to the new BioSample, to correctly link the sequence data to the BioSample that describes their biophysical context.

If, on the other hand, you want to submit new sequences to already existing BioSamples, you have to change the first’s column name on the SRA_metadata_Dathaton.xlsx’s excel file from "*sample_name" to "biosample_accession”. Then you can add the existing BioSample's accession numbers (SAMN#) to link the new sequence files to the already existing BioSamples; and to include them in the new BioProject. How to find the accession numbers of your BioSamples was explained at the BioSample attributes step.

##### Explanation of the elements of a public display at a single SRA Sample <a name="elementssra"></a>

<img src=".\First time upload images\experiment-display-long.png">

#### Step 7. Files <a name="files"></a>

In the step, you will upload the files listed in the SRA Metadata Excel file. Files can be compressed using gzip or bzip2 and may be submitted in a tar archive, but archiving and/or compressing your files is not required. Uploading zip files is not permitted. If you are uploading a tar archive, list each file name, not the archive name.

<img src=".\First time upload images\uploading-files.png">

We recommend you use the ***Web browser upload via HTTP or Aspera Connect plugin*** option to upload the files, unless you have more than 10 GB of data or more than 300 files.

Also, we recommend you select ***Autofinish submission*** once the files have been successfully uploaded. Take into consideration that depending on the size and number of files, the uploading may take from several minutes to a few hours to get uploaded. 

Don’t forget to press ***Continue*** to save your progress. Otherwise you have to upload the files again.

#### Step 8. Review and Submit <a name="review"></a>
This is a sub paragraph, formatted in heading 3 style

## Accessing an unfinished submission <a name="unfinished"></a>
The first paragraph text

## Processing of the submission<a name="processing"></a>
The first paragraph text

### The Project is being reviewed by NCBI’s staff<a name="reviewed"></a>
The first paragraph text

### The Project has been accepted<a name="accepted"></a>
The first paragraph text

#### Public display and searchable elements of a BioSample<a name="publicbiosample"></a>
The first paragraph text

### Public display and searchable elements of a SRA Experiment<a name="publicsra"></a>
The first paragraph text

## Changing a submission<a name="changing"></a>
The first paragraph text

## Downloading data<a name="dowloading"></a>
The first paragraph text
