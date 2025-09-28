# JobApAi (Chrome Extension)

A Chrome extension with a side panel to analyze a candidate CV, a job description, and a job application form (as text), then produce field-by-field suggestions that you can copy into the form.

## Features

- Side panel UI with inputs for CV, Job Description, and Form text
- Uses OpenAI API to suggest values per field with brief reasoning
- Copy each field value or copy all as JSON
- Options page where users paste their own OpenAI API key (stored in Chrome Sync storage)

## Install (Developer Mode)

1. In Chrome, go to `chrome://extensions`.
2. Enable Developer mode (toggle in the top-right).
3. Click "Load unpacked" and select this folder.
4. Click the extension icon and pin it. Clicking the icon opens the side panel.
5. Open the Options page (link at the top of the side panel) and paste your OpenAI API key.

## Usage

1. Open the side panel from the extension icon.
2. Paste your CV text, the job description, and the application form text (labels/questions).
3. Click Analyze. The model will return a JSON of fields and suggested values.
4. Copy individual values or copy all as JSON.

## Privacy and data

- Keys are stored locally via Chrome Sync storage and used only to call OpenAI.
- The analysis uses the `gpt-4o-mini` model by default; you can change it in `background.js`.
- No data is sent anywhere other than OpenAI for analysis.

## Packaging for the Chrome Web Store

- Ensure no secrets are embedded in code or files.
- Keep the Options flow (BYOK) as the only key path.
- Prepare icons and screenshots for the listing.
- Zip this folder contents (excluding `.git`):
  - `zip -r job-form-filler-ext.zip . -x '*.git*'`
