# Azure Data Factory Project

In our Azure Data Factory (ADF) project, we are designing and implementing data pipelines and data flows to orchestrate and transform data across multiple sources and destinations. The pipelines manage end-to-end data movement, while the data flows handle complex transformations such as joins, aggregations, lookups, and surrogate key generation to ensure clean, consistent, and analytics-ready data.



A-copy activity ->from blob to blob and also perform Copy_Activity_From_Github in which take data from Git-Hub website directly and store into blob storage.copy data from one loc/GitHub website to another loc/folder/storage using copy activity by http connection

<img width="1255" height="615" alt="P2" src="https://github.com/user-attachments/assets/3f77e4cb-3905-4b50-ba0a-7f06f92cd7c0" />


B-Get Metadata Activity-> to  want specific files from folder and then using for each to iterate file one by one and if file match with IF condition then copy data from sink folder.Get metadata activity and then use if condition and for each activity to fetch specific file name
Data Flow is like a visual drag-and-drop tool to design how your data should be transformed and moved, without writing a lot of complex code. If u want to apply transformation on data we will use data flow And then Set up trigger to run pipeline with particular timeline

<img width="1677" height="616" alt="image" src="https://github.com/user-attachments/assets/97968c07-8026-4db8-8469-ed2901c9f6d2" />


C-Set Variable Activity-> used to store information like filename and size etc.if you want specify files into your specific location/folder 
if you are performing get metadata activity like all child items and i want to store information in variable we will use set variable activity and you can store anything

<img width="1682" height="627" alt="image" src="https://github.com/user-attachments/assets/70c94442-ed5f-4e52-bcc0-4ff72aa3135e" />


D-Execute Pipeline Activity-> If we want to run pipeline within pipeline then we will use this activity. Execute Pipeline activity is used when you want one pipeline to run another pipeline.

<img width="1688" height="601" alt="image" src="https://github.com/user-attachments/assets/685fc9b2-b8b7-4649-ad22-9f30fae04724" />


E-Join transformation->when u combine data based on column basis

<img width="1750" height="613" alt="image" src="https://github.com/user-attachments/assets/e7b11564-856e-423f-b2a1-a9d31caa5eaf" />

F-Append Variable activity empowers you to dynamically add or concatenate values to existing variables

<img width="1203" height="622" alt="image" src="https://github.com/user-attachments/assets/5b76de49-0ea8-492f-8e65-0387428f1b27" />

G-Swict Activity->we have input folder in which employee and department file we want to store specific file into specific folder ex-employee folder goes into employee file

<img width="1805" height="693" alt="image" src="https://github.com/user-attachments/assets/2761368a-2924-4d69-9ef7-a707b9a6e0b8" />

H-Validation Activity-> to ensure pipeline only continue execution once it has validated data attached, dataset reference exists , that meet specified criteria.

<img width="1813" height="672" alt="image" src="https://github.com/user-attachments/assets/bfb567de-fc5c-4dc8-9f4f-b19bc0066e67" />

I-Pivot Transformation-> Pivot is a transformation in Mapping Data Flow that turns row data into columns.Unpivot is a transformation used to convert columns into rows.

<img width="1710" height="558" alt="image" src="https://github.com/user-attachments/assets/abc83d95-1ef5-4917-a25a-0ef2129fa24a" />

J-surrogate key-> as a simple ID tag you give to each row in a table, just to keep track of it — even if the real data doesn’t have a unique identifier.A new column with unique IDs generated inside a Mapping Data Flow.
It’s not taken from your source data — ADF creates it for you automatically.
Usually used in data warehousing to give each row a simple unique key (like 1, 2, 3…) even when no natural key exists.


<img width="1750" height="628" alt="image" src="https://github.com/user-attachments/assets/312f8e21-6dcc-4b43-813f-12c9bfa5da8e" />

K-> SCD-TYPE1 DATA FLOW->It is a technique in data warehousing to manage and track historical changes in dimension tables, commonly implemented as Type-1 (overwrite)

<img width="1732" height="616" alt="image" src="https://github.com/user-attachments/assets/9bce9353-b533-493e-b311-c902d557f687" />

L-> WINDOW TRANSFORMATION->to similar to SQL window functions (ROW_NUMBER, RANK, LAG, LEAD, running totals, moving averages, etc.).

<img width="1756" height="610" alt="image" src="https://github.com/user-attachments/assets/f4c15c11-7c90-493b-a396-cf56e93fe376" />










