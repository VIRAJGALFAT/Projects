---

Built an isolated **virtual** **penetration** **testing** **lab** using **VirtualBox**, simulating real-world attack and defense scenarios using **Kali** **Linux** and vulnerable machines (**Metasploitable**, **DVWA**). Configured internal networks, firewalls, and tested exploits using tools like **Nmap**, **Metasploit**, and **Burp Suite**.

---

### **Project Setup**

This guide will teach you how to set up your own private lab. To do this, we’ll need three things:

- Virtualization software
- Attacking Machine
- Target Machine

Virtualization software allows one physical computer to run multiple virtual machines (VMs). A virtual machine functions like a separate computer, complete with its own operating system.

VirtualBox is a popular virtualization software. VMware is another alternative.

To practice hacking, you need two machines — an attacking machine and a target machine.

The downloads required for this setup are quite large.

- [Download VirtualBox](https://www.virtualbox.org/wiki/Downloads) (download the extension pack as well)
- [Download Kali](https://www.kali.org/get-kali/#kali-virtual-machines) (64-bit Virtualbox image or .iso file)
- [Download Mr Robot vulnerable machine](https://www.vulnhub.com/entry/mr-robot-1,151/)

---

### **How to Install Kali Linux**

Now, let’s install the Kali Linux attacking machine. Then click the green “Add” icon on the VirtualBox interface and point to the .iso file.

![image.png](attachment:834eacde-629f-43d3-be63-51b09f332639:image.png)

All the default settings will be applied, and you should have the attacking machine installed.

### **How to Install a Target VM**

Now let’s install the target. Double-click on the downloaded `mrRobot.ova` file. Use the default settings and click “Finish”.

![image.png](attachment:a5622ebb-eccc-44c9-b63d-415c4994ddca:image.png)

### **Update Networking Settings**

There are many ways to set up a network in VirtualBox. But in this case, we want to isolate our lab from the public internet. The best way to do this is to set up a host-only network.

In a host-only network, the VMs can communicate with each other but not with the public internet. Let’s set it up.

In the VirtualBox interface, click on “Tools” and click “Host-only Networks”. Then click “Create”. It will automatically create a host-only network with an IP range.

![image.png](attachment:d7791098-27b1-4e67-a6ca-73f18c7acae7:image.png)

We are ready to boot the machines.

![image.png](attachment:a72458ac-2518-4463-a11c-707f9fd70045:image.png)

 Kali Linux UI is shown below.

![image.png](attachment:f9f6e40a-a188-4a74-8229-c5cf56aa0865:image.png)

 Mr.Robot box UI is shown below.

![image.png](attachment:f1434eba-209f-417e-8df0-02719ea43645:image.png)

Now let’s find the IP addresses of these machines.

![image.png](attachment:47d4c19f-4768-4373-a8ab-02844060327b:image.png)

Attacker machine IP and MAC address.

![image.png](attachment:13d36efa-dbe6-4811-afab-017934ad8193:image.png)

Host machine IP and MAC address.

![image.png](attachment:d3a57798-bf0c-40c0-9596-95e0852c455c:image.png)

A quick comparison of the IP and MAC addresses of both machines.

### **Conclusion**

We successfully set up your hacking lab using VirtualBox. This lab provides you with the flexibility to practice ethical hacking in a controlled and isolated environment.

---
