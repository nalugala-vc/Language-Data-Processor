

# MASSIVE Dataset Processing Project (Group 5 ICS C)

This project involves the processing and transformation of the MASSIVE dataset. The main goals include setting up a Python development environment, generating language-specific Excel and JSONL files, and uploading results to Google Drive and GitHub.

## Table of Contents

- [Project Setup](#project-setup)
- [File Generation](#file-generation)
- [Uploads](#uploads)
- [Usage](#usage)

## Project Setup

### Dependencies 
- Python3
Go to the official Python website's download section:[python](https://www.python.org/downloads/ "Visit python")

- pandas 
```bash
pip install pandas
```
- openpyxl 
 ```bash
pip install openpyxl
```
- for Google Drive Api
```bash
pip install google-auth google-auth-oauthlib google-auth-httplib2 google-api-python-client
```


### Setting up the Development Environment(Optional)
- Set up a virtual environment:
- 1.Windows system:
- create the virtual environment
 
```bash
         python -m venv name_of_the_environment
```
- Activate
```bash
      .\name_of_the_environment\Scripts\activate
 ```
   
- 2.Linux Systems:
- create the virtual environment
```bash
            python3 -m venv name_of_the_environment
```
     
- Activate:
```bash
      source name_of_the_environment/bin/activate
```
- To Deactivate the environment in both Windows and linux Systems:
```bash
      deactivate
```



### Directory Structure

- `/dataset`: Contains the MASSIVE dataset file(s).
- `/scripts`: Python scripts for processing.
- `/output`: Output directory for resulting files.

## File Generation

### Excel Files (en-xx.xlsx)
For each language paired with English, a respective `en-xx.xlsx` file is generated containing the `id`, `utt`, and `annot_utt` columns.

### JSONL Files
For English (en), Swahili (sw), and German (de), individual `.jsonl` files are generated for test, train, and dev sets respectively.

### Large JSON File
A combined JSON file representing translations from English to other languages using the train sets is generated. It's pretty printed for better readability.

## Uploads

### Google Drive
Files can be uploaded to a designated Google Drive Backup Folder. If you're using `pydrive`, ensure you have set up the necessary OAuth credentials.

### GitHub
Ensure you have initialized a git repository, added your changes, committed them, and pushed to your GitHub repository.

## Usage

1. Place your dataset in the `/dataset` folder.
2. Run the Python scripts from the `/scripts` folder to perform dataset processing.
3. Check the `/output` folder for the generated files.
4. Use the provided utilities (or manually) to upload files to Google Drive and GitHub.

---

