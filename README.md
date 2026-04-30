# active-directory-lab
Simple Azure AD practice lab demonstrating user management and security groups
# Active Directory Lab

Simple hands-on Azure AD practice project for learning cloud identity management.

## 📚 What I Did

Created a basic Azure AD environment with:
- **3 Users** (different departments and roles)
- **5 Security Groups** (for access control)
- **Permission Scenarios** (showing how access works)

## 👥 Users Created

| Name | Email | Department | Role |
|------|-------|------------|------|
| John Smith | john.smith@bd5830gmail.onmicrosoft.com | Engineering | Senior Developer |
| Jane Doe | jane.doe@bd5830gmail.onmicrosoft.com | Engineering | Developer |
| Sarah Admin | sadmin@bd5830gmail.onmicrosoft.com | Operations | System Admin |

## 🔐 Security Groups Created

**Department Groups:**
- Engineering-Team (john.smith, jane.doe)
- Operations-Team (sadmin)

**Resource Groups:**
- File-Server-Access (everyone)
- VPN-Access (everyone)
- Database-Admins (sadmin only)

## 🎯 Key Learning: Least Privilege

Each person gets ONLY what they need:

**Developers (John & Jane) Can:**
- ✅ Access company files
- ✅ Work remotely (VPN)
- ❌ Access database

**Admin (Sarah) Can:**
- ✅ Access everything
- ✅ Manage database
- ✅ Access company files
- ✅ Work remotely

## 📋 Real-World Scenarios

### Scenario 1: Developer Tries Database Access
- Developer is NOT in Database-Admins group
- Result: **Access Denied** ✗
- Why: Developers don't need database access

### Scenario 2: Admin Accesses Database
- Admin IS in Database-Admins group
- Result: **Access Allowed** ✓
- Why: Admins need to manage databases

### Scenario 3: Everyone Accesses Files
- Everyone is in File-Server-Access group
- Result: **Access Allowed** ✓
- Why: Everyone needs company files

## 💡 What This Teaches

✅ How Azure AD works
✅ How users are organized in groups
✅ How permissions are controlled
✅ Security principle: Least Privilege
✅ Real company access models
✅ How to scale to many users

## 🎤 For Interviews

**Say:** "I created an Azure AD practice lab with users, security groups, and permission scenarios. This shows I understand how companies manage cloud access and security."

**Example:** "I restricted database access to only admins. When a developer tries to access it, they can't because they're not in the Database-Admins group. This demonstrates the principle of least privilege."

## 🚀 Skills Demonstrated

- Cloud identity management (Azure AD)
- User account creation
- Security group management
- Access control principles
- Understanding of RBAC (Role-Based Access Control)
- Security best practices

## 📖 How to Replicate

1. Go to Azure Portal
2. Create users with different roles
3. Create security groups
4. Add users to appropriate groups
5. Document who can/can't access what
6. That's it!

## 💼 For Job Applications

**LinkedIn:** "Just completed Azure AD practice lab showing cloud identity management. Created users, security groups, and permission scenarios demonstrating least privilege principles."

**Resume:** 
