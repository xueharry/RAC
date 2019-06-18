# RAC
Work for the Harvard Royal African Company (RAC) research project, centered primarily on computational textual analysis of historical letters related to the RAC.

# Directory Structure
## Raw HTML
Digital versions of the original paper texts were scraped from [Oxford Scholarly Editions Online](http://www.oxfordscholarlyeditions.com/) using [Web Scraper](http://webscraper.io/). A dump of the scraped data in .csv format is stored in `raw_html`, organized by volume number.

## Jupyter Notebooks
The code for cleaning and data manipulation are contained within the following Jupyter Notebooks:

`Clean-Scraped.ipynb` - Extraction of letter numbers from raw HTML, extraction of letter text and joining with metadata based on volume and letter number.

## `csv` Directory
This directory contains various files of the text data at various stages of preprocessing, along with a hand-curated metadata file:
1. `csv/032818_RAC_Networks_Database.xlsx` - Hand-compiled metadata on the letters, with key information including unique identifiers (UID), date, place and author 
2. `csv/texts.csv` - Extracted letter texts with corresponding volume and letter number in .csv format.
3. `metadata_text_merged.csv` - Joined data file of the text file `texts.csv` and the metadata file, joined on volume number and letter number. **This should be the primary reference data file.**

# Questions?
Email wenzhexue2014@gmail.com

