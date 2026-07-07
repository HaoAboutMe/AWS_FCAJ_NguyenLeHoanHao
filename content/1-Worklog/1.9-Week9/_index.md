---
title: "Week 9 Worklog"
date: 2026-07-04
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Week 9 Objectives:

* Upgrade and optimize the web interface, developing a new modern layout that works seamlessly across various screen resolutions.
* Deploy the Frontend using Amazon S3 Static Web Hosting combined with Amazon CloudFront as CDN to optimize global page load speeds.
* Resolve Lambda Cold Start issues to improve overall system performance and reduce response latency.
* Research, standardize the infrastructure architecture, and design a detailed AWS Architecture Diagram for the Cloud Battleship application.

### Tasks performed during the week:

| Day | Task | Start Date | Completion Date |
| --- | ---- | ---------- | --------------- |
| 2   | - Refactored CSS code and UI components, starting the implementation of the new modern web interface design <br> - Optimized the layout of match status displays and the lobby placement setup area | 06/29/2026 | 06/29/2026 |
| 3   | - Continued refining the new UI: polished hover effects, shadows, and glassmorphism in both Light and Dark modes <br> - Resolved layout clipping and responsive alignment issues for the control menu and mobile buttons | 06/30/2026 | 06/30/2026 |
| 4   | - Researched strategies to mitigate serverless Lambda Cold Start latency <br> - Developed a warm-up Lambda function to send periodic heartbeat signals to the core business logic Lambdas <br> - Configured EventBridge Rules in the SAM template to automatically trigger the warm-up process every 5 minutes | 07/01/2026 | 07/01/2026 |
| 5   | - Deployed the static Frontend on Amazon S3 and configured appropriate S3 Bucket Policies <br> - Created and configured an Amazon CloudFront Distribution as the CDN in front of S3, optimizing caching policies and integrating SSL/TLS for secure HTTPS connections <br> - Troubleshot Redirect URI issues during Cognito User Pool integration with Facebook Login | 07/02/2026 | 07/02/2026 |
| 6   | - Researched and designed the AWS Architecture Diagram, detailing the REST API, WebSocket (APIGW), Lambda, DynamoDB, and S3/CloudFront data flows <br> - Visualized the architecture using Mermaid diagrams for inclusion in the project documentation | 07/03/2026 | 07/03/2026 |
| 7   | - Conducted end-to-end performance testing of the system post-deployment with the warm-up Lambda and CloudFront CDN distribution <br> - Finalized architectural documentation, addressed outstanding CSS issues, and compiled the Week 9 progress report | 07/04/2026 | 07/04/2026 |

### Achievements:

* **Enhanced and Upgraded User Interface (UI):**
  * Redesigned the visual theme to feel more modern, improving contrast and grid visual cues for the board and custom-painted ships.
  * Refined mobile responsive views to eliminate button layout clipping or text-wrapping on smaller screens.

* **Successful Frontend Deployment on AWS:**
  * Deployed the static Frontend onto Amazon S3 Static Web Hosting, reducing server resource loads.
  * Integrated Amazon CloudFront to distribute the static content with low latency and secure HTTPS connections globally.

* **Resolved Lambda Cold Start Issues:**
  * Reduced first-request API latency from several seconds to under 200ms using the automated scheduler powered by Amazon EventBridge.

* **Designed a Professional AWS Architecture Diagram:**
  * Created a comprehensive and detailed architecture diagram, providing clear documentation of serverless services and client-server communication channels.
