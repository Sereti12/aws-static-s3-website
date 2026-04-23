<p align=center><strong>Project Overview </strong></p>
This project demonstrates hands-on experience in deploying a fully functional static website using Amazon S3 bucket. The main objective is to implement a cost-effective, highly available, serverless hosting solution while using appropriate access control and configuration best practices. 
The implementation covers bucket provisioning, controlled public access, bucket policy configuration, static web hosting, and content deployment. 
<p align=center><strong>Architecture</strong></p>
<p>This solution utilizes a simple serverless architecture:</p>
<ul>
	<li>A client (web-browser) sends a request to the bucket website endpoint</li>
	<li>The bucket retrieves and serves the static content (HTML, CSS, JavaScript)</li>
  <li>Access is controlled via a bucket policy granting public read-only access</li>
</ul>
  ![Architecture](https://github.com/Sereti12/aws-static-s3-website/blob/700709bf618638ada9664cf050af84c5adbd2557/Architecture.jpg?raw=true)
