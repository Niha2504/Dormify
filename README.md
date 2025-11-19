1. Team Name:Dormify

2. Problem Statement:
Title: Inefficient and Opaque Hostel Bed Allocation and Request Management.
Statement: Current hostel bed allocation relies on manual, paper-based processes, leading         to delayed updates on vacancies and slow, non-transparent student request/approval             cycles. This results in administrative burden for wardens, student uncertainty regarding       room status, and allocation friction when attempting to secure or transfer to a vacant  bed.

3. Idea Description:Real-Time Hostel Bed Allocation and Request Management System.
    Concept: A dual-interface mobile application (for Students) and web portal (for Wardens)       that provides real-time visibility into hostel bed vacancies and facilitates a digital         request-and-approval workflow for bed allocation.

4. Key Features
Category------------------>Feature Description	
User Authentication------->Separate Sign-in/Sign-up for Students and Wardens.
Warden Login------>Warden authentication must be verified against an internal college database.
Real-Time Vacancy Status-------->Warden must update a bed status (Occupied/Vacant) immediately.
Student Bed Request----->Students can select an available vacant bed and send a formal request.
Warden Request Dashboard-------->Warden can view all pending student requests, student details, and the selected bed.
Request Action------>Warden can Accept (Allocates the bed) or Reject (Sends rejection message) the student's request.
Student Notification------->Instant notification (In-app/Push) of the Warden's decision (Accept/Reject).
Waitlist Feature------->For a preferred room/block, students can join a waitlist if no beds are vacant.
Room Filtering--------->Students can filter vacancies by room type, block, and price.
Warden Re-allocation Tool--------->If a student selects a bed just before it's taken, the Warden can message the student asking them to choose another, or directly remove the invalidated selection.
Hostel Rules/FAQ------------>A section for displaying common hostel regulations and FAQs.

5. Technical Stack
Component------->Technology------->Rationale
Frontend(Mobile App)------>React Native/Flutter------->Allows a single codebase for both Android and iOS mobile apps(for Students).
Frontend(Warden Portal)------>React/Vue.js-------->Robust framework for a data-heavy, real-time administrative dashboard.
Backend(API)--------->Node.js(Express)/Python(Django/Flask)-------->Efficient for handling simultaneous, real-time data updates and notifications.
Database--------->MongoDB(NoSQL)--------->Highly flexible schema for user data, room status, and request logs. Good performance for real-time reads/writes.
Real-Time Messaging--------->Socket.IO/Firebase Cloud Messaging(FCM)--------->Essential for instant push notifications to students upon a Warden's decision or vacancy update.

6. Notes
   Collaboration: The team should maintain separate code branches for the StudentApp and the
   WardenPortal but use a unified API and database to ensure data consistency.
   Security: Warden accounts must have higher security protocols, including multi-factor          authentication, as they manage critical allocation data.
   Data Structure: The core database schema must accurately map Hostel→Block→Room→Bed, with a     clear status flag (Vacant/Occupied) and an AllocatedTo field (Student ID).

7. Timeline 

Phase--------->Duration(Weeks)--------->Key Milestones
Phase 1:Planning & Setup------->2 Weeks--------->Finalize detailed wireframes. Setup Git repositories, API, and core database structure.
Phase 2:Core Features----------->6 Weeks-------->Implement Authentication (Student/Warden). Real-Time Vacancy Display. Warden Update Status feature.
Phase 3:Allocation Workflow-------->4 Weeks--------->Implement Student Request Submission. Warden Approval/Rejection Logic. Notification System.
Phase 4:Testing & Deployment--------->3 Weeks----------->End-to-end testing, bug fixing. Beta launch with a small group of students/wardens.
Total Estimated Time------------>15 Weeks--------->Full release of the Minimum Viable Product.
