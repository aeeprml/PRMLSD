F50 – PRMLSD website correction

- Equipment illustrations are embedded in index.html as SVG data images; no separate equipment_images folder is required.
- India live clock is initialized and refreshed every second using Asia/Kolkata time.
- Maintenance cards use four columns on wide screens, three on medium desktop, two on tablet and one on mobile.
- Existing station and maintenance records are retained from F49.

Upload index.html and logo(2).jpg to the GitHub repository root. No Excel workbooks are required for normal website operation.

Validation: inline JavaScript syntax checks passed and ZIP integrity checked. Live browser interaction testing was not performed. Browser localStorage remains device-specific; shared database integration is not included.
