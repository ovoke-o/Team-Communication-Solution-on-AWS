## Scenario: Solving the Team communication and instant messaging problem
<h4>Course: Cloud Computing on AWS</h4>

<p>Implemented a team communication solution using Mattermost and AWS. This is a scalable solution that can be hosted on a public cloud, with its servers, storage etc. completely managed and controlled by an IT team in accordance with a company’s governance and security requirements.</p>

---

## 🧰 Architecture diagram
<p align="center">
  <!-- Replace with your own GIF or image -->
  <img src="img/img-1.jpg" alt="Java Selenium animation" width="900">
</p>

## 🧰 Architecture Implementation
<ul>
  <li>
    <p>Implement 2 different subnets (one public and the other private) in a custom VP</p>
  </li>
  <li>
    <p>Install and configure MySQL on an Amazon Linux 2 instance on the private subnet using the instructions provided. (Hint: Use a bastion host and a NAT gateway)</p>
  </li>
  <li>
    <p>Install and configure Mattermost on an Amazon Linux 2 instance on the public subnet using the provided instructions.</p>
  </li>
   <li>
    <p>Configure the security groups to allow the ports as shown in the architecture.</p>
  </li>
  <li>
    <p> Test the installation by accessing the IP of the public instance in a browser via the port 8065.</p>
  </li>
</ul>

---

## 🧰Step 1 (a): Creation of VPC
<ul>
  <li>
    <p>Navigate to VPC using the Services button at the top of the screen</p>
  </li>
  <li>
    <p>Select "Your VPCs" on the left side of the screen</p>
  </li>
  <li>
    <p>Click on "Create VPC".</p>
  </li>
   <li>
    <p>Enter the following fields:
            - Name: Project 1 VPC</li>
            - IPv4 CIDR Block: 10.0.0.0/16
            -  The rest of the options can be ignored.</p>
  </li>
  <li>
    <p> Select "Create VPC".</p>
  </li>
   <li>
    <p> Select the VPC and click on Actions->Edit DNS hostnames.</p>
  </li>
  <li>
    <p> Enable DNS hostnames and click on Save.</p>
  </li>

  <p align="center">
  <!-- Replace with your own GIF or image -->
     <img src="img/img-2.png" alt="Java Selenium animation" width="900">
     <img src="img/img-3.png" alt="Java Selenium animation" width="900">
     <img src="img/img-4.png" alt="Java Selenium animation" width="900">
</p>
</ul>

## 🧰Step 1 (b): Creation of Public Subnet
<ul>
  <li>
    <p>Navigate to VPC -> Subnets</p>
  </li>
  <li>
    <p>Click on "Create Subnet"</p>
  </li>
   <li>
    <p>Enter the following fields:
            - Name: Public Subnet</li>
            - VPC: Select the Project 1 VPC</li>  
            - IPv4 CIDR Block: 10.0.1.0/24
            -  The rest of the options can be ignored.</p>
  </li>
  <li>
    <p> Click on "Create".</p>
  </li>
   <li>
    <p> Once the subnet has been created, select the subnet, and click on Actions->Modify Auto-assign IP settings.</p>
  </li>
  <li>
    <p> Enable the option "Auto assign IPv4" and select Save.</p>
  </li>

  <p align="center">
  <!-- Replace with your own GIF or image -->
     <img src="img/sub-1.png" alt="Java Selenium animation" width="900">
     <img src="img/sub-2.png" alt="Java Selenium animation" width="900">
<!--      <img src="img/img-4.png" alt="Java Selenium animation" width="900"> -->
</p>
</ul>

### 🛠️ Skills & Tools Covered
<p>
  <a href="https://aws.amazon.com/" target="_blank" rel="noreferrer">
    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/amazonwebservices/amazonwebservices-original-wordmark.svg" alt="aws" width="40" height="40"/>
  </a>
   <a href="https://aws.amazon.com/" target="_blank" rel="noreferrer">
    <img src="img/EC2.png" alt="aws" width="40" height="40"/>
  </a>
  <a href="https://aws.amazon.com/" target="_blank" rel="noreferrer">
    <img src="img/Virtual Private Cloud.png" alt="aws" width="40" height="40"/>
  </a>
   <a href="https://aws.amazon.com/" target="_blank" rel="noreferrer">
    <img src="img/Security Hub.png" alt="aws" width="40" height="40"/>
  </a>
   <a href="https://aws.amazon.com/" target="_blank" rel="noreferrer">
    <img src="img/Transit Gateway.png" alt="aws" width="40" height="40"/>
  </a>
   <a href="https://aws.amazon.com/" target="_blank" rel="noreferrer">
    <img src="img/RDS.png" alt="aws" width="40" height="40"/>
  </a>
  <a href="https://aws.amazon.com/" target="_blank" rel="noreferrer">
    <img src="img/Network Firewall.png" alt="aws" width="40" height="40"/>
  </a>
</p>



