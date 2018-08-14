# NeuroMetadataComparison
#### A python script for comparing metadata from the Neuromorpho DB. 
***
Created By: Usama Nasir Saifi.

For questions/comments you can reach me at u.saifi@rutgers.edu
***

### Instructions for Windows:

1. Install Python 3.5.2 from https://www.python.org/ftp/python/3.5.2/python-3.5.2-amd64.exe
2. Once Python 3 has been installed, you need to install NumPy and Pandas. This can be done from the command prompt by using the following commands:
    - Open the command prompt and write : **pip install numpy**
    - Open the command prompt and write : **pip install pandas**

### Usage
1. Place the excel metadata file and metacompare.py in the same directory.
2. Open command prompt and navigate to the directory. Then write **py metacompare.py path_to_excel_file sheetname with metadata**
*For the example in this repo, this would be: py metacompare.py glia.xlsx Metadata*

This will write a new sheet to the original excel file with the comparisons in a matrix format.

### Data Format Considerations

- In the first column (A), the feature rows that need to be compared should have integers next to them.
![alt text](https://github.com/uns1/NeuroMetadataComparison/blob/master/readme_images/ColInt.PNG)

- In the first row (1), the group numbers should be integers with no strings or other text i.e. should just be numbers from 1 to n.
![alt text](https://github.com/uns1/NeuroMetadataComparison/blob/master/readme_images/GrpInt.PNG)

- After the last row of feature data, there should be no data in the sheet. This is vital for Pandas to correctly read the data in the excel file.
![alt text](https://github.com/uns1/NeuroMetadataComparison/blob/master/readme_images/NoDat.PNG)

*In the attached images, the highlited rows and/or columns are the ones the I'm talking about*
