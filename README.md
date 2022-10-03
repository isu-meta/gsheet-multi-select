# gsheet-multi-select
Google Sheets script for selecting multiple values to populate a cell

Adapted from https://stackoverflow.com/questions/23369296/selecting-multiple-values-from-a-dropdown-list-in-google-spreadsheet/53310932#53310932

To use this script:
1. In your Google Sheet, set up data validation for a cell (or cells), using data from a range. In cell validation, do not select 'Reject input'.
2. Go to Extensions > Apps Script
3. In the script editor, go to Files > + > Script
4. Name the file multi-select.gs and paste in the contents of multi-select.gs. Save.
5. In the script editor, go to Files > + > HTML
6. Name the file dialog.html and paste in the contents of dialog.html. Save.
7. Run multi-select.gs
	a. Review permissions
	b. Sign in
	c. Allow
8. Back in your spreadsheet, you should now have a new menu called 'Scripts'. Refresh the page if necessary.
9. Select the cell you want to fill with multiple items from your validation range.
10. Go to Scripts > Multi-select for this cell... and the sidebar should open, showing a checklist of valid items.
11. Tick the items you want and click the 'Set' button to fill your cell with those selected items, comma [semicolon] separated.
You can leave the script sidebar open. When you select any cell that has validation, click 'Refresh validation' in the script sidebar to bring up that cell's checklist.

Notes
• This is a container-bound script (bound by the sheet in which it was created)
• Only users who have permission to edit a container can run its bound script. 
