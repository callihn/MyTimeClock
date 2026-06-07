# MyTimeClock

> A no-nonsense time clock app for hourly workers. Track hours, calculate pay, and print reports — all offline.

---

## 🚀 Downloads

[![Get Latest Release](https://img.shields.io/badge/Get%20Latest%20Release-blue?style=for-the-badge&logo=github&logoColor=white)](https://github.com/callihn/MyTimeClock/releases)

---

## 🔒 Privacy & Data Safety

* **Zero Network Permissions:** `MyTimeClock` operates entirely offline. Your tracking data, hourly rates, and earnings reports never leave your device.
* **No Telemetry / Analytics:** No background tracking scripts, no cloud syncing, and no user tracking accounts required.
* **Storage Integrity:** Uses Android's Storage Access Framework (SAF) so backup databases are stored exactly where you choose on local storage or removable SD cards.

---

## Features

- **Clock In / Out** — One tap to clock in, one tap to clock out. Buttons swap colors (green = available action, red = inactive).
- **Live Session Timer** — Elapsed time displayed while clocked in (`HH:MM:SS`). Toggle to show running earnings instead.
- **Today Summary** — Completed hours and earnings for today pinned at the top.
- **Overtime Pay** — Configurable weekly (US federal) or daily (California-style) overtime with custom threshold and multiplier.
- **Holiday Worked Pay** — One-tap add 11 US holidays with automatic date computation. Floating holidays (MLK Day, Memorial Day, etc.) dynamically resolve to the correct date for any year. Customizable multiplier for hours actually worked on holidays.
- **Holiday Pay (PTO)** — Separate holiday pay for paid time off on holidays. Added per-day in the Database Editor at your regular rate. Does not count toward overtime thresholds.
- **Pay Period** — Set which day and time your work week ends.
- **Weekly & Monthly Summaries** — Day-by-day and week-by-week breakdowns of hours and gross pay. Tap a card for full-screen view.
- **Print Reports** — Select any combination of past weekly/monthly summaries and print to PDF. Cards render exactly as they appear on screen.
- **Database Editor** — Google Calendar-style month grid with full-screen day detail view. Navigate any month/year, tap days to see entries, check off multiple entries for batch delete, long-press days for bulk selection/deletion, and add manual hours.
- **Manual Hours Entry** — Add hours for any day in decimal or `HH:mm` format. Choose type: Regular hours, Sick pay, Vacation pay, or Holiday pay. Types display in the entry list so past entries are self-documenting. Sick, vacation, and holiday pay do not count toward overtime.
- **Custom Date Range Summary** — Enter any start/end date to see total hours and gross pay in a styled card with full-screen detail view and print to PDF.
- **Clock-In Editing** — Adjust the start time of an active session.
- **Short Session Warning** — Confirms before clocking out under 15 minutes.
- **Home Screen Widget** — Clock in/out, view session timer, and see today's total hours and earnings.
- **Auto Backup** — Schedule automatic database backups (Daily/Weekly/Monthly). Backups run in the background — restore any backup directly from Settings. First backup runs immediately when enabled.
- **Export / Import Database** — Export your database via Android's Storage Access Framework (SAF) file picker for safekeeping, or import a previously exported file.
- **Database Defragmentation** — Run SQLite `VACUUM` to reclaim space and optimize database performance.
- **Customizable Theme** — 6 preset color schemes (Green, Blue, Purple, Teal, Orange, Pink) or create your own with the built-in HSV color picker for primary, secondary, and text colors. Light/dark mode toggle from the menu persists across launches.

---

## Technical Details

- **Architecture:** 100% Offline-first local architecture.
- **Storage:** Local SQLite database with automated background maintenance (`VACUUM`).
- **File Management:** Native Android Storage Access Framework (SAF) for secure database exports and backups.

---

## Screenshots

<details>
  <summary>📸 Click to view app screenshots</summary>
  <br>
  <table>
    <tr>
      <td><img src="https://github.com/user-attachments/assets/28fadd5e-3100-40b3-99c9-def812d92cec" width="250" alt="Screenshot_20260606-224843_MyTimeClock"></td>
      <td><img src="https://github.com/user-attachments/assets/f1ac1c76-7672-40a5-9d79-070f68a638c9" width="250" alt="Screenshot_20260606-224852_MyTimeClock"></td>
      <td><img src="https://github.com/user-attachments/assets/7908baf2-481e-43e0-a441-13308340e4a5" width="250" alt="Screenshot_20260606-224904_MyTimeClock"></td>
    </tr>
    <tr>
      <td><img src="https://github.com/user-attachments/assets/b6d9c897-a535-4536-8b25-ca1a4dc78634" width="250" alt="Screenshot_20260606-224915_MyTimeClock"></td>
      <td><img src="https://github.com/user-attachments/assets/07c8d8dd-85d3-445b-92a2-754cbb5779e7" width="250" alt="Screenshot_20260606-224936_MyTimeClock"></td>
      <td><img src="https://github.com/user-attachments/assets/5b82af3a-e104-478e-97b5-129396727b6f" width="250" alt="Screenshot_20260606-224946_MyTimeClock"></td>
    </tr>
    <tr>
      <td><img src="https://github.com/user-attachments/assets/01224dc4-63ea-4061-962b-103836d07f3f" width="250" alt="Screenshot_20260606-224954_MyTimeClock"></td>
      <td><img src="https://github.com/user-attachments/assets/a87ce64e-aea1-4f66-b2c5-1fba09736646" width="250" alt="Screenshot_20260606-225023_MyTimeClock"></td>
      <td><img src="https://github.com/user-attachments/assets/878e6bc4-25d5-48fc-9881-0ac16d5d369a" width="250" alt="Screenshot_20260606-225217_MyTimeClock"></td>
    </tr>
    <tr>
      <td><img src="https://github.com/user-attachments/assets/fab66c4b-2388-47bd-bba1-c436e711c719" width="250" alt="Screenshot_20260606-225233_MyTimeClock"></td>
      <td><img src="https://github.com/user-attachments/assets/92c80242-e1e7-4688-b1ae-788ff9109d8b" width="250" alt="Screenshot_20260606-225239_MyTimeClock"></td>
      <td><img src="https://github.com/user-attachments/assets/95b79c8d-59dd-457f-81c3-0f692158a4a8" width="250" alt="Screenshot_20260606-225248_MyTimeClock"></td>
    </tr>
    <tr>
      <td><img src="https://github.com/user-attachments/assets/d88578a9-f14d-4a97-b65a-cf617b7656ad" width="250" alt="Screenshot_20260606-225320_MyTimeClock"></td>
      <td><img src="https://github.com/user-attachments/assets/b0bbd249-6ce6-439a-92f6-88750bbb3dc7" width="250" alt="Screenshot_20260606-225328_MyTimeClock"></td>
      <td><img src="https://github.com/user-attachments/assets/f40f4cfb-e8c8-45bf-84da-d23ee58e7f20" width="250" alt="Screenshot_20260606-225341_MyTimeClock"></td>
    </tr>
    <tr>
      <td><img src="https://github.com/user-attachments/assets/4e0c67f8-62b1-4cc2-a1ac-f77fa82b8dc8" width="250" alt="Screenshot_20260606-225432_MyTimeClock"></td>
      <td><img src="https://github.com/user-attachments/assets/052299a5-db42-43bd-a244-dfc4aa21b8c8" width="250" alt="Screenshot_20260606-225443_MyTimeClock"></td>
      <td><img src="https://github.com/user-attachments/assets/fec9a4d9-9cfe-478a-bd53-0218ba901504" width="250" alt="Screenshot_20260606-225450_MyTimeClock"></td>
    </tr>
    <tr>
      <td><img src="https://github.com/user-attachments/assets/f0bea347-2919-4a3f-bd51-db21edd35456" width="250" alt="Screenshot_20260606-225502_MyTimeClock"></td>
      <td><img src="https://github.com/user-attachments/assets/019d1361-e0e3-4475-9f81-22a8a2534af0" width="250" alt="Screenshot_20260606-225511_MyTimeClock"></td>
      <td><img src="https://github.com/user-attachments/assets/b60e3099-2e59-4748-8256-87d7fb8efd96" width="250" alt="Screenshot_20260606-225519_MyTimeClock"></td>
    </tr>
    <tr>
      <td><img src="https://github.com/user-attachments/assets/7a816c76-a3b1-4161-b063-10cc64f1cb21" width="250" alt="Screenshot_20260606-225540_Nova Launcher"></td>
      <td><img src="https://github.com/user-attachments/assets/8089565a-c16e-4040-8dab-db73721c3c43" width="250" alt="Screenshot_20260606-225549_Nova Launcher"></td>
      <td><img src="https://github.com/user-attachments/assets/59d229c4-c515-4945-a081-eb5a490ff972" width="250" alt="Screenshot_20260606-225605_MyTimeClock"></td>
    </tr>
    <tr>
      <td><img src="https://github.com/user-attachments/assets/7b3ff83f-95ed-4ebc-9fd0-43f913dd837b" width="250" alt="Screenshot_20260606-225619_MyTimeClock"></td>
      <td><img src="https://github.com/user-attachments/assets/7c887ef1-499e-43f3-8c18-3c97904fc6dc" width="250" alt="Screenshot_20260606-225623_Nova Launcher"></td>
      <td><img src="https://github.com/user-attachments/assets/0581b765-7d4d-4bc2-b048-13059287e53f" width="250" alt="Screenshot_20260606-225933_MyTimeClock"></td>
    </tr>
  </table>
</details>
