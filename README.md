# Identifying MS17-010 EternalBlue Vulnerability Using Metasploit

## Background

Metasploit is a versatile penetration testing and security auditing platform that allows penetration testers to identify vulnerabilities in systems and assess their security posture. The framework consists of various modules that can be combined to perform different tasks, including identifying and exploiting vulnerabilities.

The MS17-010 EternalBlue vulnerability is a critical remote code execution flaw that affects the Windows Server Message Block (SMB) protocol. This vulnerability can be exploited to execute arbitrary code on the target system, leading to potential compromise and unauthorized access.

## Exercise Overview

In this exercise, I used Metasploit to identify a machine vulnerable to the MS17-010 EternalBlue exploit using an auxiliary module. The objective was to demonstrate how to use Metasploit's auxiliary modules to identify vulnerable machines and understand Proof of Concept (PoC) techniques for responsible penetration testing.

## Learning Objectives

- Utilize Metasploit's auxiliary modules to identify vulnerable machines.
- Understand the importance of PoC techniques in responsible penetration testing.
- Conduct penetration tests ethically and effectively.

## Importance of Proof of Concept

Penetration testing should be conducted responsibly and with care. Instead of running full exploits that may cause damage or disruption in a production environment, using PoC techniques allows penetration testers to demonstrate vulnerabilities without causing harm. PoC provides valuable evidence to clients about existing vulnerabilities, aiding in informed decision-making for improving security.

## Steps Taken

1. **Launch a Vulnerable Machine**: A virtual machine running a vulnerable version of Windows (e.g., Windows XP or Windows 7) with the MS17-010 vulnerability was launched.
   
2. **Metasploit Console**: Within the Metasploit console, the auxiliary module `scanner/smb/smb_ms17_010` was used to scan the target machine for the MS17-010 vulnerability.

3. **Scan Execution**: The auxiliary module was configured with the target machine's IP address and executed to detect the vulnerability.

4. **Validation**: The output from the "MS17-010 SMB RCE Detection" auxiliary module indicated whether the host was likely vulnerable to MS17-010.

## Results

The Metasploit scan successfully identified the target machine as likely vulnerable to the MS17-010 EternalBlue exploit. This demonstrated the effectiveness of using Metasploit's auxiliary modules for vulnerability identification.

## Conclusion

The exercise showcased the importance of responsible penetration testing through PoC techniques. By identifying vulnerabilities without causing harm, penetration testers can provide valuable insights to clients, helping them make informed decisions to improve their security posture. The use of Metasploit's auxiliary modules proved to be an effective method for vulnerability assessment in this exercise.

