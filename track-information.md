# General

### License
We ask the participants to work under the MIT licence so that we can re-use the code for future data pre-processing. 
If participants used pre-existing code or work, they should credit the original author and be aware of licenses of the source. 
When in doubt, contact [Jonathan de Bruin](https://github.com/J535D165).

### Scoring form
All proposed solutions will be assessed on the following key points:
1. Deliverables: were they submitted in time?
2. The proposed idea/solution as a concept
3. Cleanliness of code
4. Documentation of code
5. Structure of GitHub repository
6. Clearness of the readme (intended for someone with minimal coding experience) 
7. Re-usability of the script
8. Final Pitch/Presentation
9. Is the repository public
10. Track specific bonus

Each key point is worth a maximum of 10 points, thus the maximum score is 100.

# Track specific information
## Track 1: Data pre-processing


*Track Lead: [Jelle Teijema](https://github.com/JTeijema)*

*Track Expert: [Jonathan de Bruin](https://github.com/J535D165)*

### Background
Before we can do anything with the data, for example in Track 2 and 3, there has to be some pre-processing. 
The raw data is quite challenging, containing much noise and little structure. 
Most data is raw email HTML, combined with a header. Wob requests (Wet openbaarheid van bestuur - translates to: Government Information (Public Access) Act) 
also allow for the censoring of some personal data, so some email addresses and personal names are scrubbed. 

Still, a real treasure trove of information is hidden within the mess. 
Available are at least titles, IDs, message types, message content, multiple date formats (which aren’t always the same for a single entry!), 
locations and more. Documents are labeled on correspondence, reports, permits, governmental decisions and special documents.

### Provided materials 
For this track participants can use the raw data as provided by FTM.

### Anticipated Output
The anticipated output of Track 1 is a script that processes the raw data, as provided by FTM, in such a way that it can be used for Track 2 and 3. 

Rows in the data should be the different records (files/documents) and the there should be two columns:
‘title’: This could be the subject of a document or the title of an email.
‘abstract’: Containing the text in the document/email. 
Moreover, the output file should either be in a tabular format with extensions .csv, .tab, .tsv, or .xlsx. CSV and TAB files are preferably comma, semicolon, 
or tab-delimited. The preferred file encoding is UTF-8 or latin1.

It is completely up to you how the data is pre-processed, as long as it is cleaner than [the one Jelle Teijema prepared](link to dataset).

### Scoring bonus points
Is the dataset cleaner than the one pre-processed by [Jelle Teijema](https://github.com/JTeijema)?

## Track 2: Visualization
*Track lead/expert: [Sofie van den Brand](https://github.com/SagevdBrand) & [Laura Hofstee](https://github.com/LHofstee)*

### Background
Outside of reading all the documents, visualization is also a very useful tool to identify the relations between the documents. 
From [semantic clusters](link to semantic cluster when done) (applied to the CORD-19 database for example) to [wordclouds](https://github.com/asreview/asreview-wordcloud) 
(for example as implemented in ASReview), a visualization can say more than 1000 words. 

### Provided materials 
For this track participants can use the [pre-processed data](link here). 

### Anticipated Output
As visualization is a mainly creative track, there is no clear pre-defined anticipated output. 
However, the visualization(s) should aim to showcase relations between the contents of the documents in such a way that FTM could put it on their website! 
No presentation needed, the visualization should explain it all. 

### Scoring bonus points
Re-usability for future datasets of FTM.

## Track 3: Smart Screening
*Track lead: [Otto Mättas](https://github.com/ottomattas)*

*Track expert: [Rens van de Schoot](https://www.rensvandeschoot.com/)*

### Background
Follow the Money currently uses crowdsourcing to analyze all the different documents of the Shell Papers. This means that people can read any and all files in any order. 

### Anticipated Output
The goal of the third track is to provide FTM with a pipeline that allows for faster screening of the documents. For example, instead of randomly reading one document after another, it would be far more helpful to read documents ranked by, for example, relevance.  One option  is to create a plug-in for ASReview like we did for the covid-19 dataset. Do you have any other cool ideas about what could be done with the data, or if you have completely different ideas on how to use ASReview? Go for it, let’s hack ASReview!

### Provided materials 
For this track participants can use one or all of the [datasets we prepared](https://github.com/asreview-ftm-hackathon/Data). This data is actually [constructed out of the first dataset](https://github.com/ftmnl/asr). The 10 datasets resemble the many different [datasets FTM will eventually collect](https://www.ftm.nl/dossier/shell-papers#wob-verzoeken). 

### Scoring bonus points
Does the pipeline make multiple datasets available?
