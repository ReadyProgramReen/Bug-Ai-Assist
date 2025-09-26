# Bug-Ai-Assist

This project is an **AI-powered bug triager extension** built as a team effort.
The goal is to let developers paste in a stack trace and instantly get an AI-generated explanation of the error, the likely reason, and suggested solutions, all **without leaving VS Code**.


<img width="1845" height="970" alt="Screenshot -bug-triager 2" src="https://github.com/user-attachments/assets/0fabff4d-85b7-4507-b06a-71c119aaac24" />

## My Role
I was responsible for the **entire frontend (UI)**, including:
- Designing and building the Webview-based dashboard (HTML, CSS, JavaScript)
- Creating the **Analyze panel** where users paste their stack traces
- Structuring the AI response display into **Problem / Reason / Solution**
- Implementing the **History panel** to log past analyses
- Adding a **Settings panel** (theme, language, toggles for monitoring & notifications)
- Styling and theming (dark/light mode support, responsive layout)

## Teammate's Role
- Built the **backend integration** with the OpenAI API
- Wired up stack trace analysis and AI response handling
- Connected the backend to update the **History log** dynamically
- Helped adjust structure for IDs, layout, and responsive flow

## Tech Stack
- **Frontend (UI):** HTML, CSS, JavaScript (VS Code Webview)
- **Backend:** Node.js, OpenAI API
- **AI:** OpenAI GPT models

## How It Works
1. User pastes a stack trace into the **Analyze panel**.  
2. The extension sends the trace to the backend.  
3. The backend calls the **OpenAI API** and returns a structured response.  
4. The UI displays the response as **Problem / Reason / Solution**.  
5. The result is also logged in the **History panel** for future reference.  

## Current Status
- The project is at the **MVP stage**: working end-to-end with AI-powered analysis and history logging.
- History data is stored locally for now, but can be extended with a database in future iterations.  
