# 🧠 Salesforce Hands-On Learnings & Practical Log

This log is used to document and track all hands-on exercises, configurations, coding tasks, and custom creations you build in your Salesforce Developer Orgs or Trailhead Playgrounds.

---

## 🛠️ Essential Admin & Developer Skills Checklist

Check off these skills as you successfully configure or code them!

### 🔹 1. Data Model & UI Config
- [ ] Create a Custom Object with appropriate plural naming and search capabilities.
- [ ] Configure custom field types (Text, Number, Date, Currency, Picklist, Multi-Select Picklist).
- [ ] Establish Object Relationships:
  - [ ] **Lookup Relationship** (soft connection, parent field optional).
  - [ ] **Master-Detail Relationship** (hard connection, cascade delete, rollup summaries).
- [ ] Customize **Page Layouts** and organize fields into logical sections.
- [ ] Configure **Record Types** and distinct **Picklists** tailored to different user processes.
- [ ] Create a **Roll-Up Summary Field** to calculate values from child records to parent records.

### 🔹 2. Data Validation & Automation
- [ ] Write a **Validation Rule** using logical formulas (e.g., `AND()`, `OR()`, `ISCHANGED()`, `ISPICKVAL()`).
- [ ] Build a **Formula Field** to automate calculated values.
- [ ] Automate a business process with **Lightning Flow Builder**:
  - [ ] **Record-Triggered Flow** (to automatically update a field or create a task).
  - [ ] **Screen Flow** (to guide users through a multi-step data entry screen).
  - [ ] **Scheduled Triggered Flow** (to run bulk processing daily/weekly).

### 🔹 3. Security, Sharing & Governance
- [ ] Create a new **User** and configure their profile.
- [ ] Customize **Organization-Wide Defaults (OWD)** to restrict baseline access.
- [ ] Create a **Role Hierarchy** to grant management-level read/write access.
- [ ] Create **Sharing Rules** to open up record access to specific groups/roles.
- [ ] Create a **Permission Set** to grant specialized access (e.g., "Export Reports") without editing the Profile.

### 🔹 4. Developer & Code (Apex & UI)
- [ ] Execute programmatic queries using **SOQL** and **SOSL** in the Query Editor.
- [ ] Write an **Apex Trigger** to automate logic before or after database changes (handling bulk scenarios).
- [ ] Build an **Apex Helper Class** with modular, reusable logic.
- [ ] Write an **Apex Test Class** achieving at least 75% code coverage (with mock data creation).
- [ ] Develop a **Lightning Web Component (LWC)** with HTML, JS, and CSS configurations.

---

## 📝 Hands-On Learning Log

Use this section to log each practical configuration or code segment you build!

### Example Entry:
> #### 📅 May 8, 2026: Created Custom Object "Property" for Real Estate App
> * **Business Problem:** A real estate client needs to track properties for sale, including price, address, and status.
> * **Configuration / Implementation Steps:**
>   1. Created custom object `Property__c` (Plural: Properties).
>   2. Created fields: `Price__c` (Currency), `Beds__c` (Number), `Baths__c` (Number), and `Status__c` (Picklist: Available, Pending, Sold).
>   3. Set up a validation rule `Price_Must_Be_Positive` to ensure `Price__c > 0`.
> * **Lessons Learned:** Learned that custom objects are automatically appended with `__c` (custom) in their API name, and that picking the right primary field type (Text vs. Auto-Number) is crucial.
> * **Evidence:**  
>   ![Property Schema](screenshots/property-schema-builder.png) *(Placeholder Link)*

---

*Add your learning log entries below:*

### 📅 [Insert Date]: [Insert Title of Practical Task]
* **Business Problem:** 
* **Configuration / Implementation Steps:**
  1. 
  2. 
  3. 
* **Lessons Learned:** 
* **Evidence:**  
  ![Alt Text](screenshots/your-screenshot.png)
