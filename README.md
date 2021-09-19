# EC601_Project1
**Individual project 1 for EC601**

*Research on the topic of 'Network security in IoT'*

*Author: Nuwapa Promchotichai (Prim)*

## Problem Statement
IoT (Internet of things) security refers to the techniques, strategies, and tools used to protect IoT devices (network-based devices) from becoming compromised. 

Ideally, all IoT devices should be well assessed of all the security risks and the infrastructure of the IoT devices should be secured accordingly against the dangers. However, the Internet of things is growing fast and there are more products being pushed out to the market. More and more people are buying IoT devices and integrating them into their home. 

As IoT devices are becoming more capable and cloud networks becoming more interconnected, there are more risks being imposed upon IoT devices. Without proper security for IoT, any connected devices can be vulnerable to hackers, thus putting the consumer’s personal data at risk.

It is important to reduce risk associated with IoT devices and explore several potential solutions to protect consumers against potential threats. There should be a comprehensive IoT device security standard and also rigorous procedures to test IoT devices against vulnerabilities. In addition, users should be warned about the threats and be well-informed on how to properly handle a situation where their personal data might be at risk.

## Applications
IoT security involves protecting connected devices. This can include being mindful of cybersecurity vulnerabilities as early as in the design phase of IoT devices and throughout each stage of development. It can also involve network security, API security etc. The general applications of the IoT security can include:
1. IoT device or applications updates
  * The data associated with IoT devices should always be protected and secured. Therefore, regular update of the IoT devices with security patches is crucial to make sure that the system is up to date against new threats.
2. Secure internet-based communication 
  * To make sure that the systems are not compromised, the communication must be secured if the device is connected to the cloud.
3. Authentication and authorization
  * Password protection should be required in the IoT application. IoT systems should require a strong password to prevent brute force attacks. Additionally, enforcing smart password management such as mandatory password changes, or random strong password generator can help improve IoT security.
4. Data integrity
  * All sensitive or confidential data must be encrypted during transmission and storage. 
  * There should be a strict access control policy for APIs to prevent Man in the Middle (MMITM), code injections, or distributed denial of service (DDos) assaults.
5. Actively monitor and Detect IoT devics
  * Notify users about updated software when one becomes available. Also notify users if the software they are running is outdated. 
  * Constantly scans and monitors for attack entries that may occur.

There are also more state of art research on IoT security including identifying IoT security patterns to help design secure IoT applications, intrusion detection, and methods for IDS setup in future IoT systems.

The applications of IoT security are important such that it will help protect consumers' data and push IoT technologies development and implementation forward. With a strong understanding of possible vulnerabilities and how to handle them, soon, we will be able to connect to any device and control every aspect of life. With COVID-19, we see a rising adoption of IoT. IoT devices are paving the way for a revolution, thus the security risks need to be addressed and solved so that the technology can be developed to its full potential.

## Literature Review

 IoT applications include both parts in the cloud as well as cyber-physical systems. IoT systems can be complex which comes along with higher security risks, thus, there are many approaches to handle the complexity and heterogeneity of the system. This report will focus on the state-of-art strategies of using blockchain-based authentication schemes for IoT.
 
IoT architecture consists of three different layers and there are different security challenges on these layers. The key technologies of IoT include sensors, embedded systems, nano-technology, and radio frequency identification (Srivastava, 5). Thus, to understand the IoT system and the risks associated with it, the underlying technologies at different levels of IoT architecture should be considered. 
Srivastava’s paper on “Future IoT-enabled threats and vulnerabilities: State of the art, challenges, and future prospects” discusses the three layers of IoT architecture and the underlying threats at each different layer. IoT security architecture layer includes: sensing layer, transport layer, and the application layer. Sensing layer refers to the layer at which the IoT system gets and processes data from different domains. If an unsecured sensor node joins the network, the network’s integrity, confidentiality, and availability can be compromised. Therefore, some of the security risks associated with the sensing layer include node capture, replay attack, timing attack, and eavesdropping. The transport layer in IoT helps connect entities so that they will be able to interact within a given network. The possible security threats associated with the transport layer include security at core network, access network, and local area network. These threats affect the data integrity of IoT systems. The application layer may include different services which directly relate to information gathered from sensors. At this layer, it is important to consider cloud security such as buffer overflow, software bugs, data access issues, user authentication issues, virus, Trojan horse, etc.

One of the approaches to cyber attacks in IoT include blockchain solutions. Blockchain has attracted attention in resolving several authentication-related issues of IoT authentication protocols (Srivastava, 8). By utilizing advanced encryption algorithms via blockchain techniques, the exploitation of Sybil attack can be obstructed. Blockchain-based methodologies also utilized Lagrange interpolation which helps alleviate vulnerabilities of chosen plain text message attack.

Some of the state-of-art security analysis techniques used by blockchain-based authentication schemes include Yin et al., Lin et al., and Li et al.
* Li et al. technique utilized the Lagrange interpolation mechanisms which can be used to bye-pass Sybil attack. 
* Yin et al. technique utilized the contributions of pre-image sample-able doorway techniques which can help preferred message attack to be unforgeable. 
* Lin et al. technique was designed based on the cryptographic algorithms (AES, MAC, ABS etc.) which satisfies the security requirements fine access control mechanisms and mutual authentication.

Even though there has been a high growth of IoT-based applications in the last few years, IoT still faces many challenges. Although blockchain-based technology can be used to help alleviate some of the IoT security risks, there are still some technology specific challenges with blockchain in IoT. Blockchain architecture is unsuitable for large-scale IoT networks, as the architecture has limited nodes in permissioned networks as well as limited throughputs. The garbage data generation of the blockchain technology also affects the overall performance of the system. Storage is also a big challenge as the nodes have to store ledger instead of any centralized server. In addition, there are compliance and legal issues that limit the adoption of blockchain technology from manufacturers and service providers. There should be defined regulatory rules so that adoption of blockchain technology with IoT can be done efficiently at a global scale.

## Open Source Research
There are several open source projects which touch upon the IoT security analysis. This section will focus on the open source framework for IoT layers security analysis. 

The first open source analysis framework is called **IoTSecFuzz (ISF)**. ISF is a framework for automatization of IoT layers security analysis. The ISF project is licensed under the MIT License. ISF’s goal is to combine comprehensive testing of IoT device security at all levels of implementation. The framework operates with tested devices at three levels: hardware (debugging interfaces), firmware (reverse engineering of the device’s OS), and communication (NRF24, Bluetooth, Wifi, ip-networking). ISF system is a flexible modular system in which users can add their own modules to be tested. Some of the modules available with current ISF framework includes, fast top-password protocol bruteforce, ubertooth, avr loader, ble_tool, cfe, etc. ISF has a console user interface in which the user can run tested devices with different modules. The framework is written by Ilya Shaposhnikov, Sergey Bliznyuk and Sofia Marakhovich. There has yet to be a contribution from other programmers aside from the three authors. The project's latest update was in 2018.

Another open source analysis framework for IoT security is called **EXPLIoT**. EXPLIoT is a framework for security testing IoT and IoT infrastructure. EXPLIoT provides a set of plugins (each plugin executes a specific test case) which can be extended to create new plugins. The test cases provide the basis of automation of security/regression testing for IoT products. The goal of EXPLIoT is to cover as many IoT protocols, hardware platforms, and products as possible. The plugins of EXPLIoT have a unique identifier (ID) and consist of three components: protocol it targets, product it targets, name of the plugin itself that describes its action. The framework is written by Aseen Jakhar and the latest update was in May 2021. 

## Duplicate the results
I tried to run IoTSecFuzz, however, I ran into a problem setting up modules for IoTSecFuzz. 
However, the IoTSecFuzz Github repository has given a comprehensive example on how the framework can be applied.

## Reference


I. R. Atoui, “The Importance of Security by Design for IoT Devices,” IIoT World, 25-Apr-2018. [Online]. Available: https://www.iiot-world.com/ics-security/cybersecurity/the-importance-of-security-by-design-for-iot-devices/. [Accessed: 17-September-2021].

II. F. H. Foomany, “IoT legislation device manufacturers need to know about,” SearchCompliance, 11-Aug-2021. [Online]. Available: https://searchcompliance.techtarget.com/post/IoT-legislation-device-manufacturers-need-to-know-about. [Accessed: 17-Sep-2021].

III. “How to Secure IoT Devices in the Enterprise,” Palo Alto Networks. [Online]. Available: https://www.paloaltonetworks.com/cyberpedia/how-to-secure-iot-devices-in-the-enterprise. [Accessed: 18-Sep-2021].

IV. “Internet of Things (IoT) security,” imperva, 29-Dec-2019. [Online]. Available: https://www.imperva.com/learn/application-security/iot-internet-of-things-security/. [Accessed: 18-Sep-2021].

V. cuelogic, “IoT Application Security Challenges and Solutions,” IoT For All, 01-Oct-2019. [Online]. Available: https://www.iotforall.com/iot-application-security. [Accessed: 18-Sep-2021].

VI. A. Jakhar, "expliot_framework / expliot," GitLab. [Online]. Available: https://gitlab.com/expliot_framework/expliot [Accessed: 18-September-2021].

VII. L. Li, J. Liu, L. Cheng, S. Qiu, W. Wang, X. Zhang, and Z. Zhang, “CreditCoin: A Privacy-Preserving Blockchain-Based Incentive Announcement Network for Communications of Smart Vehicles,” IEEE Transactions on Intelligent Transportation Systems, vol. 19, no. 7, pp. 2204–2220, 2018.

VIII. Q. Lin, H. Yan, Z. Huang, W. Chen, J. Shen, and Y. Tang, “An ID-Based Linearly Homomorphic Signature Scheme and Its Application in Blockchain,” IEEE Access, vol. 6, pp. 20632–20640, 2018.

Shaposhnikov, S. Bliznyuk, and S. Marakhovich, “Invuls / Iot projects / IOTSECFUZZ,” GitLab. [Online]. Available: https://gitlab.com/invuls/iot-projects/iotsecfuzz. [Accessed: 17-Sep-2021]. 

IX. S. Shea and I. Wigmore, “What is IoT Security?,” IoT Agenda, 06-Apr-2021. [Online]. Available: https://internetofthingsagenda.techtarget.com/definition/IoT-security-Internet-of-Things-security. [Accessed: 18-Sep-2021].

X. A. Srivastava, S. Gupta, M. Quamara, P. Chaudhary, and V. J. Aski, “Future IoT-enabled threats and vulnerabilities: State of the art, challenges, and future prospects,” International Journal of Communication Systems, vol. 33, no. 12, May 2020.

XI. W. Yin, Q. Wen, W. Li, H. Zhang, and Z. Jin, “An Anti-Quantum Transaction Authentication Approach in Blockchain,” IEEE Access, vol. 6, pp. 5393–5401, 2018.

