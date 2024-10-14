# FastSearch
A tool that parses into your large folders, identifying every sentence with your target word and tracking its file location.

### Overview
An adaptable framework for searching keywords across multiple document types, including PDFs, Word, and Excel files. The code utilizes parallel processing to speed up the task by processing files concurrently.

### Libraries Used
os: To navigate and interact with the file system.
glob: For finding file paths that match specific patterns.
python-docx: To read and search through Word (.docx) files.
openpyxl: To handle Excel (.xlsx) files.
PyMuPDF (fitz): For extracting text from PDF files.
concurrent.futures (ThreadPoolExecutor): For parallel processing to improve efficiency.


### Instructions 
Insert Folder Path: In the folder_path variable, replace the placeholder string with the path of the folder you want to search. This folder can contain subdirectories, and the script will search recursively.

Example:

python
Copy code
folder_path = r'C:\path\to\your\folder'


Insert Keywords: Modify the keywords list with the words or phrases you want to search for in the documents. You can include multiple keywords by adding them to the list.

Example:

python
Copy code
keywords = ['keyword1', 'keyword2']