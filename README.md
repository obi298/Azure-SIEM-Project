# Azure SIEM Project



# Introduction:


In the modern era of technology, companies are heavily relying on their IT infrastructure in order to do their everyday tasks. And of course in the world of technology, it is important that companies are up to date on their security. Cybersecurity threats and incidents are not unknown and nowadays, attackers are getting smarter and smarter to the point where adding firewalls isn’t enough to stop these malicious attacks. Companies use SIEM (Security Information and Event Management) tools to monitor suspicious events within the work environment. In today’s era, SIEM tools are in higher demand due to cybersecurity threats evolving day by day. These tools allow security professionals to perform real-time analysis of the IT infrastructure and monitor the overall health of machines within an organization.

#In this project, I created a honeypot and exposed it to the world so that attackers can discover it.  I collected log data from the VM by using a PowerShell Script and a Third-Party API and transferred that data back to Azure to create a map of the attacks from around the world. I then was able to analyze where the attacks were coming from and take note of the number of failed login attempts from different regions.

#The purpose of this project was to learn the basics of Azure SIEM tools and use them to track down malicious attackers from around the globe. I have documented all the steps I have taken in order to successfully complete this project.







# Creating Virtual Machine:

I created a virtual machine and chose Windows 10 as my image. I intentionally made this VM vulnerable so that it can be discoverable to the whole world. I used Windows 10 Pro as my Image. I also selected the region for my virtual machine. This virtual machine was used as a honeypot to attract attackers from all over the world. I used this VM to capture failed login events from attackers and collect global data.

![1](https://github.com/obi298/Azure-SIEM-Project/assets/90945162/72d5bfba-542e-480c-8307-f9046a647748)




# Configuring VM Security Rules:

I created a username and password for this VM and configured the port rules in order to make this virtual machine vulnerable to attackers.

![2](https://github.com/obi298/Azure-SIEM-Project/assets/90945162/b7649092-2d43-455b-b0a5-e7d72227cb43)



I added a new security group and configured the network settings to make the virtual machine vulnerable and discoverable to attackers.

![3](https://github.com/obi298/Azure-SIEM-Project/assets/90945162/2af7b607-c5cd-43ac-a0cc-ff04f3608f46)


![4](https://github.com/obi298/Azure-SIEM-Project/assets/90945162/9ce135bf-fa73-445e-a665-0dd08f91a63a)


I deleted the old inbound security rule and added a new one. The new rule allowed the virtual machine to be exposed to attackers. 


![5](https://github.com/obi298/Azure-SIEM-Project/assets/90945162/50a0788e-d3b6-474d-9e40-a526c051b8ed)


Here, I created a new log analytics workspace. The logs contained geographic data from the virtual machine and were used to create a data visualization of the attacks.

![6](https://github.com/obi298/Azure-SIEM-Project/assets/90945162/2f24f0ef-afd9-4ac9-a7dd-f832de90a293)


I then went to Microsoft Defender for Cloud So that I can select a subscription plan for cloud services management and servers.

![7](https://github.com/obi298/Azure-SIEM-Project/assets/90945162/40fd62a9-6434-4dba-a456-8085729c1a64)


![8](https://github.com/obi298/Azure-SIEM-Project/assets/90945162/7b57f00b-4bb1-41c8-896d-be097263cd8a)



![9](https://github.com/obi298/Azure-SIEM-Project/assets/90945162/38d0b709-fb87-4121-9306-a61f424f283e)


![10](https://github.com/obi298/Azure-SIEM-Project/assets/90945162/1f5044c1-e262-46d6-817d-d014f1b4fb06)

















