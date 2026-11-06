# Chrome Extensions

## Page Navigator

[Download Page Navigator v1.1.0](https://github.com/BluehatTom/Extensions/raw/refs/heads/main/Page-Navigator-v1.1.0.zip)

Navigate long pages with **Top, Middle, and End**, live search as you type, heading navigation, previous-position history, and saved reading spots.

### New in v1.1: ChatGPT companion

- **Open ChatGPT** opens a movable, resizable companion window or brings the existing companion forward.
- **Copy selected text** copies a highlighted passage from the current page.
- **Copy & open** copies the passage, then opens or focuses ChatGPT. Paste your text, add a question, and send when ready.
- Assign an optional ChatGPT shortcut at `chrome://extensions/shortcuts`.

No API key is required. The companion opens the normal ChatGPT website; sign in there if asked. Page Navigator never submits a message automatically.

### Install

1. Download and extract the ZIP.
2. Open `chrome://extensions` and enable **Developer mode**.
3. Choose **Load unpacked** and select the extracted `page-navigator` folder containing `manifest.json`.
4. Pin the extension and refresh your open webpages.

### Update from v1.0

Replace the files in your existing `page-navigator` folder with the new version. Open `chrome://extensions`, click **Reload** on Page Navigator, and refresh your webpages. Keeping the same installation preserves your settings and saved spots.

The ZIP includes all source files, installation instructions, and automated logic tests. Navigation and search run locally. The copy controls request clipboard-write access, and a narrow ChatGPT host permission supports companion-window reuse. No clipboard-read permission is requested.

Automated checks cover navigation, live search, copying, and companion-window behavior. Real Chrome installation and visual rendering were not tested in the build environment; see `VALIDATION.txt` inside the ZIP for the exact test scope.

### Previous version

[Page Navigator v1.0.0](https://github.com/BluehatTom/Extensions/raw/refs/heads/main/Page-Navigator-v1.0.0.zip)

---

## Miami Course List Lightweight

[Download Miami Course List Lightweight v1.8.2](https://github.com/BluehatTom/Extensions/raw/refs/heads/main/Miami_Course_List_Lightweight_v1_8_2.zip)

Chrome/Edge extension for [Miami University's Course List](https://www.apps.miamioh.edu/courselist/). Adds a docked and collapsible side panel for saved search filters, built-in major/minor and modality selections, course-row checkboxes, and Excel/CSV/PDF exports.

**Schedule Builder:** Assemble a schedule across multiple searches, using the **far-right results column** for meeting days, times, and calendar dates. It flags potentially conflicting sections when the same days and times overlap within overlapping meeting-date ranges (including sprint courses). Missing meeting dates are marked for verification. Schedule exports clear the draft after a successful save; saved presets remain intact.

### Install or update

1. Download and extract the ZIP above.
2. Open `chrome://extensions` (or `edge://extensions`), enable **Developer mode**, and choose **Load unpacked**.
3. Select the extracted `Miami_Course_List_Lightweight` folder containing `manifest.json`.
4. Open or refresh the Course List website.

To update without losing presets, **replace the files in your currently loaded extension folder**, then reload the extension on the Extensions page. You may also export a preset backup first. Detailed instructions and feature documentation are inside the ZIP's `README.md`.

*Local browser tests passed; the university's live post-search page layout has not yet been verified.*
