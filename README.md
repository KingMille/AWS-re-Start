Web App Integration with Amazon Aurora - AWS re/Start Project

Description

This project is a part of my AWS re/Start course, where I developed a web application integrated with an Amazon Aurora database. The project involved setting up an Amazon EC2 instance to host the web app, which allows users to input and retrieve data like names and addresses. The data is then stored in the Amazon Aurora database. 

Well-Architected Framework Pillars

During the project, several pillars of the AWS Well-Architected Framework were considered:

1. Reliability:
   - Utilized an Amazon Aurora cluster automatically managed by AWS, which includes two copies of the database. This setup ensures high availability and data redundancy in case of failures.
   - The cluster provides automatic failover capability, allowing the application to maintain uptime with minimal interruption if one instance becomes unavailable.

3. Security:  
   - Configured security groups to restrict traffic, allowing access only from my IP address, preventing unauthorized access and ensuring secure communication between the web app and the database.

4. Cost Optimization:  
   - Chose a burstable instance class for the Amazon Aurora database instead of a memory-optimized class, since the project requirements were not resource-intensive. This approach reduced costs while maintaining adequate performance.
   
Potential Upgrades Based on Well-Architected Framework
Here are some upgrades that could further improve the project, aligned with AWS Well-Architected Framework principles:

1. Reliability:  
   - Implement multi-AZ deployment for the Amazon Aurora cluster to ensure that data is replicated across multiple Availability Zones, increasing fault tolerance and availability.

2. Security Enhancements:  
   - Implement user permissions management within the EC2 instance and database, ensuring that only authorized users have access to modify configurations.
   - Use AWS Secrets Manager to store and manage database credentials securely, instead of hardcoding them in the application, ensuring enhanced security for sensitive information.
   
3. Enhanced Cost Optimization:  
   - Explore the use of EC2 Spot Instances for non-critical aspects of the web app, reducing hosting costs.
   - Migrate static web content to Amazon S3 with CloudFront for faster content delivery and reduced load on the EC2 instance, further optimizing costs.
