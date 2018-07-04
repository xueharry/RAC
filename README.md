# RAC
Work for the Harvard Royal African Company (RAC) research project, centered primarily on computational textual analysis of historical letters related to the RAC drawn from OCR scans of the original texts

# Directory Structure
## Raw Text
OCR scans of the original paper texts were parsed into plaintext files using Adobe Acrobat. The raw plaintext (.txt) files are contained within the directory `First Law Scans Cropped`.

## Jupyter Notebooks
The code for cleaning and data manipulation are contained within the following Jupyter Notebooks:

`Segment-Text.ipynb` - Segmenting of the raw text into individual letters based on regular expression matching

`Clean-Text.ipynb` - Basic automated cleaning of section titles where titles were mistakenly included in the text body during the plaintext conversion process

`Join-Text-Database` - Joining of segmented and cleaned text with metadata based on volume and letter number

## `csv` Directory
This directory contains various files of the text data at various stages of preprocessing, along with a hand-curated metadata file:
1. `csv/032818_RAC_Networks_Database.xlsx` - Hand-compiled metadata on the letters, with key information including unique identifiers (UID), date, place and author 
2. `csv/segmented.csv` - Segmentation of text into individual letters based on regex matching
3. `csv/segmented_cleaned.csv` - Hand-cleaned version of `csv/segmented.csv' to address OCR to text parsing errors of section titles
4. `csv/segmented_with_numbers.csv` - Version of `segmented_cleaned.csv` with volume and letter numbers included
5. `metadata_text_merged.csv` - Joined data file of the text file `segmented_with_numbers.csv` and the metadata file, joined on volume number and letter number

# Questions?
Email wxue@college.harvard.edu

