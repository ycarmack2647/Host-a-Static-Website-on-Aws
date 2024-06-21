# Hosting a Static Website on AWS

## Project Overview

This project demonstrates how to host a static HTML web application on AWS, leveraging various AWS services to ensure high availability, security, and scalability. The project setup includes configuring a VPC, deploying EC2 instances, and utilizing an Application Load Balancer among other components.

## Architecture Diagram

![Architecture Diagram]

## Deployment Steps

### 1. Configure a Virtual Private Cloud (VPC)
- Set up a VPC with both public and private subnets across two different availability zones to ensure high availability and fault tolerance.

### 2. Deploy an Internet Gateway
- Deploy an Internet Gateway to enable connectivity between VPC instances and the internet.

### 3. Establish Security Groups
- Create Security Groups to act as a network firewall, controlling traffic to and from the instances.

### 4. Utilize Availability Zones
- Leverage two Availability Zones to enhance system reliability and fault tolerance.

### 5. Utilize Public Subnets
- Use public subnets for infrastructure components like the NAT Gateway and Application Load Balancer.

### 6. Implement EC2 Instance Connect Endpoint
- Set up EC2 Instance Connect Endpoint for secure connections to assets within both public and private subnets.

### 7. Position Web Servers in Private Subnets
- Place web servers (EC2 instances) within private subnets for enhanced security.

### 8. Enable Internet Access via NAT Gateway
- Enable instances in both the private application and data subnets to access the internet via the NAT Gateway.

### 9. Host the Website on EC2 Instances
- Deploy the static website on EC2 instances.

### 10. Employ an Application Load Balancer
- Use an Application Load Balancer and a target group to distribute web traffic evenly to an Auto Scaling Group of EC2 instances across multiple availability zones.

### 11. Utilize an Auto Scaling Group
- Set up an Auto Scaling Group to automatically manage EC2 instances, ensuring website availability, scalability, fault tolerance, and elasticity.

### 12. Store Web Files on GitHub
- Store web files on GitHub for version control and collaboration.

### 13. Secure Application Communications
- Use AWS Certificate Manager to secure application communications.

### 14. Configure Simple Notification Service (SNS)
- Set up SNS to alert about activities within the Auto Scaling Group.

### 15. Register Domain and Set Up DNS
- Register the domain name and set up a DNS record using Route 53.

## Repository Contents

- **/scripts/**: Contains the deployment scripts.
- **/diagrams/**: Contains the architecture diagram.
- **README.md**: This file.

## Getting Started

1. **Clone the Repository:**
    ```bash
    git clone https://github.com/ycarmack2647/your-repo-name.git
    ```
2. **Navigate to the Project Directory:**
    ```bash
    cd your-repo-name
    ```
3. **Follow the Deployment Steps:**
    - Use the provided scripts and follow the deployment steps detailed above.

## Contributing

Feel free to submit issues and pull requests. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For any inquiries, please reach out to me via [LinkedIn](https://www.linkedin.com/in/yashon-carmack-43911b70/) or [GitHub](https://github.com/ycarmack2647).

---

Happy coding!

