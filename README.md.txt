# Garage Management System - Salesforce Project

## Project Overview
The **Garage Management System (GMS)** is a Salesforce-based application designed to manage automotive repair operations efficiently. It helps garages maintain customer information, schedule appointments, track services, manage billing, and generate reports and dashboards for better business insights.

---

## Features Implemented
1. **Objects & Relationships**
   - Customer Details
   - Appointments
   - Service Records
   - Billing Details & Feedback
   - Lookup relationships between objects

2. **Fields**
   - Standard fields: Phone, Email, Vehicle Number Plate
   - Custom fields: Checkboxes for services, Picklists, Currency fields, Ratings, Date fields

3. **Automation**
   - **Apex Trigger & Handler**: Automatically calculate service amount based on selected services.
   - **Flows**:
     - Update Billing Amount when payment is completed
     - Send Email Alert to Customer
     - Update Service Status after Quality Check

4. **Validation Rules**
   - Vehicle number plate format validation
   - Rating should be between 1 to 5

5. **Reports & Dashboards**
   - Custom Report Type: Service Information
   - Line Chart Report for Service Ratings
   - Dashboard for visual analytics
   - Scheduled subscriptions

6. **Profiles & Roles**
   - Manager & Salesperson profiles with specific permissions
   - Role hierarchy and sharing rules

---

## Sample Screenshots
- Customer Details New Record
- Appointment with Service Amount
- Service Record before and after Quality Check
- Billing Details Record
- Service Information Report with Line Chart
- Service Rating Dashboard

*(All screenshots are saved in the `Screenshots` folder.)*

---

## How to Use
1. Login to Salesforce and access the **Garage Management App**.
2. Create **Customer Details** records.
3. Create **Appointments**, select services, enter Vehicle Number Plate.
4. Create **Service Records** and mark Quality Check as True to automatically update Service Status.
5. Create **Billing Records** and mark Payment Status to update Payment Paid via Flow.
6. Access **Reports** and **Dashboards** for analytics.

---

## Apex Code
- **AmountDistributionHandler.cls**: Calculates service amount automatically.
- **AmountDistribution.trigger**: Executes handler before insert or update on Appointment.

---

## Authors
- Ragul Ananth P: [johnebenezer08@gmail.com ]
