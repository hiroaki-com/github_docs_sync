# GitHub Docs Sync

A Google Colab notebook to automatically fetch documentation or source code from GitHub and save it to Google Drive.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1rFXK52rq7V8TD_iMT-JZ1qqLzlP5qnlx#scrollTo=JHKmCFrZfIPe)

## Overview

This tool allows you to sync data from specified GitHub repositories (or specific subdirectories) directly to your Google Drive without needing a local environment.

**Primary Use Cases:**
*   **AI Data Preparation**: Collecting knowledge bases for NotebookLM, Claude Projects, or custom GPTs.
*   **Documentation Management**: Archiving official documentation, wikis, or internal knowledge bases.

## File
`github_docs_sync.ipynb`

## Usage

1.  Click the **[Open In Colab]** badge above to open the notebook.
2.  Fill in the **Settings Form**:
    *   `repo_url`: The GitHub URL you want to fetch (supports specific folder paths).
    *   `drive_folder`: The destination folder name in your Google Drive.
3.  Click the Play button (▶) to run the script.
4.  When prompted, click "Connect" to authorize Google Drive access.

## Features

*   **Subdirectory Support**: You can specify a specific folder URL (e.g., `/docs` or `/src`) to fetch only what you need, rather than cloning the entire repository.
*   **Version History**: Saved folders are automatically named with `RepositoryName_Timestamp` to prevent overwriting previous data.
*   **Batch Processing**: Supports processing up to 5 URLs in a single run.
