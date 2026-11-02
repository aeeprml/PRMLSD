PRMLSD WEBSITE – F48

This revision repairs two obsolete scripts that were breaking the live website:
1. Removed an old RMI preview script that attempted to update elements that do not exist. The current RMI module remains in place.
2. Removed an obsolete duplicate MIS editor that referenced missing misHead/misBody elements and overwrote the current MIS form controls.
3. Added safe handling when an MIS station/statement template is unavailable.

Maintenance remains divided into three sections:
1. Preventive Maintenance Master
2. Maintenance Schedule
3. Actual Maintenance Register

No Excel workbook is required in the GitHub repository for normal operation. The MIS templates and October 2026 maintenance source records are embedded in index.html. CSV import/export and Excel/PDF report export are optional user actions.

Repository contents:
- index.html
- logo(2).jpg
- ptr-3.jpeg
- equipment_images/*.svg

IMPORTANT:
- This version still uses browser localStorage for several modules. Data entered on one device/browser is not automatically shared with other Sub Engineers. A shared online database (Cloudflare D1 + Worker API) is a separate required deployment step for multi-user synchronized data.
- JavaScript syntax and ZIP integrity were checked. A full live browser test was not completed.
