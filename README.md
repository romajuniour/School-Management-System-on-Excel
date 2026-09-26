# School Management System on Excel
This is a School Management System on Excel and is designed to help schools manage student records, school fees, classes, users, and other school administration tasks. Created on Excel using macros.

Offline Excel School Management System for your school. Best for Remote/Off grid schools with no internet access or people who just love working on Excel.

**Features**

✅ Multi-user Excel System

✅ Admin Dashboard 

✅ Class & Stream Management

✅ School Fees Management & Payment Tracking

✅ User Roles & Access Management

✅ Reports and Receipts


**🛠️ Tools Used**
- Microsoft Excel
- Pivot Tables
- Charts
- Excel Formulas
- Data Validation
- Conditional Formatting
- Text Files



**System Architecture**
📁 SCHOOL SYSTEM (root)

│

├── 📁 DATA

│   ├── 📁 CFG		                  # Configuration files (fast text/CSV, one encrypted Excel for users)

│   │   ├── Usr.cfg       	 	    # Hash or ROT 13 – user credentials & permissions

│   │   ├── Sid.cfg                # Hash or ROT 13  (one line)

│   │   ├── Fees.csv               # Plain CSV – fee structures

│   │   ├── ClassTeacher.csv       # Plain CSV – class‑teacher mapping

│   │   └── TermControl.csv        # Plain CSV – term dates/status

│   ├── 📁 CNT		                # Plain text counters (fast read/write)

│   │   ├── Admission.dat    	   # Last admission number

│   │   ├── Allocation.dat	       # Last allocation number

│   │   └── ... (other counters)

│   ├── 📁 LCK                     # Temporary lock files for soft‑locking

│   ├── Audit.lck                   # Structured audit log (I don't think its relevant)

│   ├── Registry.lck                # Student & guardian data (can be per Admission number)

│   ├── Ledger_2026.lck             # Financial data (partitioned by year or per invoice/receipt number)

│   └── Ledger_2025.lck

│

├── 📁 LOG

│   └── Log_2026-03-16.log            # Plain text – all macro actions, errors, debug info

│
├── 📁 Assets
│   ├── Students							# Folder for Students Pictures saved per admission number

│   ├── School								# Folder for School logo Pictures

│   └── ...

│

├── Operations.xlsm                    # Merged registration & finance (or keep separate)

├── Reports.xlsm                       # Reporting / dashboards

└── Admin.xlsm                         # Optional – user management tool (can be locked away)


**📂 Project Files**

https://drive.google.com/file/d/1daFLNlx0VHAhBLiroC5edrOojBZ8isRn/view?usp=drive_link

**Videos**

1.  https://youtu.be/Cl2-hcuM6Cw?si=uxmj3YmlObp4G67h

2.  https://youtu.be/7hvY0lb_7Tk?si=Z3ydwgymOay_PMbt
