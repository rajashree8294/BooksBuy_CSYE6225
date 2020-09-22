# BooksBuy_CSYE6225
BooksBuy is a Cloud-Native Application built using Angular 9, NodeJS, MySQL, Sequelize.Deployed on Amazon Web Services using EC2, S3, Lambda Function, Route53, SNS, SES, CloudDeploy, CodeWatch services. Implemented Continuous Integration and Continuous Deployment (CI/CD) using CircleCI workflows.Implemented Infrastructure as a Code using Terraform. Session management using JWT Token at the server side and Session Storage on the Front End side of an application.

Functional Features:
- SIGN UP/LOGIN : Users can create account in the BooksBuy. Users credentials are secured using BCrypt password hashing scheme with Salt

- ROLE BASED PROFILE VIEW : A user can be a BUYER or BUYER & SELLER. According to the role, users can see their dashboard. Seller can never buy the book they have                               uploaded. Buyer can never sell the book. Buyer can "BECOME A SELLER" by updating profile. Similarly, Seller can unsubscribe from the                                 selling service any point of time

- UPLOAD BOOK/DELETE/EDIT: A book can be uploaded with multiple Authors and Images. A Seller can upload multiple books. Books which are publishing in future will be                            listed on the metioned publish date not before that. Similar to upload, Books can be deleted or edited. Only Seller who uploaded the book                            can perform these actions. Any changes to the book will be reflected to the Book added in cart by a buyer.This feature is implemented                                using Amazon S3 bucket for storing uploaded book images

- FORGET PASSWORD: Clicking on FORGET PASSWORD will make RESET PASSWORD option available. The reset password link is shared with the user via Email. This feature is                    implemented using Function As A Service (FAAS) Lambda Function of AWS. Simple Notification Service (SNS) and Simple Email Service (SES) are                          integrated to complete the delivery of an email to User

# Infrastructure Management on AWS
- Used Terraform as a Infrastructure as Code to provision and manage cloud infrastructure

- Built Amazon Machine Image using Packer


Click on the image below for the demo of an Application

[![Watch the video](https://img.youtube.com/vi/e_YWE55_QaM/0.jpg)](https://youtu.be/e_YWE55_QaM)
