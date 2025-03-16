Charle8.com

Overview

This project showcases the complete design and deployment of a static website on AWS using Terraform, from the ground up. It was inspired by and evolved from my work on charle8.com, but rebuilt as a structured, fully automated Infrastructure as Code (IaC) solution. The purpose of this project is to demonstrate how to host a static website securely, efficiently, and repeatably on AWS without manual console work — using Terraform to orchestrate every step of the deployment.
The final result is a scalable, production-ready website infrastructure that uses AWS best practices for security, automation, and DNS/SSL configuration.

Problems and Troubleshooting Summary

Problems / Solution

S3 Public Access Blocked Error	
- Adjusted S3 public access block settings and fine-tuned bucket policy to allow public read but block other actions.

403 Forbidden Error on S3 Website
- Corrected bucket policies and ensured correct index/error documents were specified.

SSL Certificate DNS Validation Failure
- Automated DNS record creation via Route 53 for ACM validation, ensuring domain ownership confirmed.

Domain Not Routing to S3 Website
- Corrected Route 53 alias records to point to the right S3 website endpoint and ensured TTL propagation time was accounted for.

IAM Permission Denied on Deployments
- Refined IAM policies to grant required permissions without over-privileging.


Including many many more involving css, html, js for the website creation portion
- Fully created from scratch
