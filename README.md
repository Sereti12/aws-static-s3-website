## **Project Overview**

This project demonstrates hands-on experience in deploying a fully functional static website using an Amazon S3 bucket. The main objective is to implement a cost-effective, highly available, serverless hosting solution while applying appropriate access control and configuration best practices.

The implementation covers bucket provisioning, controlled public access, bucket policy configuration, static web hosting, and content deployment.

---

## **Architecture**

This solution utilizes a simple serverless architecture:

* A client (web browser) sends a request to the S3 website endpoint  
* The bucket retrieves and serves static content (HTML, CSS, JavaScript)  
*  Access is controlled via a bucket policy granting public read-only access  

<p align="center">
  <img src="Architecture.jpg" alt="Architecture Diagram" width="1000"/>
</p>

*Figure 1: Architecture of static website hosting using Amazon S3. This diagram demonstrates how client requests are served directly from the S3 endpoint.*
