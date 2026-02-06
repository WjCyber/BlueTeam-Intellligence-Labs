# Lab — Manage Authorization (Linux)

## 🎯 Operational Objective
Manage authorization in a Linux environment by analyzing and correcting file and directory permissions, applying the principle of least privilege to reduce unauthorized access risk.

## 🧠 Defensive Context
This lab focuses on Linux access control, a core Blue Team responsibility for protecting system integrity and sensitive data.

Misconfigured permissions may lead to:
- Unauthorized file modification
- Privilege escalation
- System compromise

## 🛠️ Actions Performed
- Reviewed file permissions using Linux commands
- Removed write access for unauthorized users
- Corrected permissions on hidden files
- Modified directory permissions to restrict access to the legitimate user
- Validated access after changes

## 🔐 Technical Tasks
### File permission changes
- Identified files with excessive permissions
- Restricted write access for other users

### Hidden file
- Analyzed `.project_x.txt`
- Configured read-only access for user and group
- Removed all write permissions

### Directory permissions
- Evaluated permissions on the `drafts` directory
- Restricted access so only the `researcher2` user has execute and access rights

## 🔎 Applied Concepts
- Authorization vs Authentication
- Linux permission model (read, write, execute)
- User and group-based access control
- Principle of Least Privilege
- Preventive security hardening

## 🧪 Outcome
- Eliminated unauthorized access
- Reduced attack surface
- Maintained system functionality
- Improved data integrity and confidentiality

## 📌 Notes
This lab was completed without the use of AI tools, reinforcing independent technical reasoning and hands-on understanding of Linux authorization.

## 🔗 Reference
Google Cybersecurity Certificate — Manage Authorization (Linux)
