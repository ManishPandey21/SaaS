# SaaS
WebApp
Contractual Correspondence DMS Web Application Development
Project Overview
The Contract Department requires a Document Management System (DMS) to efficiently handle contractual correspondence. The system should enable users to track, organize, retrieve, and collaborate on contract-related documents such as letters, claims, approvals, and other official communications.

Key Objectives
Organized Storage: Store all contractual letters with structured metadata.
Easy Search & Retrieval: Search letters using various criteria (tags, references, subjects, etc.).
Tagging & Reference Linking: Link correspondence based on contractual matters (e.g., Hindrance, EOT, Variation, Claim, DWP).
Collaboration & Drafting: Provide tools for drafting replies and tracking communication history.
Version Control & Approvals: Maintain a review and approval workflow.
Secure Access Management: Implement role-based access control (RBAC) for different users.
Core Features & Functionalities
1. Document Management
✅ Upload with Metadata

Fields: Date, Letter Number, From/To, Subject, Reference Numbers, Contract Code.
Support for PDF and Word documents with an integrated viewer.
✅ Tagging System

Predefined tags for Hindrance, EOT (Extension of Time), Variation, Claim, DWP, etc.
Option to add custom tags for contract-specific tracking.
✅ Reference Linking

Auto-detection and linking of referenced letters within uploaded documents.
Ability to manually link related letters for better traceability.
✅ Folder Organization

Users can create, rename, and organize folders by project, contract, or subject (e.g., KNPDD-01 Contract).
Bulk upload/download letters.
2. Collaboration Tools
✅ Drafting Workspace

Collaborative text editor for drafting replies and contract-related letters.
Version control with change tracking and rollback options.
✅ Comments & Annotations

Users can add comments and annotations to specific sections of letters.
Threaded discussions for contract-related clarifications.
✅ Approval Workflow

Users can route drafts for review and approval.
Email notifications for pending approvals.
3. Search & Filters
✅ Advanced Search

Full-text search across all stored documents.
Search by keywords, letter numbers, subjects, contract codes, tags, references.
✅ Filter Views

Predefined filters such as:
“Pending Replies”
“EOT Claims”
“Urgent Letters”
4. Data Management
✅ Centralized Data Table

A table view displaying all documents with columns:
Date, Letter No., From/To, Subject, Tags, Status, References.
Ability to sort, filter, and export document data.
✅ Export Options

Download individual letters (PDF/Word).
Download entire folders as ZIP files.
5. Key Pages of the Web Application
📌 Dashboard
Overview of recent letters, pending actions, and folder shortcuts.
Quick statistics:
“Letters Pending Reply”
“Overdue Claims”
“Newly Uploaded Documents”
📌 Document Upload Page
Form with fields:
Metadata: Date, Letter No., From/To, Subject, References, Contract Code.
Tags: Dropdown selection for Hindrance, EOT, Claim, etc.
File Upload: Drag-and-drop support for PDF/Word documents.
📌 Document List Page
Interactive table view with sortable columns and bulk actions (tag, archive, download).
Quick filters for commonly used queries (e.g., "Show all EOT letters").
📌 Document Detail Page
Preview document with built-in PDF/Word viewer (zoom/rotate support).
Metadata panel displaying all entered fields and tags.
Linked references to related letters (e.g., "Ref: O-SYST-KNPDD-01-LTT-00132").
Action buttons:
Reply, Edit Metadata, Download, Share.
📌 Collaboration Workspace
Draft replies using predefined templates (e.g., "EOT Approval Letter").
Track changes and compare versions of letters.
📌 Folder Management Page
Create nested folders (e.g., KNPDD-01 > EOT Claims > 2023).
Bulk download folders as ZIP files.
📌 Search Page
Full-text search across all documents.
Filters for refining search by date range, tags, status (e.g., "Approved," "Pending").
📌 Templates & Samples
Prebuilt templates for common contract letters (e.g., "Financial Implication Approval Request").
6. Advanced Features
✅ OCR Integration

Extract text from scanned letters to enable full-text search.
✅ Deadline Alerts

Automated notifications for upcoming reply deadlines (e.g., "DDC must respond by 10th Nov 2024").
✅ Role-Based Access Control (RBAC)

Admin: Full system access.
Contract Managers: Edit metadata, tag, and draft replies.
Viewers: Read-only access.
✅ Audit Log

Track who viewed, edited, or downloaded documents.
7. Sample Use Case (Based on Provided Letter)
For the letter uploaded (Kanpur-LET-JVTI-CPM-00685-E01), the following workflow would be implemented:

Upload the PDF with Metadata:

Date: 11th Oct 2022
Letter No.: Kanpur-LET-JVTI-CPM-00685-E01
From: GC
To: SYSTRA MVA Consulting
Subject: Financial Implication for EOT
Tags: EOT, Claim
References: O-SYST-KNPDD-01-LTT-00185, O-SYST-KNPDD-01-LTT-00132
System Auto-Links Related Letters:

Displays links to Ref 1, 2, 3 on the document detail page.
Assign Letter to a Folder:

Folder: KNPDD-01 > Extension Requests
Collaborate on Drafting a Reply:

Users work on a draft response using the “EOT Justification” template.
Submit for internal approval before finalizing.
Monitor and Track Progress:

The system tracks who edited/drafted the reply.
If pending, alerts contract managers about upcoming deadlines.
8. Technology Stack
✅ Frontend: React.js
✅ Backend: Node.js (Express.js)
✅ Database: MongoDB
✅ Other Essentials:

Multer (for file uploads)
PDF.js (for document preview)
ElasticSearch (for full-text search & indexing)
JWT Authentication (for security) https://github.com/ManishPandey21/SaaS
Expected Outcome
A centralized, searchable, and efficient system for managing contract correspondence that improves: ✔ Document retrieval speed
✔ Collaboration on drafting responses
✔ Tracking and linking related correspondence
✔ Ensuring compliance with contractual deadlines
