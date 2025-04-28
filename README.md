# Project Overview
The Cre8iveSkill Service Dashboard is a web portal enabling customers to upload design files, request quotes, track orders, review digital proofs, and place re-orders—all within a single, cohesive interface 
Make a README
. It embodies an Agile-Hybrid approach, translating strategic goals from the BRD into precise, testable requirements in the FRS 
GitHub
.

Documentation
We maintain two core documents in docs/:

Business Requirements Document (BRD)
Captures vision, objectives, stakeholders, epics, user stories, and non-functional requirements.
📂 docs/Cre8iveSkill_Customer_Service_Dashboard_BRD.pdf 
GitHub Docs

Functional Requirements Specification (FRS)
Details system behaviors as “shall” statements, organized by feature modules (File Upload, Quotation, Tracking, etc.) with priorities and stimulus–response sequences.
📂 docs/Cre8iveSkill_Service_Dashboard_FRS.pdf 
GitHub

Tip: Keep the README concise; for in-depth details, refer to the full PDFs in docs/ 
Reddit
.

Key Features
File Upload & Preview: Accepts .AI, .DST, .EPS, .PNG, .JPG (≤50 MB) with instant preview in under 5 s 
FreeCodeCamp

Parameter Capture: Interactive forms for stitch types, thread colors, fabric, dimensions, and special instructions 
GitHub

AI-Powered Quoting: Generates cost estimates in ≤ 30 s, with manual override options for operations 
GitHub Docs

Order Tracking: Kanban-style pipeline with stage ETAs and automated notifications 
blogs.incyclesoftware.com

Proofing & Approval: High-resolution proof viewer, inline annotation tools, and one-click sign-off 
GitHub Docs

Order History & Reordering: Full archive of past orders, downloadable files, and “Reorder” workflow 
Reddit

In-Dashboard Messaging: Threaded order-specific chats with contextual FAQs and tutorials 
Reddit

Tech Stack

Layer	Technology
Frontend	React · Tailwind CSS · Framer Motion
Backend API	Node.js · Express · REST
Database	MySQL (encrypted columns)
Auth	OAuth 2.0
Quoting Engine	Python Flask · scikit-learn
File Storage	AWS S3
Notifications	SendGrid · WebSocket
Deployment	Docker · Kubernetes · AWS EKS
Getting Started
Clone the Repo

bash
Copy
Edit
git clone https://github.com/YourOrg/cre8iveskill-service-dashboard.git
cd cre8iveskill-service-dashboard
Install Dependencies

bash
Copy
Edit
# Backend
cd api && npm install

# Frontend
cd ../web && npm install
Configure Environment

bash
Copy
Edit
cp api/.env.example api/.env
cp web/.env.example web/.env
Fill in database URLs, API keys, and AWS/S3 credentials.

Run Locally

bash
Copy
Edit
# In one terminal
cd api && npm start

# In another terminal
cd web && npm start
Open http://localhost:3000 in your browser.

Repository Structure
graphql
Copy
Edit
cre8ive-dashboard/
├── api/                    # Express backend
├── web/                    # React frontend
├── docs/                   # BRD and FRS PDFs, wireframes
├── .env.example
├── docker-compose.yml
└── README.md
Contributing
We welcome your contributions! Please:

Fork the repo

Create a feature branch (git checkout -b feature/MyFeature)

Commit (git commit -m "Add MyFeature")

Push (git push origin feature/MyFeature)

Open a Pull Request

See docs/CONTRIBUTING.md for full guidelines 
GitHub
.

License
MIT © Cre8iveSkill. See LICENSE for details.

Contact
Lead: Sonal M. Khobragade (sonal@cre8iveskill.com)

Issues: Use this repo’s Issues tab for bug reports and feature requests

Docs: Browse docs/ for BRD, FRS, UI mockups
