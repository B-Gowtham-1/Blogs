---
title: "Day 4: The Cloud, Virtual Machines & Why Everything Is Just Someone Else’s Computer ☁️😂"
seoTitle: "Understanding Virtual Machines and Ownership"
seoDescription: "Cloud computing uses virtual machines on providers' servers, offering benefits but essentially relies on someone else's computer"
datePublished: Sat Mar 01 2025 06:02:46 GMT+0000 (Coordinated Universal Time)
cuid: cm7pspmsl000107l85f4thqqp
slug: day-4-the-cloud-virtual-machines-and-why-everything-is-just-someone-elses-computer
tags: aws, azure, devops, gcp

---

So today, I finally understood what **Cloud Providers** are and how **Virtual Machines (VMs)** work. And guess what? It turns out **"the cloud" is just someone else’s computer**—but fancier, more scalable, and way more expensive if you forget to turn things off. Let’s break this down **like I’m explaining to my past confused self.**

---

## **What Even Is Cloud Computing?** 🤔

Imagine you want to run an application—maybe a website, an AI model, or a game server. Normally, you’d need:  
🖥 **A powerful computer** (which costs money)  
⚡ **Electricity & maintenance** (also money)  
🔒 **Security** (firewalls, backups, disaster recovery… headache!)

Now, let’s say you don’t want to deal with all that. Instead, you **rent** computing power, storage, and networking from big tech companies that own massive **data centers**. That’s **Cloud Computing** in a nutshell.

### **Why Is It Called "Cloud" Though?**

It’s just a marketing trick! There's **no actual cloud.** It’s **a bunch of computers in a data center** somewhere in the world. But "cloud" sounds cooler than "someone else's server farm."

---

## **Meet the Big Bosses of the Cloud** ☁️💰

There are many cloud providers, but three **own the game**:

### 1️⃣ **Amazon Web Services (AWS) – The King of the Cloud 👑**

* The **biggest** and most widely used cloud platform.
    
* Used by Netflix, Airbnb, NASA—literally half the internet.
    
* Offers 200+ services but has **a pricing model so confusing that you’ll cry.**
    

### 2️⃣ **Microsoft Azure – The Corporate Favorite 💼**

* If your company loves Windows, they probably use Azure.
    
* Integrates well with Microsoft products (Office 365, Teams, etc.).
    
* Used by big enterprises and governments.
    

### 3️⃣ **Google Cloud Platform (GCP) – The Smart Nerd 🤓**

* Built for AI, machine learning, and big data.
    
* Used by companies like Spotify, Snapchat, and YouTube.
    
* Great at analytics but **not as popular as AWS and Azure.**
    

### **Other Cloud Providers**

There are others too: **IBM Cloud, Oracle Cloud, Alibaba Cloud, Linode, DigitalOcean**—but let’s be real, AWS, Azure, and GCP run the show.

---

## **Types of Cloud Services** ☁️💡

Cloud providers **don’t just rent out computers**. They offer different types of services:

### **1️⃣ Infrastructure as a Service (IaaS) – "Rent a Computer" 🖥**

* You get **virtual machines, storage, and networking.**
    
* You install and manage your software.
    
* Example: AWS EC2, Azure Virtual Machines, Google Compute Engine.
    

### **2️⃣ Platform as a Service (PaaS) – "Rent a Managed Server" 🚀**

* You get a **pre-configured environment** (database, runtime, etc.).
    
* No need to worry about OS updates or security patches.
    
* Example: AWS Elastic Beanstalk, Google App Engine, Azure App Service.
    

### **3️⃣ Software as a Service (SaaS) – "Rent a Ready-Made App" 📱**

* Fully managed apps like **Google Drive, Gmail, and Dropbox.**
    
* You just log in and use them.
    

---

## **Virtual Machines (VMs): The Illusion of Many Computers** 💻✨

Now, let’s talk about **Virtual Machines (VMs).**

A **VM is a "computer inside a computer."** Imagine installing **Windows inside your Linux machine**—yep, that’s a VM. It **tricks software** into thinking it’s running on a real machine, but it’s actually just a **software-based simulation** of one.

### **How Virtual Machines Work (In Simple Terms)**

Think of your computer as a **hotel**. 🏨 Inside the hotel, there are **rooms** (VMs). Each room has:  
🛏 **Its own furniture (OS, applications)**  
🔑 **A separate key (security & user permissions)**  
💡 **Independent utilities (RAM, CPU, disk space)**

Even though they share the **same hotel (hardware),** each room **thinks it’s a separate building.**

### **Why Use Virtual Machines?**

✅ **Run multiple OS on the same machine** (Windows + Linux together)  
✅ **Isolated environments** (so viruses in one VM don’t kill your main OS)  
✅ **Cloud computing** (AWS, Azure, GCP use VMs to provide cloud services)

---

## **Cloud vs Virtual Machines: What’s the Difference?**

| Feature | Cloud Computing ☁️ | Virtual Machines 💻 |
| --- | --- | --- |
| Where It Runs | In someone else’s data center | On your computer or the cloud |
| Cost | **Pay-as-you-go** (can be expensive!) | **Free** if local, but needs hardware |
| Maintenance | Cloud provider takes care of it | You manage it yourself |
| Scalability | Scale up/down instantly | Limited by your PC's hardware |

### **Cloud + Virtual Machines = Ultimate Power**

Most cloud services **use Virtual Machines** behind the scenes. When you rent a server from AWS or Azure, you're **actually renting a VM running in their data center.**

---

## **Do I Need a Cloud or a VM?** 🤔

* **If you want to run a personal project on your PC** → Use a **Virtual Machine.**
    
* **If you want to build a scalable web app** → Use **Cloud Computing.**
    
* **If you have unlimited money** → Rent both and flex on your friends.
    

---

## **Final Thoughts** 🎯

Today, I learned that:  
☁️ **Cloud computing is just renting powerful computers from rich tech companies.**  
💻 **Virtual machines let you run multiple "fake computers" inside a real one.**  
💸 **Both can burn your wallet if you forget to turn things off.**

Cloud is the future, but **knowing how Virtual Machines work is still important.** Because at the end of the day, **everything is just someone else’s computer.** 😂

And that’s **Day 4 of DevOps**—Cloud Computing & Virtual Machines! 🚀

---

## **Next Steps**

Tomorrow, I might go deeper into **Docker, Kubernetes, or serverless computing**. But first, let me go and **double-check my AWS bill before I go broke.** 😭💸