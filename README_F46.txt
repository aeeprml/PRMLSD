APTRANSCO PORUMAMILLA SUB DIVISION MIS – F46
Maintenance module revision based on F45.

WHAT CHANGED
- Preserved F45 homepage, existing sections, logo, PTR image and reference MIS templates.
- Replaced the old Maintenance Schedule page with two tabs:
  1) Preventive Maintenance Master
  2) Actual Maintenance Register
- Imported all 92 Statement 11 schedule rows from the October 2026 workbooks:
  MKP: 40 rows
  PML: 28 rows
  KSP: 24 rows
- These 92 rows represent 43 station-specific equipment names and their periodicity entries.
- Omitted Make & Rating from the new maintenance UI, as requested.
- Carried forward overdue occurrences without duplicate creation.
- For the 13 imported rows with an actual completion date, generated the next due occurrence from the actual date and periodicity.
- Added automatic next-due calculation for monthly, quarterly, half-yearly and yearly periods (half-yearly is available as an option; it was not imported where absent).
- Added editable equipment master activities and periodicities, small equipment SVG illustrations, initial schedule date setup, and Excel/PDF print exports.
- Fixed F45 maintenance script's element lookup helper so DOM elements are retrieved correctly.

SOURCE DATA
- 2026/Oct 26/MIS 10-2026 220 KV PMML.xlsx – Stat-11
- 2026/Oct 26/MIS 10-2026 132 KV PML.xlsx – Stat-11
- 2026/Oct 26/MIS 10-2026 132 KV KSPD.xlsx – Stat-11

IMPORTANT
- October Statement 11 values are imported as provided. The source Make & Rating column is not displayed.
- The generic checklist activity text is an editable proposed template, not a certified APTRANSCO maintenance instruction. Verify against current APTRANSCO circulars and OEM manuals before formal adoption.
- Data persistence in this F45-derived static website uses browser localStorage. Entries made on one device/browser are not automatically shared with other users/devices. Shared multi-user storage requires the connected online database/API.
- PDF export opens the browser print dialog; select “Save as PDF”.
- Excel export is an Excel-compatible .xls workbook generated from the current register view.

IMPORT CHECK
- Statement 11 source rows imported: 92.
- Station-wise equipment counts: MKP 19, PML 13, KSP 11 (43 station-equipment combinations total).
- Imported rows with actual completion dates: 13; next occurrences calculated from those actual dates.
- Source workbooks are included under source_data for audit/reference.
