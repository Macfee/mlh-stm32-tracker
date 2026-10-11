# STM32 学习追踪器

A standalone Chinese-language learning task tracker for Global Hack Week.

## Features

- Add STM32 learning tasks (up to 160 characters).
- Mark tasks complete or incomplete and filter by status.
- Show completed and total task counts.
- Save tasks in this browser using localStorage; an empty saved list stays empty.
- Confirm before deleting an individual task.
- Export the task list as JSON.
- No external packages or network requests.

## Run

Download `index.html` and open it in a browser, or run `python -m http.server 8000` in this folder and visit `http://localhost:8000`.

The four initial tasks are unchecked examples, not claims of completed study. Data is tied to this browser and origin; export a backup before clearing browser storage or switching devices. If browser storage is unavailable, changes stay only in the current session.

## Verification

Browser checks confirmed adding a test task, toggling completion, retaining its state after reload, and filtering completed tasks. The export control displays its completion message; the browser automation did not capture a downloaded file, so downloading should be checked manually.
