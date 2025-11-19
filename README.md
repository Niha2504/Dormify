1. Team Name:Dormify

2. Problem Statement:Inefficient and Opaque Hostel Bed Allocation and Request Management.
   Current hostel bed allocation relies on manual, paper-based processes, leading         to delayed updates on vacancies and slow, non-transparent student request/approval             cycles. This results in administrative burden for wardens, student uncertainty regarding       room status, and allocation friction when attempting to secure or transfer to a vacant  bed.

3. Idea Description:Real-Time Hostel Bed Allocation and Request Management System.
    A dual-interface mobile application (for Students) and web portal (for Wardens)that provides real-time visibility into hostel bed vacancies and facilitates a digital         request-and-approval workflow for bed allocation.

4. Key Features
   The core functionality of HostelHub centers on a secure, dual-interface system. It requires separate sign-in and sign-up for both Students and Wardens. The most critical feature is the Warden's ability to provide real-time vacancy status updates for all beds. Students can then view these vacancies and formally request a specific bed. The Warden reviews these requests via a dedicated dashboard and can Accept or Reject the allocation, which triggers an immediate notification to the respective student.

5. Tech Stack
   The system will be technologically robust, built upon a modern, scalable stack. The student-facing mobile application will be developed using React Native or Flutter to ensure cross-platform compatibility. The Warden administrative portal will be a responsive web application built with React or Vue.js. The backend logic will be handled by Node.js (Express) or Python (Django/Flask), with a flexible MongoDB database managing all user, room, and request data. Socket.IO or Firebase Cloud Messaging (FCM) will be utilized for the essential real-time communication and push notifications.

6. Notes
   Effective development requires several key operational considerations. The development team must maintain separate codebases for the student app and the warden portal, ensuring maximum efficiency without compromising the unified API. Furthermore, security protocols must be strictly implemented, especially for Warden accounts, as they handle sensitive allocation data. The underlying database structure is crucial and must clearly define the status of every bed using the hierarchy: Hostel → Block → Room → Bed.

7. Timeline
   The entire Minimum Viable Product (MVP) is projected to be completed in a focused 15-week timeline. This period begins with a two-week phase for detailed planning and system setup. The subsequent phases dedicate six weeks to developing the core features (like user authentication and vacancy display) and four weeks to building the complex allocation request-and-approval workflow. The project concludes with a three-week phase dedicated to thorough end-to-end testing and final deployment preparation.
