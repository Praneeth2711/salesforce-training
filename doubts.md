# ❓ Salesforce Doubts & Resolution Tracker

Keep track of errors, conceptual gaps, and development blockers here. Documenting your blockers and how you solved them is one of the most effective ways to build deep technical expertise in Salesforce!

---

## 🚦 Doubt Status Tracker

| ID | Doubt / Blocker / Error | Category | Date Logged | Status | Resolution & Key Takeaways |
| :--- | :--- | :---: | :---: | :---: | :--- |
| **01** | What is the fundamental difference between **Lookup** and **Master-Detail** relationships? | Data Modeling | `May 8, 2026` | 🟢 Resolved | **Master-Detail:** High dependency. If parent is deleted, child is deleted. Child inherits security settings of parent. Roll-up summaries are possible on parent. <br>**Lookup:** Loose coupling. Child can exist without parent. Parent deletion does not automatically delete child (unless specified). Security can be independent. |
| **02** | Why do we see the error `System.LimitException: Too many SOQL queries: 101` in Apex? | Apex Governor Limits | `May 8, 2026` | 🟢 Resolved | Triggered when a SOQL query is placed inside a `for` loop, exceeding the limit of 100 synchronous queries. **Resolution:** Always bulkify your Apex! Execute queries outside loops, store results in Maps/Lists, and iterate over collections instead. |
| **03** | When should I use a **Validation Rule** versus a **Flow** to enforce data correctness? | Automation | `May 8, 2026` | 🟢 Resolved | **Validation Rules** *only check if data is correct* before saving, preventing bad data from entering Salesforce. **Flows** actually *change or automate data fields/actions*. Always use Validation Rules first if your only goal is to prevent invalid entries. |
| **04** | [Sample Doubt: Replace or add your own here!] | Security | `May 8, 2026` | 🔴 Pending | [Add steps you are taking to research, documentation links, or ideas.] |

---

## 📐 Template for New Doubts

Copy-paste this row to the bottom of the table above to track a new doubt:

```markdown
| **XX** | [Briefly describe the doubt or paste the error code] | [Category] | [Date] | 🔴 Pending | [Add notes, research, or resolution when found] |
```

---

## 📚 Top Resources to Resolve Salesforce Doubts

If you hit a roadblock, try these steps in order:
1. **Salesforce Stack Exchange:** The go-to forum for Salesforce developers and architects. Search with specific error codes.
2. **Trailblazer Community Groups:** Great for admin, flow, and business-focused questions.
3. **Developer Console Logging:** When debugging Apex, turn on the log inspector, set the filter to `USER_DEBUG` level, and read the values.
4. **Official Salesforce Developer Docs:** For precise API, Apex method, or syntax structures.
