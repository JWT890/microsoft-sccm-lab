# microsoft-sccm-lab
This guide provides a comprehensive, step-by-step walkthrough for building a fully functional Microsoft Endpoint Configuration Manager (SCCM/MECM) home lab using VirtualBox. Perfect for IT professionals preparing for certifications, learning SCCM administration, or testing deployment scenarios in a safe environment. The lab consists of three virtual machines: a Windows Server 2022 Domain Controller with DNS and DHCP, a Windows Server 2022 SCCM Primary Site Server with SQL Server 2019, and a Windows 10/11 client for testing deployments. All components are configured to work together in an isolated network environment, allowing you to practice application deployment, operating system deployment, software updates, compliance settings, and reporting without affecting production systems. The entire setup requires approximately 8-10 hours to complete and assumes basic knowledge of Windows Server, Active Directory, and virtualization concepts.  

Windows 2022 Server download: https://www.microsoft.com/en-us/evalcenter/download-windows-server-2022  
Windows 10/11 Enterprise: https://www.microsoft.com/en-us/evalcenter/evaluate-windows-11-enterprise  
SQL Server Developer Edition download: https://go.microsoft.com/fwlink/?linkid=866662  
Microsoft Endpoint Configuration Manager Current Branch (SCCM): https://info.microsoft.com/ww-landing-microsoft-endpoint-configuration-manager.html?culture=en-us&country=us  
Windows Assessment and Deployment Kit ADK: https://learn.microsoft.com/en-us/windows-hardware/get-started/adk-install  

First go and setup the NAT Network that will be used:  
SCCM Lab: 192.168.10.0/24  

Setup:  
VM1: Domain Controller  
Memory: 4096 MB  
Space: 60 GB  
Network: NAT Network on Adapter 1  
Processer: 2 CPUs  
Version: Windows 2022

VM2: SCCM  
Processer: 4 CPUs  
Network: NAT Network on Adapter 1  
Memory: 12288 MB  
Space: 150 GB  

VM3: Client  
Memory: 4096 MB  
Network: NAT Network on Adapter 1  
Space: 60 GB  

