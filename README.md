# jde-mapping-sheet

Turn any JSON payload into a JD Edwards field mapping sheet, in your browser, with no installation.

Mapping a third-party JSON payload to JDE usually means retyping every field into Excel. JDE Mapping Sheet reads the payload for you and gives you one row per field. You add the JDE table, alias, description and logic, then copy the finished sheet into Excel.

[Download JDE-Mapping-Sheet.html] (single file, free to use)

Designed and ideated by Pranoy.K. Developed by Claude.

Features

Build a mapping sheet from a JSON payload

Paste or upload a JSON payload and every field becomes a row.
Each row shows the full path, the data type and a sample value.
Add the JDE table, JDE alias, description and logic or remarks on the same row.
Nested objects and arrays are handled. Fields that appear in only some array items still get a row.
A progress bar shows how many fields are mapped.

Map to your existing Excel data

Upload an Excel (.xlsx, .xls) or CSV file. It appears as a table with all your own columns, plus a JSON path column.
Drag a field from the payload list onto any row, and the complete path is filled in. On a touch screen, tap the field, then tap the row.
Each payload field shows how many rows use it.
Workbooks with several sheets get a sheet picker.

Paths you can use in scripts

Paths read like /invoicePeriod/startDate or /billingReference/invoiceDocumentReference/issueDate.
Arrays appear as /lines[*]/itemNumber. You can switch to [0], [], /0 or /* styles.
This makes it easy to write Groovy or other transformation scripts from your mapping.

Work with large sheets

Sort any column and filter each column separately, or search across all columns.
Resize columns by dragging their edges, and drag the ⋮⋮ grip to reorder them.
Long text wraps inside cells.
An automatic # column lets you restore the original order by sorting on it.
“Reset view” restores column order, widths, sort and filters.

Export to Excel

“Copy for Excel” copies the whole sheet. Paste it straight into Excel.
“Copy CSV” is also available for the mapping sheet.

Clear anything, any time

Each section has its own clear button, and “Reset all” at the top right wipes everything. Clear buttons ask for a second click so nothing is lost by accident.

Your data stays with you

Everything runs in your browser. Your payload and mappings are not uploaded to any server.
Your work is saved in the browser you use, so you can close the page and come back.
How to use it

Option A: Build a mapping sheet from scratch

Open the file in Chrome, Edge or Firefox.
In the Payload box, paste your JSON or click Upload .json. Click Format to tidy it.
Stay on the Build mapping sheet tab. Every field is now a row.
For each row, fill in JDE table, JDE alias, Description and Logic / remarks.
Use the filters under the headings to find rows, for example Unmapped in the Mapped column.
Click Copy for Excel and paste into a spreadsheet.

Option B: Map to a field list you already have

Load your JSON payload as above.
Open the Map to existing Excel data tab.
Click Upload Excel or CSV. Put column headings in the first row. You can also paste rows copied from Excel.
Drag each payload field from the left list onto the matching row.
Add remarks if needed, then click Copy for Excel. You get your original columns plus the JSON path, type, sample value and remarks.

Tips

On the first tab, type a JDE alias that exists in your uploaded Excel data and the table and description fill in automatically. This needs headings that contain “table”, “alias” and “description”.
Pasting the exported sheet back into the second tab later restores your mappings.
Click the # heading to get back to the original row order after sorting.
Requirements and good to know
Works in current versions of Chrome, Edge and Firefox on desktop.
Internet connection needed when you open it, because it loads its fonts and Excel reader online. Without a connection, CSV upload and pasted rows still work, but .xlsx upload does not.
Moving columns needs a mouse. On touch screens, sorting, filtering and tap-to-map still work.
The page can’t save an Excel file for you, so use “Copy for Excel” and paste.
