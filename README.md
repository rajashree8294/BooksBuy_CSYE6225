# BooksBuy_CSYE6225

## TECH STACK

- Angular 9, NodeJS, MySQL, Sequelize
- Amazon Web Services (AWS) - EC2, S3, Lambda Function, Route53, SNS, SES, CloudDeploy, CodeWatch 
- Continuous Integration and Continuous Deployment (CI/CD) - CircleCI 
- Infrastructure as a Code (IaaC) - Terraform
- Session management - JWT Token at the server side, Session Storage on the Frontend.

## FUNCTIONAL FEATURES:
- SIGN UP/LOGIN : Users can create account in the BooksBuy. Users credentials are secured using BCrypt password hashing scheme with Salt

- ROLE BASED PROFILE VIEW : A user can be a BUYER or BUYER & SELLER. According to the role, users can see their dashboard. Seller can never buy the book they have                               uploaded. Buyer can never sell the book. Buyer can "BECOME A SELLER" by updating profile. Similarly, Seller can unsubscribe from the                                 selling service any point of time

- UPLOAD BOOK/DELETE/EDIT: A book can be uploaded with multiple Authors and Images. A Seller can upload multiple books. Books which are publishing in future will be                            listed on the metioned publish date not before that. Similar to upload, Books can be deleted or edited. Only Seller who uploaded the book                            can perform these actions. Any changes to the book will be reflected to the Book added in cart by a buyer.This feature is implemented                                using Amazon S3 bucket for storing uploaded book images

- FORGET PASSWORD: Clicking on FORGET PASSWORD will make RESET PASSWORD option available. The reset password link is shared with the user via Email. This feature is                    implemented using Function As A Service (FAAS) Lambda Function of AWS. Simple Notification Service (SNS) and Simple Email Service (SES) are                          integrated to complete the delivery of an email to User

## AWS INFRASTRUCTURE MANAGEMENT
- Used Terraform as a Infrastructure as Code to provision and manage cloud infrastructure

- Built Amazon Machine Image using Packer


Click on the image below to start demo of an Application

[![Watch the video](https://img.youtube.com/vi/e_YWE55_QaM/0.jpg)](https://youtu.be/e_YWE55_QaM)
