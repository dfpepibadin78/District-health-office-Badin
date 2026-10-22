EPI Badin Public Complaint Portal — Prototype
Included
`index.html`: responsive multilingual (English, Urdu, Sindhi) interactive prototype.
Complaint categories, Taluka/UC/locality fields, optional identity, anonymous submission.
Local demo reference numbers and tracking.
Demo admin dashboard, status changes and CSV export.
Important limitations
This is a browser-only prototype. It uses `localStorage`; submissions exist only in the same browser profile and are not sent to any server. There is no secure admin login, central database, evidence upload, SMS/email notification, or production-grade reference generation. The dashboard is not protected and must never be used for real complaints or personal/sensitive data.
Preview locally
Extract the ZIP.
Open `index.html` in a modern browser.
Submit a clearly fictional test complaint and try tracking the generated reference.
Switch languages using the selector.
Before public launch
A production implementation needs:
A backend API and central database (for example PostgreSQL/Supabase).
Server-side reference number generation with a database uniqueness constraint.
Secure administrator authentication, role-based access and audit logs.
Database row-level security; public users must not be able to list/read all complaints.
A secure tracking design (random secret or OTP in addition to reference ID).
Input validation, rate limiting, spam protection, restricted attachment storage and malware checks.
HTTPS, environment secrets, backups, retention/deletion rules and a privacy notice approved by the responsible authority.
User acceptance testing in English, Urdu and Sindhi, and approval from the District EPI office before the portal is represented as official.
Do not put real citizen data into this prototype. It is not connected to the District EPI Badin office and is not live.
