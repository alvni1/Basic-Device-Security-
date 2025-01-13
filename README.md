<h1>Basic Device Security</h1>



<h2>Description</h2>
This project consisted of configuring passwords on the command line interface (CLI) to prevent unauthorized users from making any changes on devices in the network, such as the router and the switch. Various password commands were used to create a simple plaintext password, create an encrypted password for stronger protection, and to encrypt the passwords when shown in the configuration. 

Cisco devices often serve as gateways or core components in a network. A breach in their security could expose the entire network to attacks, such as data theft, malware injection, or denial-of-service (DoS) attacks. Password protection on Cisco devices is vital to prevent unauthorized access, safeguard sensitive configurations, and protect against security breaches that could compromise the entire network. It helps maintain device integrity, mitigate internal threats, and comply with security regulations. By limiting access to critical information and enabling layered security measures, such as role-based access control and encryption, password protection ensures the reliability and security of network operations.

<h2>Languages and Utilities Used</h2>

- <b>Cisco Command Line Interface</b> 

<h2>Environments Used </h2>

- <b>Cisco Packet Tracer</b>

<h2>Things Learned/Troubleshooting</h2>
When trying to display the running configuration, there is different ways to type in the command depending on which mode you are in. For example, when in privileged EXEC mode the command would be do show running-config vs when in user EXEC mode the command would be show running-config. 

<h2>Program walk-through:</h2>

The service password-encryption command encrypts all plaintext passwords stored on a device, adding a basic layer of security to the device and making it so that passwords are not easily visible. It should not be solely relied on for strong security. Instead the enable secret command should be used as well. The enable secret command is used to set an encrypted password for privileged EXEC mode (also known as enable mode). Unlike the enable password command, which stores the password in plaintext or weak encryption, the enable secret command stores the password using a much stronger, one-way hash.

![Screenshot 2025-01-06 231141](https://github.com/user-attachments/assets/6ed858e3-b117-42f4-9d46-8e2959424179)

The do show running-config command shows that passwords currently on the Cisco device are encrypted and are not easily visible. 

![Screenshot ![Screenshot 2025-01-06 231141](https://github.com/user-attachments/assets/0d59ff03-e5f0-4f79-a945-ef5953fb4502)
2025-01-06 231309](https://github.com/user-attachments/assets/01c84ffe-4ad5-4259-9dd6-2c83fe9d2aa0)

