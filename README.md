Project 2: Basic Web Hosting
Step 1: Create AWS Account and Explore Free Tier
If you don't have an AWS account, sign up for one at AWS Console.
Explore the AWS Free Tier to understand the services available without incurring charges.
Step 2: Launch First EC2 Instance
Navigate to the EC2 service in the AWS Management Console.
Launch an EC2 instance following the wizard. Choose an Amazon Machine Image (AMI), instance type, and configure instance details.
Create or select a key pair for SSH access.
Review and launch the instance.
Step 3: Deploy Static Website using S3
Go to the S3 service in the AWS Management Console.
Create a new S3 bucket with a unique name.
Upload your static website files (HTML, CSS, JavaScript, images) to the S3 bucket.
Enable static website hosting for the S3 bucket and configure the index and error documents.
Step 4: Implement SSL/TLS using ACM
Go to the ACM service in the AWS Management Console.
Request a new SSL/TLS certificate for your domain (or use the one you own).
Choose a validation method (DNS validation is common) and complete the validation process.
Once the certificate is issued, associate it with your S3 bucket. If using a custom domain, you can also associate it with a CloudFront distribution.
Step 5: Test the Static Website
Access your static website using the S3 bucket URL or custom domain.
Ensure that the website loads correctly over HTTPS.
Check the SSL/TLS certificate details to confirm it's valid.
Additional Tips:
Custom Domain:

If you have a custom domain, configure it using Route 53 and update DNS settings.
CloudFront (Optional):

For enhanced performance and security, consider using CloudFront as a CDN. Configure it to distribute content from your S3 bucket.
Permissions:

Adjust S3 bucket permissions to allow public access for hosting.
Monitoring:

Set up CloudWatch Alarms to monitor the S3 bucket and website performance.
Documentation:

Document the steps taken, configurations made, and any issues faced during the project.
