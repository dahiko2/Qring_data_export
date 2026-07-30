QRing Dashboard parses the .noedata Android backup file from the QRing app (Blivas smart ring) directly in the browser — no upload, no backend. It reconstructs the app's SQLite database, then displays daily/monthly/yearly views with step/distance/calorie rings, a sleep-stage hypnogram, SpO2 and temperature charts, and one-click export to a multi-sheet Excel file. Built because the official app has no analytics or data export.

Tested with QRing app version 1.0.1.131 and Blivas ring firmware 2.00.27 — other versions may use a different database schema.

How to get the .noedata file (Samsung):

▎ 1. Install Samsung Smart Switch on a PC and connect your phone via USB.

▎ 2. In Smart Switch, choose Backup (not "Switch phones") and select only the QRing app.

▎ 3. In the backup output folder, find com.app.cq.ring.noedata — that's the file this dashboard reads.


Standard Android adb backup won't work — the app disables it. Smart Switch uses a privileged system backup path that bypasses that restriction.
