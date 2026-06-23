# [HireReady Notebook](https://hireready.omarcodes.io)

**HireReady Notebook** is a minimalist NotebookLM-style web app for interview and resume preparation. It lets candidates upload resumes, job descriptions, company notes, recruiter notes, and interview-prep documents, then ask grounded questions using Gemini with visible source references.

The project was built for the **Build with AI UAE** workshop as an industry-specific document assistant for the recruitment, career, and interview-prep space.

## Problem Statement

Job seekers and students often prepare for interviews using scattered documents: resumes, role descriptions, company notes, counselor advice, and project writeups. They need a fast way to understand what matters, identify gaps, prepare strong answers, and create a concise interview briefing.

HireReady Notebook turns those documents into an interactive preparation workspace.

## Core Features

- Upload multiple documents: **PDF, TXT, and MD**
- Select which files are active context for the AI
- Read uploaded PDFs in a central document viewer
- Search uploaded PDF text
- Ask Gemini questions about active documents
- Get grounded answers with document/page or section references
- Generate interview-prep outputs with commands:
  - `/summary` — summarize active sources
  - `/gaps` — compare resume evidence against role criteria
  - `/questions` — generate interview questions
  - `/star` — build STAR-format answer preparation
  - `/brief` — create candidate briefing notes
  - `/deck` — generate a visual candidate briefing deck
- Download generated briefing decks as **PPTX**
- Export chat as Markdown or printable PDF
- Dark mode / light mode
- Resizable three-panel research workspace
- Browser-based notebook persistence using local storage and IndexedDB

## Industry Focus

HireReady Notebook is designed for the **recruitment and interview-preparation industry**.

It helps users answer questions such as:

- What parts of my resume match this job description?
- What experience is missing or weak?
- What technical and behavioral questions should I prepare for?
- Which projects should I talk about in the interview?
- How can I structure answers using STAR?
- What should my candidate briefing deck include?

## App Structure

The interface uses a three-panel layout:

1. **Left sidebar — Document Library**
   - Upload files
   - Select active context
   - Search PDFs
   - Manage notebooks

2. **Center workspace — Paper View / Generated Artifacts**
   - View PDFs
   - Navigate pages
   - Preview generated briefing decks
   - Export outputs

3. **Right sidebar — AI Assistant**
   - Enter Gemini API key
   - Choose Gemini model
   - Ask questions
   - Use commands
   - Export chat

## Gemini Setup

The app is client-side and uses the user's own Gemini API key.

Supported model options in the UI include:

- `gemini-2.5-flash-lite`
- `gemini-2.0-flash-lite`
- `gemini-2.0-flash`
- `gemini-2.5-flash`

The default intended model is:

```text
gemini-2.5-flash-lite
```

To use the app:

1. Open the app in a browser.
2. Paste a Gemini API key into the API key field.
3. Wait for the connection indicator to turn green.
4. Upload documents.
5. Select active context files.
6. Ask questions or use commands like `/gaps`, `/questions`, or `/deck`.

## Disclaimer

_This tool provides interview and resume preparation support. It is **not official hiring, legal, immigration, or career advice**. AI outputs should be reviewed by the user before being used in applications, interviews, or professional communication._

## Suggested Demo Flow

1. Upload a sample resume.
2. Upload a job description.
3. Upload company or recruiter notes.
4. Mark all relevant files as active context.
5. Ask:

```text
/gaps
```

6. Ask:

```text
Generate interview questions from the active documents.
```

7. Ask:

```text
Create a candidate briefing deck.
```

8. Show the generated deck and download it as PPTX.

## Competition Angle

HireReady Notebook goes beyond a generic document chatbot by focusing on interview preparation. It combines document-grounded Q&A, resume gap analysis, interview question generation, STAR answer support, and briefing deck creation in one minimal research workspace.
