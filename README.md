# n8n LinkedIn Auto-Poster Workflow

An automated n8n workflow that watches a Google Sheet for new article links and automatically posts them to LinkedIn.

## Overview

This workflow automates personal or business content distribution by monitoring a specific Google Sheet. Whenever a new row containing an article URL or post text is added, n8n grabs the content and publishes it directly to your LinkedIn profile/page.

## Prerequisites

Before importing this workflow, ensure you have:
* An active **n8n** instance (Localhost, Docker, or Self-hosted).
* A **Google Cloud Platform** project with Google Sheets API enabled and OAuth credentials.
* A **LinkedIn Developer App** set up with `w_member_social` permissions for OAuth authentication.
* A target **Google Sheet** with headers for your posts (e.g., `Title`, `URL`, `Status`).

## How to Import & Setup

1. **Download the Workflow:**
   * Download the `workflow.json` file from this repository.

2. **Import into n8n:**
   * Open your n8n canvas.
   * Click on the top-right menu (`...`) and select **Import from File**.
   * Upload the `workflow.json` file.

3. **Configure Credentials:**
   * **Google Sheets Trigger:** Re-authenticate with your Google OAuth account and select your designated Spreadsheet and Sheet name.
   * **LinkedIn Node:** Connect your LinkedIn OAuth account credentials.

4. **Activate:**
   * Toggle the workflow to **Active** to start listening for updates!

## License

This project is open-source and available under the [MIT License](LICENSE).
