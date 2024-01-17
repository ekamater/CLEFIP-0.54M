# CLEFIP-0.54M
The CLEFIP-0.54M is subpart of the CLEFIP 2011 test collection http://www.ifs.tuwien.ac.at/~clef-ip/download/2011/index.shtml special made for patent classification.
## Description
The CLEFIP-0.54M dataset contains 6 csv files with data coming from 541,131 patents originated from the CLEFIP 2011. More specifically, the data comes from the latest documents/versions of these 541,131 patents that have simultaneously the main classification code, an EN abstract, EN description, EN claims, EN title, applicants and inventors. Moreover, the text of EN abstract, EN description, and EN claims has undergone a further preprocessing removing any character that is not alphabetic and removing English stopwords.
## Details about the dataset's content
Each csv file had initially two columns: the main IPC classification code and the text of a patent section, i.e., abstract, description, claims, title, applicants and inventors. 

In the latest release of the database, each csv has four columns: the ucid, the text of a patent section, the main classification code and all ipcr codes. The main classification code and ipcr codes were given at the subclass (3rd) level, the ucid refers to the latest patent document/version available for that patent, and the text contains the 60 first words from the respective patent section after cleaning punctuation, symbols and numbers, and stop words for the abstract, the description and the claims, while no preprocessing of text has been performed for the title, applicants and inventors. Moreover, the information for the main classification code has been extracted from the "main-classification" field of the patent document, while the ipcr codes gathers classification codes extracted from the "main-classification", "further-classification" and "classifications-ipcr" fields of the patent document.
The stop words used are available here: https://drive.google.com/file/d/1QgVcHXTiCdf1mDewqd39g2CHDVqfeUKO/view?usp=drive_link.

The patent data were initially tranferred in a SQL database using the steps described here: https://github.com/ekamater/CLEFIP2011_XML2MySQL

## Downloads
The latest version of the dataset is available here: https://drive.google.com/drive/folders/1Nk8p6zd_Hv4BbySsedB2I0eMrz2SBhjR?usp=drive_link

The previous versions of the dataset are available here: https://drive.google.com/drive/folders/1PyKsz9nCqLkpC7XGcp4rYxmHBJplbe83?usp=sharing

## Dataset's history
The dataset's history can be seen here: https://docs.google.com/document/d/1YYHNlQen3o20iSkBCMLQZcbWV8835pWA-sZWvT4g42w/edit?usp=drive_link
