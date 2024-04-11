# 2023-24-BE47
**Group No. 47**
**BE Major Project - Drivido : Blockchain-Powered Vehicle Network**

**Group Members:**

1. Sakshi Patil  D17C-61
2. Shalini Mirani D17C-35
3. Paraskumar Panchal D17C-41
4. Sanjana Bhojwani D17C-11

# Abstract of the project 
Indian Regional Transport Office (RTO) is a government agency responsible for managing various aspects of motor vehicle registration, driver licensing, and regulation of road transport within a specific region or jurisdiction. RTOs play a crucial role in ensuring the safe and efficient operation of road transport systems, maintaining traffic regulations, and collecting revenue for the government through vehicle registration and licensing fees. The current RTO system has been facing some issues such as inconsistency and integration, even though efforts have been made to address these problems like implementing technology upgrades, streamlining processes. Despite these , the system still faces problems like long waiting times for services and irregular results.
The proposed model which is built using IoT and blockchain technology intends to track and record information about vehicles for traffic monitoring and ticket creation. The process consists of the following steps: (1) collecting data from various sensors on vehicles and signal cameras for traffic violations such as speeding or running red lights, (2) creating a blockchain for vehicle information and traffic rule violations, (3) using sensor data and camera footage to issue tickets with video proof for users to verify or contest, (4) queries on issued tickets by the accused are managed in a separate Complaint tracking Blockchain and ticket's status is updated.

# How it works
1. The RTO side (i.e. the client side) will issue a challan as per the violations detected through the sensors. The issued ticket will first get connected to the peer nodes and reach the endorser peers that checks the fabric certificate authority of the requesting member and other details that are needed to authenticate the transaction.
2. Then it executes the chain code and returns a response. This response indicates the approval or rejection of the following transaction. The response is carried out to the client.
3. After getting the approval from the endorsed peers the transactions are then sent to the ordering nodes by the client side application. The received transactions are then added to the specific blocks of the different organisa- tions(in our case the Vehicle Owner side) .
4. The received transactions are validated with the help of the committing nodes.
5. After receiving the transactions and getting validated through the committing nodes, the transaction is then added to the ledger. Hence completing the transaction.


# Technology and Tools utilized
1. Blockchain Technology: Blockchain is the foundational technology used to securely store and manage data related to vehicle information and traffic violations. It ensures data immutability, transparency, and security, making it suitable for creating an unchangeable record of the RTO system's data.
2. IoT Devices and Sensors: Internet of Things (IoT) devices and sensors are utilized to collect real-time data from vehicles, such as location, speed, and other relevant information. These devices enable the tracking of vehicle movements and help in identifying traffic violations like overspeeding.
3. Smart Contract Platforms: Smart contracts, built on blockchain platforms like Ethereum or Hyperledger, are used for automating the ticket generation process. These self-executing contracts automatically generate tickets when specific conditions (e.g., traffic violations) are met, ensuring efficiency and accuracy.
4. Complaint Tracking Blockchain: A dedicated blockchain is introduced for tracking and handling inquiries and updates on ticket status. This blockchain ensures transparency and fairness throughout the process, allowing users to contest issued tickets and monitor the progress of their complaints.

# Built Using
1. HyperLedger Fabric
2. NodeJs
3. Hyperledger Fabric SDK for Node.js
4. Chaincode (Smart Contracts)
5. Javascript
