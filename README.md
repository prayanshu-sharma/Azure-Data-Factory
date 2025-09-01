# Azure Data Factory Project

Azure Data Factory Project we are creating some data pipeline and dataflow
In this project
A-we are perform copy activity from blob to blob and also perform Copy_Activity_From_Github in which take data from Git-Hub website directly and store into blob storage.copy data from one loc/GitHub website to another loc/folder/storage using copy activity by http connection

<img width="1255" height="615" alt="P2" src="https://github.com/user-attachments/assets/3f77e4cb-3905-4b50-ba0a-7f06f92cd7c0" />


B-Get Metadata Activity to  want specific files from folder and then using for each to iterate file one by one and if file match with IF condition then copy data from sink folder.Get metadata activity and then use if condition and for each activity to fetch specific file name
Data Flow is like a visual drag-and-drop tool to design how your data should be transformed and moved, without writing a lot of complex code. If u want to apply transformation on data we will use data flow And then Set up trigger to run pipeline with particular timeline

<img width="1677" height="616" alt="image" src="https://github.com/user-attachments/assets/97968c07-8026-4db8-8469-ed2901c9f6d2" />


C-Set Variable Activity used to store information like filename and size etc.if you want specify files into your specific location/folder 
if you are performing get metadata activity like all child items and i want to store information in variable we will use set variable activity and you can store anything

D-Execute Pipeline Activity- If we want to run pipeline within pipeline then we will use this activity. Execute Pipeline activity is used when you want one pipeline to run another pipeline.

E-
