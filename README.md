# Dienstplan-System Pro 📅

A smart, rule-based employee scheduling application designed for managing part-time staff at the SPORTFABRIK front desk. This tool automates the creation of fair and compliant schedules by taking into account complex German labor laws for Minijobbers, Werkstudenten, and Permanent employees.



---
## ## Key Features ✨

This application goes beyond basic scheduling and includes a sophisticated rule engine to ensure schedules are both optimal and legally compliant.

* **Automated Schedule Generation:** Creates a full month's schedule with a single click, based on employee availability and a robust scoring system.
* **Role-Based Scheduling Rules:** Applies different rules and hour targets based on employee type:
    * **Minijob:** Weekly hour steering and monthly earnings cap monitoring.
    * **Werkstudent (Student):** Manages the 20-hour weekly limit with legally compliant exceptions for night/weekend work.
    * **Permanent:** Adheres to strict contract hours.
* **Dynamic Monthly Hour Targets:** Automatically adjusts monthly target hours to account for:
    * **Hour Carryover (`Übertrag`):** Surpluses or deficits from the previous month are carried over.
    * **Vacation & Sick Leave:** Approved absences proportionally reduce the required work hours for the month, in line with German law.
* **Vacation & Absence Management (`Urlaubsverwaltung`):** A dedicated ledger to track annual vacation allowances, manually entered days taken, and planned absences for all staff.
* **Live Validation & Manual Overrides:** The schedule provides real-time warnings (⚠️) and blockers (❌) for rule violations. Managers can manually assign or swap shifts, with all changes being instantly re-validated.
* **Data Export:** Export schedules to **CSV** for spreadsheets or printable **PDF** formats.
* **Clean Architecture:** The front-end is refactored to use **HTML `<template>` tags**, separating the application's structure (HTML) from its logic (JavaScript) for easier maintenance.

---
## ## Technology Stack 🛠️

This is a pure front-end application with no server-side dependency.

* **HTML5**
* **CSS3** (with CSS Variables for theming)
* **Vanilla JavaScript (ES6+)**
* **Libraries:** jsPDF & jspdf-autotable for PDF generation.

---
## ## Local Setup & Installation 🚀

Getting the application running is simple:

1.  Clone the repository to your local machine.
2.  Open the `staff_scheduler.html` file in any modern web browser (like Chrome, Firefox, or Edge).

That's it! All data is stored locally in your browser's **`localStorage`**.

---
## ## Future Development (Roadmap)

While the current version is a powerful local tool, the next logical step is to migrate it to a professional, multi-user cloud application.

* [ ] **Migrate to a Cloud Back-End:** Move the data persistence and core logic to a Backend-as-a-Service platform like **Supabase** or **Firebase**.
* [ ] **Implement User Authentication:** Allow different managers to securely log in and access the schedule.
* [ ] **Develop Employee-Facing Features:**
    * Allow employees to propose shift swaps with each other.
    * Create an "open shift board" for employees to claim available shifts.
* [ ] **Introduce Schedule Templates:** Enable managers to save and load common weekly schedule patterns.

---
## ## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
