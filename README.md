🚗 Garage Management System (GMS)








📘 Project Overview

The Garage Management System (GMS) is a cloud-based application built on the Salesforce Platform to digitalize and automate operations in automotive repair workshops.
It enables garages to efficiently manage customers, appointments, vehicles, services, and billing — all from a unified, secure, and scalable environment.

By using Salesforce CRM tools, the system enhances customer satisfaction, data accuracy, and operational transparency, empowering businesses to focus more on quality service delivery rather than manual paperwork.

🎯 Objectives

✅ Automate garage operations and service tracking

✅ Improve customer engagement through CRM integration

✅ Enable real-time vehicle and billing management

✅ Provide business insights through analytics and dashboards

⚙️ Key Features
🗓️ Appointment Scheduling

Simplifies the booking process for customers

Manages daily service schedules to reduce downtime

🚘 Vehicle & Service Management

Tracks service history and maintenance records for every vehicle

Provides live service status updates

👥 Customer Relationship Management (CRM)

Stores customer details and preferences securely

Automates reminders, feedback requests, and promotions

🧾 Billing & Invoicing

Generates accurate and professional invoices

Supports multiple payment modes with tax and discount calculations

🧰 Inventory & Spare Parts Management

Tracks spare parts availability and automates reorder processes

Prevents stockouts and ensures resource readiness

📊 Reports & Dashboards

Provides visual insights into garage performance

Displays metrics like service ratings, payment trends, and workload efficiency

🧠 Technical Implementation
🔹 Platform

Salesforce Developer Edition (Cloud CRM)

🔹 Salesforce Components Used

Custom Objects: Customer Details, Appointments, Service Records, Billing & Feedback

Tabs: Created for each object for easy navigation

Lightning App: “Garage Management Application”

Fields: Text, Email, Phone, Currency, Picklist, Checkbox, Date, Formula

Validation Rules: Ensure valid inputs for vehicle numbers, service ratings, and payment status

Triggers & Apex Class: Automate service cost calculations and record updates

Flows: Automate email alerts and payment confirmations

Reports & Dashboards: Visualize performance and customer feedback

💡 Sample Apex Trigger
trigger AmountDistribution on Appointment__c (before insert, before update) {
    if (Trigger.isBefore && (Trigger.isInsert || Trigger.isUpdate)) {
        AmountDistributionHandler.amountDist(Trigger.new);
    }
}

🔐 Roles & Access Control

Roles Created: Manager, Salesperson

Public Group: Sales Team

Sharing Rules: Allow role-based record sharing (Manager ↔ Salesperson)

Profiles & Permission Sets: Defined object-level and field-level access permissions

🤖 Automation Highlights

Flows:

Auto-update billing information

Send automated “Thank You” emails after payment

Validation Rules:

Ensure data integrity (vehicle number format, rating limits, etc.)

Duplicate Rules:

Prevent duplicate customer creation using email & phone match criteria

📈 Reports & Dashboards

Custom Reports:

Service Information Report

Payment Tracking Report

Service Rating Analysis

Dashboards:

Visualizes customer satisfaction, payments, and service performance

Supports automated weekly subscriptions for manager updates

✅ Conclusion

The Garage Management System (GMS) successfully demonstrates how Salesforce can be leveraged to build a real-world cloud-based business application.
By automating core operations — from booking and billing to analytics — the system ensures improved efficiency, transparency, and customer engagement for automotive service centers.

This project highlights practical Salesforce concepts such as Custom Objects, Flows, Apex, Validation Rules, and Dashboards, providing a scalable foundation for future enhancements.

👨‍💻 Project Team
Name	Register Number	Role
M. A. Padma Kumar	953322104035	Developer
D. Sudalai Raja	953322104056	Developer
M. Piravin Kumar	953322104040	Developer
B. Muthueswaran	953322104029	Developer
S. Arikaramurthy	953322104005	Developer

Institution: Unnamalai Institute of Technology, Kovilpatti
Department: Computer Science and Engineering

🧰 Technologies Used

☁️ Salesforce Developer Edition

⚙️ Apex Programming

⚡ Lightning App Builder

🔄 Process Automation (Flows & Validation Rules)

📊 Reports & Dashboards
