# BAU Cricket Club – Cloud Computing Project

## Project Overview
This is a static website created for the BAU Cricket Club as part of our ISIT 225 Cloud Computing project at Bay Atlantic University.

We built the website using HTML and CSS and hosted it on Google Cloud Storage. Our goal was to learn how to publish a website using cloud services without managing our own web server.

## Live Website
https://storage.googleapis.com/isit225-static-website/index.html

## GitHub Repository
https://github.com/aryasathwara-cell/isit225-static-website

## Cloud Services Used
- Google Cloud Storage: Object storage for hosting the HTML and CSS website files.
- Google Cloud IAM: Controls access to the storage bucket.
- Object Versioning: Keeps previous versions of files when they are replaced.
- Lifecycle Management: Automatically deletes non-current file versions after 30 days.

Cloud Storage is a managed cloud storage service. We do not need to manage a virtual machine or operating system.

## Website Files
- index.html – Main website page
- style.css – Website design and styling
- diagram.png – Cloud architecture diagram
- README.md – Project documentation

## Architecture
User → Web Browser → Google Cloud Storage → HTML and CSS Website

Architecture diagram: https://github.com/aryasathwara-cell/isit225-static-website/blob/main/diagram.png

## Security Controls
1. IAM: Public users have read-only access to the website files through the Storage Object Viewer role.
2. Object Versioning: Allows recovery of previous file versions.
3. Lifecycle Rule: Deletes non-current versions after 30 days to help control storage costs.

Public access is limited to reading objects; visitors cannot edit or upload website files.

## Object Storage vs. VM Disk

| Feature | Cloud Object Storage | Virtual Machine Disk |
|---|---|---|
| Purpose | Stores files as objects | Stores operating system and application files |
| Server management | No server management required | VM and operating system management required |
| Access | Through cloud APIs and URLs | Through the virtual machine |
| Scaling | Managed by cloud provider | Depends on VM and disk configuration |
| Best use | Static websites, images, backups | Operating systems, databases, applications |

We chose Cloud Storage because our website only needs HTML and CSS files. It is simple to manage and does not require us to run a web server.

## Testing
- Website opens successfully in a regular browser.
- Website opens in Incognito mode without signing in.
- HTML and CSS display correctly.
- Object Versioning has been enabled.
- A 30-day lifecycle rule has been created.
- Previous-version restoration test: Pending verification.

## Remaining Tasks
- Demonstrate restoring an older version of a test file.
- Save screenshots of the restoration test and cloud configuration.
- Verify all project and presentation links.

## Team – Gujju Gang
- Arya
- Jenish Patel
- Jasmeet Kaur
- Prerak Barot

Our team worked together on website development, cloud configuration, GitHub, documentation, testing, and presentation.

## Course
ISIT 225 – Cloud Computing
Bay Atlantic University
