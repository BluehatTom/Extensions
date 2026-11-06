# Chrome Extensions

## Page Navigator

[Download Page Navigator v1.2.0](https://github.com/BluehatTom/Extensions/raw/refs/heads/main/Page-Navigator-v1.2.0.zip)

Navigate long pages with **Top, Middle, and End**, live search as you type, heading navigation, previous-position history, and saved reading spots.

### New in v1.2: page-aware chat sidebar

- **Use this page** or **Use selection** to choose the text for a question.
- Summarize, explain, find sections, or extract details into a table.
- Review the attached text before sending it.
- Use answer source buttons to jump to and highlight relevant passages.
- Keep navigation and live search available beside the conversation.

The ZIP contains the extension, a local OpenAI connector, all source files, tests, and a **START-HERE.html** setup guide.

### Install or update

1. Download and extract the ZIP.
2. Open `chrome://extensions` and enable **Developer mode**.
3. Choose **Load unpacked** and select the `page-navigator` folder containing `manifest.json`.
4. Pin the extension and refresh your webpages.

To update without losing settings or reading spots, replace the files in your currently loaded `page-navigator` folder, click **Reload** on the Extensions page, and refresh your webpages. Chrome 116 or later is required.

### Activate page chat

1. Install **Node.js 22 or later** if needed.
2. Open the included `page-navigator-connector` folder and double-click **START-WINDOWS.cmd** (a Mac/Linux start script is also included).
3. Enter your **OpenAI API key** in the connector's local setup page.
4. Copy its separate **connection code** into the Page chat sidebar and choose **Connect**.

Keep the connector running while chatting. The API key stays in memory and is forgotten when the connector closes; enter it again after restarting, or use an existing `OPENAI_API_KEY` environment configuration. The extension saves only the separate connection code. No API key is included in the download or repository.

Page chat uses the OpenAI API and needs model access and available API credits. The default model is `gpt-5.4-mini`. Attached text is sent only when you submit a question. Chat transcripts and captured pages are not saved persistently by the extension or connector.

### ChatGPT website companion

The separate **Open ChatGPT**, **Copy selected text**, and **Copy & open** controls remain available without an API key. You paste and submit text in the ChatGPT website yourself. Navigation, search, and saved spots also work without the local connector.

Automated checks cover navigation, search, context capture, source jumps, sidebar state, and the local connector's HTTP/API boundary. Real Chrome rendering, native Windows launching, and live OpenAI responses were not verified in the build environment. Exact scope is recorded in `page-navigator/VALIDATION.txt`.

### Previous versions

- [Page Navigator v1.1.0](https://github.com/BluehatTom/Extensions/raw/refs/heads/main/Page-Navigator-v1.1.0.zip)
- [Page Navigator v1.0.0](https://github.com/BluehatTom/Extensions/raw/refs/heads/main/Page-Navigator-v1.0.0.zip)

---

## Miami Course List Lightweight

[Download Miami Course List Lightweight v1.9.0](https://github.com/BluehatTom/Extensions/raw/refs/heads/main/Miami_Course_List_Lightweight_v1_9_0.zip)

**New in v1.9.0:** A visual Monday–Friday schedule with 30-minute calendar lines (8 AM–9 PM), color-coded course blocks, date-aware conflict indicators, and asynchronous/TBA classes listed below the calendar. Use **Expand width** to see all five weekdays in a wider docked panel without covering the page. Existing saved presets and exported schedule behavior are preserved.

Chrome/Edge extension for [Miami University's Course List](https://www.apps.miamioh.edu/courselist/). Adds a docked and collapsible side panel for saved search filters, built-in major/minor and modality selections, course-row checkboxes, and Excel/CSV/PDF exports.

**Schedule Builder:** Assemble a schedule across multiple searches, using the **far-right results column** for meeting days, times, and calendar dates. It flags potentially conflicting sections when the same days and times overlap within overlapping meeting-date ranges (including sprint courses). Missing meeting dates are marked for verification. Schedule exports clear the draft after a successful save; saved presets remain intact.

### Install or update

1. Download and extract the ZIP above.
2. Open `chrome://extensions` (or `edge://extensions`), enable **Developer mode**, and choose **Load unpacked**.
3. Select the extracted `Miami_Course_List_Lightweight` folder containing `manifest.json`.
4. Open or refresh the Course List website.

To update without losing presets, **replace the files in your currently loaded extension folder**, then reload the extension on the Extensions page. You may also export a preset backup first. Detailed instructions and feature documentation are inside the ZIP's `README.md`.

[Previous version v1.8.2](https://github.com/BluehatTom/Extensions/raw/refs/heads/main/Miami_Course_List_Lightweight_v1_8_2.zip)

*Local browser tests passed; the university's live post-search page layout has not yet been verified.*
