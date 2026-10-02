SWIFT SHIP TRACKER

User Story:
The SwiftShip Tracker is designed to provide a centralized Salesforce-based parcel
management solution that enables customers to book parcels, track delivery status, and
manage shipments through an intuitive interface and conversational AI support. The
system manages Parcel, Delivery, Sender, and Receiver information using Salesforce
custom objects and relationships. Flows automate parcel operations and notifications,
while AgentForce AI and Prompt Builder enable customers to retrieve parcel information
and interact with the system conversationally. Delivery agents can update parcel status in
real time, while Experience Cloud, security controls, reports, and dashboards provide
secure customer access and operational visibility.

1. INTRODUCTION

1.1 Project Overview :
The SwiftShip Tracker is a Salesforce CRM solution developed to simplify parcel
booking, shipment tracking, and delivery management. It supports the complete parcel
lifecycle from booking and dispatch through tracking and delivery confirmation.
Customers can access shipment information, while delivery agents can update parcel
details and delivery status.

1.2 Purpose :
The purpose of SwiftShip Tracker is to:
● Centralize parcel and delivery information.
● Simplify parcel booking and tracking.
● Provide real-time shipment visibility.
● Automate delivery updates and customer notifications.

● Enable conversational parcel tracking using AgentForce AI and Prompt Builder.
● Improve agent efficiency through Salesforce Flows and dashboards.
● Provide secure, role-based access to customers, agents, support staff, and
administrators.

2. IDEATION PHASE
2.1 Problem Statement (Customer Problem Statement Template)

PS I am
(Customer)

I’m trying
to

But Because Which
makes me
feel

PS-1 Customer /
Sender

book a
parcel easily

booking
requires
support
assistance or
multiple
applications
parcel
operations
are not
centralized

frustrated

PS-2 Customer /
Sender

track my
parcel

I do not
have a
simple
real-time
tracking
experience

shipment
information
is difficult to
access

confused

PS-3 Delivery Agent update
parcel status
status
updates
require
manual
handling

there is a
need for
centralized
operational
tracking

concerned

PS-4 Customer receive
delivery
updates

notifications
may not be
available at
every
delivery
stage

communicat
ion needs to
be
automated

uncertain

PS-5 Admin monitor
parcel
operations

parcel flow
and delivery
performance
are difficult
to monitor

operational
data needs
centralized
reporting

concerned

2.2 Empathy Map Canvas
User Persona: Customer / Sender
● Think & Feel: Wants a simple way to book and track parcels without repeatedly
contacting support.
● Hear: Receives delivery information and status updates from the parcel service.
● See: Parcel details, tracking status, estimated delivery date, and delivery
information.
● Say & Do: Books parcels, checks tracking information, and asks for delivery
updates.
● Pain: Delays, confusion, lack of easy tracking, and dependence on support or
multiple apps.

● Gain: Real-time visibility, self-service tracking, convenient booking, and timely
notifications.

2.3 Brainstorming & Idea Prioritization
Ideas Considered
● Manual registers
● Spreadsheet tracking
● Standalone parcel portal
● Salesforce CRM with AgentForce AI

Final Selection
Salesforce CRM selected due to:
● Centralized parcel management

● Automation through Flows
● Real-time tracking visibility
● Conversational AI assistance
● Secure role-based access
● Reports and dashboards

3.REQUIREMENT ANALYSIS PHASE
3.1 Customer Journey Map
Stages:
● Parcel Booking
● Parcel Record Creation
● Dispatch & Shipment
● In-Transit Tracking
● Out for Delivery
● Delivery Confirmation
● Customer Notification
● Feedback / Support

3.2 Solution Requirements
Functional Requirements
FR No Requirement
FR-1 Parcel booking and record creation
FR-2 Parcel status tracking
FR-3 Weight management
FR-4 Estimated delivery date management
FR-5 Sender information management
FR-6 Receiver information management
FR-7 Delivery and current-location tracking

FR-8 Agent parcel status updates
FR-9 Automated customer notifications
FR-10 AI-powered parcel tracking
FR-11 Reports and dashboards
FR-12 Customer access through Experience Cloud

Non-Functional Requirements
NFR Description
Usability Intuitive Salesforce and customer-facing interface
Security Role-based and field-level access control
Reliability Accurate parcel status and delivery information
Performance Timely Flow and AgentForce responses
Availability Salesforce cloud-based access
Scalability Supports growing parcel and delivery operations
Data Integrity Controlled access and relationship-based parcel data
Maintainability Flows, prompts, topics, and configurations can be

updated

3.3 Data Flow Diagram
Flow:
Customer / Sender
↓

Parcel Booking
↓
Parcel Record
↓
Sender + Receiver Information
↓
Delivery Record
↓
Parcel Status Update
↓
Current Location & Estimated Delivery
↓
Automated Notifications
↓
Customer Tracking / AgentForce AI
↓
Reports & Dashboards

AI Tracking Flow
Customer Query
↓
AgentForce AI

↓
Prompt Builder – Retrieve Parcel Details
↓
Parcel Record
↓
Status / Weight / Estimated Delivery
↓
Conversational Response
The Prompt Builder implementation retrieves Parcel ID, Status, Weight, and Estimated
Delivery Date information for tracking responses.

3.4 Technology Stack

Layer Technology
Platform Salesforce Developer Edition
UI Lightning App Page, Lightning Record Pages, Experience

Cloud

Database Salesforce Custom & Standard Objects
Business Logic Salesforce Flows, Apex Classes
Automation Record-Triggered Flows, Auto-Launched Flows, Scheduled

Flows

AI AgentForce AI, Prompt Builder
Notifications Email Alerts & Email Templates
Processing Batch Apex
Security Profiles, Permission Sets, Role Hierarchy, Field-Level Security,

Sharing Rules
Reporting Reports & Dashboards

4. PROJECT DESIGN PHASE
4.1 Problem–Solution Fit

Problem Solution Benefit
Parcel booking is difficult Salesforce Parcel management Centralized booking
Tracking requires support AgentForce AI + Prompt

Builder

Self-service tracking

Manual status updates Salesforce Flows Automated processes

Problem Solution Benefit
Delivery communication
gaps

Email Alerts Timely notifications

Scattered shipment
information

Parcel, Delivery, Sender &
Receiver objects

Structured data

Difficult operational
monitoring

Reports & Dashboards Better visibility

Different users need
different access

Profiles, Roles & Permission
Sets

Secure access

4.2 Proposed Solution
Functional Requirements

Parameter Description
Problem Difficult and inefficient parcel booking and tracking
Solution Salesforce-based Parcel Management System
Innovation AgentForce AI + Prompt Builder for conversational self-service

tracking and automated Salesforce Flows

Impact Centralized booking, real-time tracking visibility, timely
notifications, and efficient delivery management

Business Model Parcel, customer, delivery-agent, support, and administrator

operations

Scalability Supports growing parcel operations, Experience Cloud, and

integration with external logistics systems

4.3 Solution Architecture
● Users
● Customer | Delivery Agent | Support Staff | Admin
↓
● Salesforce Lightning / Experience Cloud
↓
● SwiftShip Tracker Salesforce Platform
● Data Layer
○ Parcel
○ Delivery
○ Sender
○ Receiver
● Automation Layer
○ Flows
○ Approval Processes
○ Apex Classes

○ Batch Apex
○ Email Alerts
● AI Layer
○ AgentForce AI
○ Prompt Builder
○ Parcel Tracking Agent
● Security Layer
○ Profiles
○ Roles
○ Permission Sets
○ Sharing Rules
○ Field-Level Security
↓
● Reports & Dashboards
↓
● Parcel Tracking & Operational Insights

5. PROJECT PLANNING & SCHEDULING
5.1 Project Planning
● Agile methodology
● Epics → Stories → Story Points
● Sprint-based execution
● Velocity calculation used for estimation
Product Backlog, Sprint Schedule, and Estimation (4 Marks)
Use the below template to create product backlog and sprint schedule
Sprint Functional
Requirement
(Epic)

User
Story
Number

User Story / Task Story
Points

Priority Team
Member
s

Sprint-1 Developer
Setup

USN-1 As a system administrator, I want to
create and configure the Salesforce
environment so that I can build the
SwiftShip Tracker parcel
management system.

3 High Member1

Sprint Functional
Requirement
(Epic)

User
Story
Number

User Story / Task Story
Points

Priority Team
Member
s

Sprint-2 Data Modeling USN-2 As an admin, I want to create
Parcel, Delivery, Sender, and
Receiver objects with proper
relationships so that parcel and
delivery data is stored and
managed systematically.

5 High Member2

Sprint-2 Data Modeling USN-3 As a staff member, I want dedicated
tabs and a Lightning App for
SwiftShip modules so that I can
easily navigate and manage parcel
and delivery operations.

5 High Member3

Sprint-3 Automation USN-4 As a system, I want to validate
parcel details, mandatory fields, and
booking inputs so that invalid or
incomplete parcel records are
prevented.

3 High Member4

Sprint-3 Automation USN-5 As a delivery coordinator, I want
automated Flows to update parcel
status and delivery information so
that parcel processing requires
minimal manual effort.

3 High Member4

Sprint-4 Apex USN-6 As a system, I want Apex triggers
and classes to automatically
perform critical parcel and delivery
actions so that important processes
are handled accurately.

5 High Member1

Sprint-4 Apex USN-7 As an inventory/operations
manager, I want Batch Apex jobs to
process and update parcel or
delivery records automatically so
that operational data remains
accurate and up to date.

5 High Member2

Sprint-5 Reports USN-8 As a manager, I want reports
showing parcel status, delivery
performance, and operational
metrics so that I can monitor
SwiftShip operations and make
informed decisions.

4 High Member3

Sprint-6 Dashboards &

AI

USN-9 As a manager, I want dashboards
showing parcel status, delivery
performance, and key metrics, while
Agentforce provides AI-powered
tracking assistance, so that I can
monitor operations efficiently.

4 Medium Member4

Project Tracker, Velocity & Burndown Chart: (4 Marks)

Sprint Total Story
Points

Duratio
n
Sprint Start
Date

Sprint End Date
(Planned)

Story Points
Completed
(as on
Planned End
Date)

Sprint Release
Date (Actual)

Sprint-1 20 6 Days 24 Oct 2022 29 Oct 2022 20 29 Oct 2022
Sprint-2 20 6 Days 31 Oct 2022 05 Nov 2022
Sprint-3 20 6 Days 07 Nov 2022 12 Nov 2022
Sprint-4 20 6 Days 14 Nov 2022 19 Nov 2022
Sprint-5 20 6 Days 21 Nov 2022 26 Nov 2022
Sprint-6 20 6 Days 28 Nov 2022 03 Dec 2022

6. Project Development Phase:

Phase 1: Requirement Analysis & Planning
Objective:
“Customers often face delays and confusion while booking, tracking, and managing
parcel deliveries because they need to call support or use multiple apps. A
conversational AI agent can simplify this by allowing customers to book parcels, get live
tracking, and manage deliveries in one place.”
Key Requirements:
• Requirement gathering from end users and delivery agents.
• Defining system scope and user personas (Customer, Agent, Admin).
• Designing the data model with relationships between Parcel, Sender, Receiver, and
Delivery.
• Identifying use cases such as parcel booking, tracking, and delivery update
automation.

• Selecting tools: Salesforce Flows, Prompt Builder, and AgentForce AI.
Defining Project Scope & Objectives
Project Scope:
1. Build a scalable CRM solution for parcel delivery businesses to manage customer bookings,
shipments, and delivery operations efficiently.
2. Support the end-to-end parcel lifecycle — from parcel booking → dispatch → tracking →
delivery confirmation.
3. Include comprehensive data model design, automation (Flows, Apex, Email Alerts),
AI-powered prompt builder, and reporting dashboards for effective management.
4. Provide role-based access for admins, delivery agents, and customers through Salesforce
profiles, permission sets, and Experience Cloud.
5. Ensure real-time parcel visibility for customers and simplified operational tracking for agents
through AI-integrated conversational support.
Objectives Summary:
● Streamline parcel operations by automating booking, tracking, and delivery notifications to reduce
manual updates.
● Improve customer satisfaction with transparent, real-time shipment status and self-service tracking
options.
● Enhance agent efficiency through centralized dashboards and guided Flows for quick status
updates.
● Enable business insights with reports and dashboards showing parcel trends, delivery
performance, and agent activity.
● Ensure security and reliability by implementing Salesforce role hierarchies, sharing rules, and
audit-based data access.

Gathering & Analysing User Needs
Users Involved:

● Customers / Senders – End users who book parcels, track deliveries, and
receive real-time updates through the portal or AI agent.
● Delivery Agents – Manage assigned parcels, update delivery status, and ensure
timely handover to customers.
● Customer Support Team – Handle delivery-related issues, respond to customer
queries, and ensure smooth communication.
<img width="1545" height="822" alt="image" src="https://github.com/user-attachments/assets/4814ab6a-79ef-46d3-aee2-4ef2fc5a3cb2" />
<img width="1851" height="851" alt="image" src="https://github.com/user-attachments/assets/3aab465f-6da8-4ff7-af59-23c848a9b8e8" />

<img width="1867" height="901" alt="image" src="https://github.com/user-attachments/assets/602c36bd-f73c-44d3-a394-7852e4fb4297" />
