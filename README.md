# **Project Overview**

This project demonstrates hands-on experience in deploying a fully functional static website using an Amazon S3 bucket. The main objective is to implement a cost-effective, highly available, serverless hosting solution while applying appropriate access control and configuration best practices.

The implementation covers bucket provisioning, controlled public access, bucket policy configuration, static web hosting, and content deployment.

---

# **Architecture**

This solution utilizes a simple serverless architecture:

* A client (web browser) sends a request to the S3 website endpoint  
* The bucket retrieves and serves static content (HTML, CSS, JavaScript)  
*  Access is controlled via a bucket policy granting public read-only access

<p align="center">
  <img src="Architecture.jpg" alt="Architecture Diagram" width="1000"/>
</p>

***Figure 1:*** *Architecture of static website hosting using Amazon S3. This diagram demonstrates how client requests are served directly from the S3 endpoint.*

# **Prerequisites**

Before implementing this solution, the following requirements should be met:

*	An active AWS account with access to the AWS management console. 
*	Basic familiarity with cloud concepts and object storage. 
*	Permissions that allow for the creation and configuration of bucket resources. 
*	Static website files ready for deployment (e.g., index.html, CSS, JavaScript assets).
  
# **Implementation**

* A bucket was provisioned with the following configuration:
*	Bucket type set to General Purpose
* A globally unique bucket name is assigned. 
* Access Control Lists (ACLs) were disabled to ensure centralized access management via the bucket policies.
  
The above-mentioned configurations align with AWS best practices for simplified and secure permission control. 

<p align="center">
  <img src="Bucket settings.png" alt="Bucket Settings Diagram" width="1000"/>
</p>

***Figure 2:*** *S3 bucket configuration with ACLs disabled. Shows the bucket setup with modern access control configurations applied.*

# **Public Access Configuration**

Public access settings were adjusted to support static website hosting:
* Block Public Access is disabled. 
* Access is restricted using a bucket policy granting read-only permissions. 
This is important as it ensures that access is enabled, while limiting exposure to only necessary actions.

<p align="center">
  <img src="Bucket settings.png" alt="Bucket Settings Diagram" width="1000"/>
</p>

