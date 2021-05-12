# PDF-NER-annotation-extractor
Two main files that will be helpful to guide through the files would be :

- _File-Names and Summary  (this is a pdf file with a guide to which file is which and the tried approaches, this is more or less the full approach and guide along with the notebook comments below).
- _MAIN.html (this is the code notebook, with comments on what each cell does and why it is there.).

The above two files are important and this readme is made to direct to the summary(pdf) file above which details the approach.

"""
The problem:
To build an AI/ML model to extract data from the rental agreements. The rental agreements will be in different data formats and available in the form of PDFs to perform the extraction.

The model should be able to extract the following fields from all the documents,

Agreement Value
Agreement Start Date          
Agreement End Date            
Renewal Notice (Days)        
Party One  
Party Two

NOTE: Please do not use a rule-based/oriented approach (RegEx, static conditions etc).

The rental agreements are in the PDF format.
Training_data/: contains a total of 43 rental agreements
Validation_data/: contains a total of 8 rental agreements

CSV-output format: 
File Name, Agreement Value, Agreement Start Date, Agreement End Date, Renewal Notice (Days), Party One, Party Two

404_Sai Sadan_Rental Agreement, 15500, 26.06.2016, 31.04.2017, 30, Mr. RK Senthil Kumar, Mr. Sandipan Nandy Mazumdar

NOTE:

The Agreement Value column should have only the numeric value.
The Agreement Start & End Date should have the dd.mm.yyyy format
The File Name shouldn’t contain the file extensions   
5. Evaluation Criteria

Per field Recall (Training data) should be greater than 90%
Per field Recall (Validation Data) should be greater than 80%
Recall here refers to (Per Field)

True = Number of exact value matches for a document’s metadata given in the training/validation set to the extracted value by the system.
False = Number of Did not match or Not Extracted
Recall = (True)/( True + False)

"""
