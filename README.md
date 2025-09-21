# Astrido Fleet Companion

## Background
Since July 2022, Toyota has introduced the **T-Care After-Sales Program** across all official Toyota workshops.  
This program was designed to enhance customer satisfaction by providing two key benefits:
- Free service and spare parts for up to **7 periodic services**, or within **3 years / 60,000 km**.  
- **Extended Warranty** for 1 year / 20,000 km, provided that customers consistently perform maintenance every 6 months.  
Despite these significant benefits, the implementation of T-Care at **Astrido Toyota Karawaci** during the period of **January–March 2024** was not optimal.  
The claim rate remained relatively low:
- 1st Service: 84%  
- 2nd Service: 86%  
- 3rd Service: 89%  
Further analysis indicated that **Fleet Customers** were the primary factor hindering the achievement of T-Care claim targets.
This situation directly affects fleet customers, as they risk losing their entitlement to the **Extended Warranty**, which protects the long-term value of their vehicles.
### Fleet Customer Composition at Astrido Toyota Karawaci:
- PT. Mitra Pinasthika Mustika Rent (MPM Rent) – 81%  
- PT. Autorent Lancar Sejahtera – 6%  
- PT. Bestindo Cakra Utama – 3%  
- PT. Anugrah Inti Abadi – 2%  
- Others – 9%  
As a follow-up, the team conducted a visit to **MPM Rent**.  
From the discussion, several key challenges were identified that contributed to the low T-Care claims:
- Pool Managers & Management had **no visibility** into Toyota units’ claim status.  
- There was **no routine monitoring system** for T-Care claims.  
- Pool Managers had **no KPI related to T-Care**, and Management had not assigned them responsibility to ensure all units submitted claims.  
---

## 🎯 Objectives
The development of **Astrido Fleet Companion** aims to provide a tool that supports Pool Managers and Management in optimizing T-Care claims, with a focus on:

- **Simplifying periodic service reminders**  
  Helping Pool Managers remind end-users in a timely manner based on automated service due dates.  

- **Enhancing coordination between Astrido Karawaci & Pool Managers**  
  Providing an integrated communication platform covering service schedules, bookings, and mobile service requests.  

- **Delivering a real-time monitoring dashboard**  
  Offering comprehensive visibility to automatically, accurately, and promptly track T-Care claim progress.  

---

## 🛠️ Tools & Technology
- **AppSheet** → Front-end application for Pool Managers & Management as the main interface.  
- **Google Sheets** → Centralized database for storing service schedules and T-Care claim records.  
- **Looker Studio** → Real-time monitoring dashboard for service compliance and claim progress.  

---

## 🔄 Flow of Astrido Fleet Companion
**Astrido Fleet Partner** is a collaboration between **Astrido Toyota** and **MPM Rent**, involving:  

- Astrido Toyota Kebon Jeruk PICs: Admin, MRA, and Service Manager  
- MPM Rent PICs: CRM, Pool Manager, and Management  

### Detail Flow:
1. **System Generates Data (Automated Data Processing)**  
   - **PIC**: Admin  
   - **Process**: Admin updates claim database weekly (Astrido Group) and monthly (Toyota National).  
     System automatically generates service schedules, claim status, punctuality status, and overdue service.  
   - **Outcome**: Structured data ready for reminders & monitoring.  

2. **Priority Service Reminder by Punctuality & Claim Status (Smart Reminder System)**  
   - **PIC**: Pool Manager, CRM MPM, MRA, Service Manager  
   - **Process**: System displays service schedules.  
     Reminders sent by priority:  
     - Eligible & Punctual → 1st Priority (Due), 2nd Priority (Overdue)  
     - Not Eligible & Late → 3rd Priority (Due), 4th Priority (Overdue)  
   - **Outcome**: Reminders are structured based on claim priority & punctuality.  

3. **After Reminder Action (Follow-up & Service Tracking)**  
   - **PIC**: Service Manager, Pool Manager, Ticketing, Customer  
   - **Process**:  
     - Customer receives reminder → asked “Booking this month?”  
     - If booking confirmed → Service performed → System updates claim data & next 6-month reminder.  
     - If no booking → Unit categorized as Overdue Service → System prepares reminder next month.  
   - **Outcome**: Unit status always updated (Claimed, Potential, Overdue).  

4. **Monitoring Dashboard & PDCA Cycle (Continuous Monitoring & Improvement)**  
   - **PIC**: Service Manager, Pool Manager, Management  
   - **Process**: Data automatically synced to dashboard.  
     Monthly evaluation of T-Care claims → PDCA cycle applied if targets not met.  
   - **Outcome**: Continuous system improvement, optimized T-Care claims, and warranty benefits secured.  

---

## 📲 Application & Dashboard
The entire workflow is integrated in one system and monitored in **real time**.

- **Astrido Fleet Companion App (AppSheet)** → Main tool for Pool Managers & CRM to manage schedules, reminders, and follow-ups.  
- **Monitoring Dashboard (Looker Studio)** → Provides interactive visualizations of:  
  - T-Care claim status per unit (claimed / overdue)  
  - Service punctuality (on time / late)  
  - Reminder & booking progress  
  - Monthly claim evaluation & achievement  

This integration enables Management, Pool Managers, and Astrido Karawaci’s After-Sales team to make **faster, more accurate, and data-driven decisions**.  

🔗 **Demo Application**: [AppSheet Link](https://www.appsheet.com/start/ecc8a290-20c2-45f2-a150-8e9590c83c82)  
*(Username: Gangga | Password: Gangga)*  

🔗 **Monitoring Dashboard**: [Looker Studio Link](https://lookerstudio.google.com/reporting/2e9e3f09-b06c-4a95-8c92-1a9b3110ecf9/page/p_9b511l8cwd)  

---

## 📊 Results & Insights
The implementation of **Astrido Fleet Companion** has streamlined the previously complex process of T-Care claim monitoring.  

- Pool Managers → Monitor claims in real time for faster & targeted follow-ups.  
- CRM → Easier reminders and follow-ups based on due dates.  
- CRM & Ticketing → Access to service & claim history for personalized communication.  
- Management → Interactive dashboard showing:  
  - T-Care claim status per unit  
  - Punctuality & overdue status  
  - Effectiveness of reminders & bookings  
  - Monthly target evaluation  

**Result:**  
The fragmented and hard-to-monitor T-Care claim process has transformed into a system that is **automated, integrated, and transparent**.  

---

## 📝 Key Learnings
1. **Centralized Data Accelerates Processes**  
   Integrated database reduces duplication, minimizes errors, and speeds up access.  

2. **Effective Automated Reminders Increase Claims**  
   Priority-based reminders outperform mass reminders by targeting actual needs.  

3. **Multi-Stakeholder Collaboration is Essential**  
   Alignment of Pool Managers, CRM, Service Advisors, and Management ensures process consistency.  

4. **Real-Time Dashboard Ensures Transparency**  
   Single dashboard visualizes claims, punctuality, and reminders for data-driven decision-making.  

5. **Continuous Improvement via PDCA Cycle**  
   Ongoing monitoring ensures adaptability to real-world conditions and targets.  

---
