# SOC-Fundamentals
All tasks are performed in LetsDefend

## Monitoring
- SIEM (Security Information and Event Management) is a security solution which has many features, but the two most valuable features for SOC Analyst are collect and filter data and supply alerts of supicious events. Some SIEM that I used to use are Splunk, Invicti, IBM QRadar.
- Here are alerts from Monitoring Channel
![image](https://github.com/buiduchoang24/SOC-Fundamentals/assets/166605385/3013f8fe-4655-4d70-ad17-abd4177c5113)
- From here, I can see many details about alert like IP source, IP destination, event time,...
![image](https://github.com/buiduchoang24/SOC-Fundamentals/assets/166605385/4a73e6f0-b9b7-4691-a0bf-52166cf3e507)

## Log Management
- Analyzing logs is a part in work of a SOC Analyst. The purposes of this process are to determine if there is any communication with a particular address and to view the details of that communication. For example, we have been attacked by a backdoor, we see it was executing and communicating from ```hacker.com```, so we can search through Log Management system to find information and details about ```hacker.com```.
- Here is the interface of Log Management
![image](https://github.com/buiduchoang24/SOC-Fundamentals/assets/166605385/566b83b4-9237-4730-b197-d8f13e394647)
- I can use search to filter events by their source IP, source port, destination IP, destination port
![image](https://github.com/buiduchoang24/SOC-Fundamentals/assets/166605385/b98f57e0-13a1-4e05-9af6-9a61e39463ff)

## EDR - Endpoint Detection and Response
- This is an integrated endpoint security solution that combines continuous, real-time monitoring and collection of endpoint data with rules-based automated response and analysis capabilities. The EDR that I used to use is LimaCharlie, I have written about it in my repo named SOC-Analyst. Another one is MetaDefender Endpoint I used at Opswat.
- Here is the interface in LetsDefend
![image](https://github.com/buiduchoang24/SOC-Fundamentals/assets/166605385/0a26e53a-66a6-4848-9506-293b020cc95e)
- In EDR, I can see many details about events like Event Time, Process ID, Command Line, Target Process Command Line, Browser History, Terminal History, Network Action,...
![image](https://github.com/buiduchoang24/SOC-Fundamentals/assets/166605385/8d22c098-2aa8-461d-83b3-f1ead048f502)
- Search and analyze information about malicious process executed on Terminal.
![image](https://github.com/buiduchoang24/SOC-Fundamentals/assets/166605385/38cd026b-0cc9-420e-b066-3ed13aed1aa0)

## SOAR - Security Orchestration Automation and Response
- SOAR stands for Security Orchestration Automation and Response. It enables security products and tools in an environment to work together, streamlining the tasks of SOC team members. For example, it will automatically search VirusTotal for the source IP of a SIEM alert, reducing the workload of the SOC analyst.

## Threat Intelligence
- This has feeds, which are data such as malware hashes, C2 (Command&Control) domain/IP addresses,... and provided by a third party.
- Here is an interface of Theat Intelligence Feed of LetsDefend.
![image](https://github.com/buiduchoang24/SOC-Fundamentals/assets/166605385/6f69518e-f9ca-4e23-af24-533ff9ee0e3a)
- I can filter malware by its hash and see where it came from
![image](https://github.com/buiduchoang24/SOC-Fundamentals/assets/166605385/65eb18c3-9a3e-450e-aad4-4a3ebadccdfe)

## Some common mistake that SOC analyst may have
- Over-reliance on VirusTotal Results: Sometimes, there are new malwares that have anti virus bypass techniques, so VirusTotal can't scan them.
- Do not analyze malware in Sandbox carefully
- Inadaquate log analysis







