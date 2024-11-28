# Oracle DBA portfolio
Welcome to my Oracle DBA portfolio! I am an experienced Database Administrator with 3.6 years of expertise in managing, optimizing, and securing Oracle databases. This portfolio showcases my projects, technical skills, certifications, and contributions.

---

## **About Me**  
- **Name**: [Mrinmoy Das]  
- **Experience**: 3.6 years as an Oracle Database Administrator  
- **Specialization**: Database installation, configuration, backup/recovery, performance tuning, and high availability.  
- **Email**: [mrinmoydas9064@gmail.com]  
- **LinkedIn**: [LinkedInProfile](https://www.linkedin.com/in/mrinmoy-das-b7210a158?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app) 

---

## **Skills**  
- **Database Administration**: Oracle 11g, 12c, 19c  
- **Backup and Recovery**: RMAN, Data Pump  
- **High Availability**: Oracle RAC, ASM, Data Guard  
- **Performance Tuning**: SQL optimization, indexing, OEM  
- **Scripting**: Shell scripting, PL/SQL, Python  
- **Cloud**: Oracle Cloud Infrastructure (OCI), AWS RDS for Oracle  
- **Tools**: Oracle SQL Developer, Toad, Oracle Enterprise Manager (OEM)  

---

## **Certifications**  
- Oracle Certified Associate (OCA) – Oracle Database 12c  
- Oracle Certified Professional (OCP) – Oracle Database Administration  
- ITIL Foundation Certification  

---

## **Projects**  

### 1. **Oracle Database Migration**  
- **Objective**: Migrated a 5TB Oracle 11g database to Oracle 19c with zero downtime.  
- **Skills Used**: RMAN, Data Pump, Shell Scripting, OEM.  
- **Outcome**: Improved performance by 20% and ensured high availability.  
- **Repository**: [Database Migration Scripts](https://github.com/your-repo/migration-scripts)

### 2. **Automated Backup and Recovery System**  
- **Objective**: Designed and implemented an automated backup and recovery solution using RMAN.  
- **Skills Used**: RMAN, Shell Scripting, OEM.  
- **Outcome**: Reduced manual intervention by 30% and ensured 100% recovery compliance.  
- **Repository**: [Backup Automation Scripts](https://github.com/your-repo/backup-automation)

### 3. **Performance Optimization for Financial Database**  
- **Objective**: Tuned SQL queries and optimized indexes for a financial application, reducing query response time from 15 seconds to 3 seconds.  
- **Skills Used**: SQL Tuning, OEM, Index Management.  
- **Outcome**: Improved application performance and user satisfaction.  

---

## **Sample Scripts**

### 1. **RMAN Backup Script**  
Automates daily incremental and weekly full backups.  
```bash
#!/bin/bash
ORACLE_HOME=/u01/app/oracle/product/19.0.0/dbhome_1
export ORACLE_HOME
ORACLE_SID=orcl
export ORACLE_SID

rman target / <<EOF
RUN {
  BACKUP INCREMENTAL LEVEL 1 DATABASE;
  BACKUP ARCHIVELOG ALL DELETE INPUT;
}
EOF


