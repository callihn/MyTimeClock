# MyTimeClock

> A no-nonsense time clock app for hourly workers. Track hours, calculate pay, and print reports — all offline.

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
