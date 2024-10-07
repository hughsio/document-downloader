# Document Downloader

## Introduction

This is **Document Downloader**, a Python script designed to scrape a website, find specific documents (like PDFs, Word docs, and Excel sheets), and download them automatically. Whether you're gathering research material, reports, or any kind of documents from the web, this tool will streamline the process for you.

## How It Works

Here's a quick rundown of what this script does:

1. **Website Scraping:** It connects to the website of your choice and looks for document links.
2. **File Filtering:** It specifically targets files with `.pdf`, `.docx`, and `.xlsx` extensions, making sure you only download the documents you need.
3. **Download Process:** Files are downloaded to a specified folder. Each file's size is checked to ensure it's under 120MB, preventing storage issues.
4. **Retries on Failure:** If a download fails, the script will retry up to three times before moving on to the next file.
5. **Zipping:** After downloading, it compresses the documents into a zip file for easy access and sharing.

## Setup

## Setup

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/hughsio/document-downloader.git
   cd document-downloader
   ```

2. **Install Dependencies:**
   This project uses a `requirements.txt` file to manage dependencies. To install them, run:
   ```bash
   pip install -r requirements.txt
   ```
   This will install all necessary packages, including beautifulsoup4, requests, and their dependencies.


3. **Run the Script:**
   Once you’ve set everything up, simply run:
   ```bash
   python downloader.py
   ```

## Customization

- **Website URL:** Modify the `website_url` variable in the script to point to the website you're interested in scraping.
- **Download Location:** Change the `output_directory` to specify where you want to save the downloaded files.
- **File Size Limit:** Adjust the `max_file_size` variable to control the maximum allowable file size.

## Why I Built This

The **Document Downloader** project came from a personal need to automate document collection from various sources online. I wanted to make a tool that could handle a variety of file types, retry failed downloads, and keep everything neatly organized with minimal effort. I hope this tool proves as useful for you as it has for me!
