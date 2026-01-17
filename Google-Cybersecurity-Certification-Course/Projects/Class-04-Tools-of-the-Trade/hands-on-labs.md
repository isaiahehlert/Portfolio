# 🧪 Hands-On Labs – Class 4: Tools of the Trade – Linux and SQL

This section contains summaries and artifacts from the hands-on labs completed in **Course 4** of the Google Cybersecurity Certificate. These labs develop core skills in **Linux command-line operations** and **SQL-based log analysis**.

---

## 🐧 **Linux Command Line Lab: Authorization and Permissions**

In this lab, I managed file and directory permissions using Linux commands. The scenario involved a sensitive research environment where I was responsible for removing unauthorized access and aligning permission settings with company security policy.

### Key Actions:
- Used `ls -la` to audit permission settings, including hidden files.
- Interpreted 10-character permission strings (e.g., `-rw-rw-r--`) to determine access levels.
- Applied `chmod` to restrict or grant permissions appropriately for user, group, and others.
- Updated a hidden file (`.project_x.txt`) to make it read-only.
- Removed execute access from a sensitive directory (`drafts`) for non-owner users.

📄 **Report**: [`UseLinuxCommandsToManageFilePermissions.txt.rtf`](./UseLinuxCommandsToManageFilePermissions.txt.rtf)  
📝 **Portfolio Entry**: Includes command breakdowns, permission audits, and project summary.

---

## 🧮 **SQL Filtering Lab – Apply Filters with AND, OR, NOT**

In this lab, I conducted advanced SQL filtering operations to analyze login patterns and isolate employee subsets. The scenario involved investigating suspicious access patterns, failed after-hours logins, and department-specific machine update requirements. This reinforced my ability to craft compound SQL queries using logical operators and pattern matching.

### Key Actions:
- Queried failed login attempts using `AND` and time filters (`login_time > '18:00:00' AND success = 0`).
- Filtered logins occurring on multiple dates using `OR`.
- Used `NOT` and `LIKE` together to exclude country codes like `'MEX%'`.
- Combined `AND` and `LIKE` to isolate Marketing department users in East-building offices.
- Queried across departments (`Finance` OR `Sales`) and excluded one (`NOT 'Information Technology'`).

📄 **Report**: [`Apply-Filters-To-SQL-Queries.rtf`](./Apply-Filters-To-SQL-Queries.rtf)  
📄 **Template**: [`Apply filters to SQL queries.docx`](./Apply%20filters%20to%20SQL%20queries.docx)  
📑 **Supporting Docs**: [`Instructions for including SQL queries.docx`](./Instructions%20for%20including%20SQL%20queries.docx), [`Table formats.docx`](./Table%20formats.docx)
