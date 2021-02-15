CSYE7250 Big Data Architecture and Governance
Group 1
Dataset Topic: Covid-19
Authors: Chinmay Arolkar, Foram Javia, Aishwarya Kumar

### This Readme contains implementation instructions for the project submitted####

Contents of the file:
   ###( 1 to 5 are used in the below implementation instructions)
1. Data folder - Contains raw dataset
2. COVID-19_Dataset_Cleanup.ipynb - Notebook for data cleaning in Python
3. Cleaned_data folder - Contains dataset after cleanup
4. COVID-19_Data Visualization.ipynb - Notebook for data visualization in Python
5. Covid_neo4jscript.txt - Neo4j commands to create nodes, indices, unique constraints and relationships

   ###(Other deliverables)
6. SIT_UAT.xlsx - Excel containing SIT UAT test cases performed in Neo4j
7. Technical_Business_Metadata.xlsx - Excel containing Business metadata and Technical metadata(extracted from Neo4j)
8. Covid-19 Project.pptx - Final presentation document

############################

Implementation Instructions:

Source : https://github.com/nytimes/covid-19-data
The dataset used in the project is in Data folder. The dataset has data until Oct 13th. Access the above source link for the latest data.

Step 1 : Data Wrangling and Data Cleaning
	COVID-19_Dataset_Cleanup.ipynb - This notebook contains code for data wrangling, data cleaning and profiling
	Input : csvs in the 'Data' folder
	Output : csvs in the 'Cleaned_data'folder
	
	###Note : Make sure to include correct input and output paths. In the notebook, input path: /data/<name_of_csv>  output path: /data/output/<name_of_csv>

Step 2: Data Visualization
	COVID-19_Data Visualization.ipynb - This notebook contains code for data visulization
	Input : csvs in the 'Cleaned_data'folder
	Output : Graphs seen in the notebook

Step 3: Neo4j
	Input : csvs in the 'Cleaned_data'folder
	
	###Note : Install Neo4j using the document provided by Dr.Kambiz Hyderi
	1. Create database COVID-19. 
	2. Importing csvs into Neo4j - 
		Click on more options(3 dots) on the top right > Manage > Click on the drill down arrow beside 'Open Folder' tab > Select Import
		###This opens the import folder. Drag and drop csvs in this folder for use in your Neo4j.
	3. Click on the 'Start' button to start your  Neo4j database
		###This opens a browser wherein you can run commands to create nodes, relationships etc.
	4. Use the Covid_neo4jscript.txt file to create database elements mentioned. 
		###Run the code one by one

Step 4: Technical metadata obtained from step 3 is included in Technical metadata sheet in Technical_Business_Metadata.xlsx
	###Note: Technical metadata generated in Step 3 can be extracted. For this, refer 'TechnicalMetadata_Extract_Neo4j.txt' file in the Metadata Master folder. 
		 Metadata Master is another folder included in the submission on Canvas.

############# EOD ###############