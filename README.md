# Virtual Private Cloud (VPC) Simulation - Summary

### Steps Overview

1️⃣ **Initialize Environment / Login**
- Start by logging into your cloud console or preparing your local environment (Docker in this case).  
- Ensure Docker is installed and running, ready to simulate the VPC setup.  

2️⃣ **Make the Script Executable**
- The script is made executable so it can run on the system.

3️⃣ **Run the Script**
- Executing the script performs all steps automatically:  
  - Creates the main VPC (`myvpc`)  
  - Creates a public subnet (`public-subnet`) and a private subnet (`private-subnet`)  
  - Launches sample containers in each subnet to simulate resource deployment  
  - Tests connectivity to demonstrate public internet access and private isolation  
  - Optionally cleans up all containers and networks  

---

### Subnet Summary

| Network         | CIDR          | Internet Access |
|-----------------|---------------|----------------|
| myvpc           | 10.50.0.0/16  | N/A            |
| public-subnet   | 10.50.1.0/24  | ✅             |
| private-subnet  | 10.50.2.0/24  | ❌             |

---

### Outcome
- Successfully simulated a **Virtual Private Cloud** locally using Docker.  
- Demonstrated **public and private subnet separation**.  
- Showed **controlled internet access** for public resources while keeping private resources isolated.  
- Provides a **foundational understanding of cloud networking concepts** without requiring a cloud account.  

