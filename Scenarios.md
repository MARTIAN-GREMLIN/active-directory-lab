# Permission Scenarios

## Scenario 1: Developer Can't Access Database

**What Happens:**
1. John (developer) tries to access database
2. System checks: "Is john.smith in Database-Admins group?"
3. System finds: NO
4. Result: **ACCESS DENIED** ✗

**Why:**
Developers don't need database access. It's restricted to protect data.

**What John Should Do:**
Ask Sarah (admin) to get the data for him.

---

## Scenario 2: Admin Can Access Database

**What Happens:**
1. Sarah (admin) tries to access database
2. System checks: "Is sadmin in Database-Admins group?"
3. System finds: YES ✓
4. Result: **ACCESS ALLOWED** ✓

**Why:**
Admins need database access for backups, maintenance, and management.

---

## Scenario 3: Everyone Can Access Company Files

**What Happens:**
1. John, Jane, or Sarah try to access company files
2. System checks: "Are they in File-Server-Access?"
3. System finds: YES for all three
4. Result: **ACCESS ALLOWED** ✓

**Why:**
Everyone needs company files, so everyone gets access.

---

## Interview Talking Point

"I demonstrated how permissions work in Azure AD. 

Database access is restricted to admins only - 
if a developer tries to access it, they can't because 
they're not in the Database-Admins group.

But everyone can access company files because everyone needs them.

This shows the principle of least privilege: 
give each person ONLY what they need."
