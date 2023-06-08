# Chapter: Cybersecurity Attack Frameworks

## 1 Kill Chain

Kill Chain is a model developed by Lockheed Martin that describes the stages by which a threat actor progresses a network intrusion. This framework consists of the following stages:

### 1.1 Reconnaissance

At this stage, the attacker determines what methods to use to complete the phases of the attack. Reconnaissance involves gathering information about the target, which can include activities such as port scanning, identifying the operating system, determining software versions, and identifying potential vulnerabilities. Tools often used for this stage include Nmap, Nessus, or Wireshark.

### 1.2 Weaponization

Here, the attacker couples payload code that will enable access with exploit code that will use a vulnerability to execute on the target system. This process may involve creating or modifying malware, hiding malware from detection systems, or creating a phishing email or website. Tools such as Metasploit, Veil-Evasion, or SET (Social-Engineer Toolkit) can be used here.

### 1.3 Delivery

In this phase, the attacker identifies a vector by which to transmit the weaponized code to the target environment. Delivery vectors can include emails, websites, USB drives, network port scanning, or man-in-the-middle attacks. For instance, spear phishing tools like GoPhish can be used for payload delivery.

### 1.4 Exploitation

At this stage, the weaponized code is executed on the target system. This can involve exploiting a vulnerability, forcing a user to perform an action (such as clicking on a link in a phishing email), or another mechanism that allows the code access to the system. Known tools like Metasploit, Exploit DB can be used to exploit vulnerabilities.

### 1.5 Installation

This mechanism enables the weaponized code to run a remote access tool and achieve persistence on the target system. This can involve activities such as changing system settings, adding registry entries, or creating new services that run at system startup. RAT (Remote Access Trojan) tools like njRAT, DarkComet, or Mimikatz are used to maintain access.

### 1.6 Command & Control (C2)

At this stage, the weaponized code establishes an outbound channel to a remote server that can then be used to control the remote access tool and possibly download additional tools to progress the attack. C2 servers may be directly controlled by the attacker, or may be part of a botnet network. Tools like Empire, Cobalt Strike, or Powershell are often used at this stage.

### 1.7 Actions on Objectives

At this stage, the attacker typically uses the access he has achieved to covertly collect information from target systems and transfer it to a remote system (data exfiltration) or achieve other goals and motives. This can involve data theft, sabotaging operations, spying, creating backdoors, or any other actions the attacker may want to undertake.

Kill chain analysis can be used to identify a defensive course-of-action matrix to counter the progress of an attack at each stage.

## 2 MITRE ATT&CK Framework

MITRE ATT&CK (Adversarial Tactics, Techniques & Common Knowledge) is a knowledge base maintained by the MITRE Corporation for listing and explaining specific adversary tactics, techniques, and common knowledge or procedures (attack.mitre.org).

The MITRE ATT&CK includes a wide range of tactics and techniques used by adversaries at different stages of an attack. For each tactic, the techniques are described in detail, with information about how they are used, how they can be detected, and how to counter them. The pre-ATT&CK tactics matrix aligns to the reconnaissance and weaponization phases of the kill chain.

## 3 Diamond Model of Intrusion Analysis

Diamond Model is a framework for analyzing cybersecurity incidents and intrusions by exploring the relationships between four core features: adversary, capability, infrastructure, and victim.

The adversary is the entity that conducts the attack. This can be a single hacker, a group of hackers, a criminal organization, or even a nation-state. Capability refers to the set of skills, knowledge, tools, and other resources that the adversary has at their disposal. Infrastructure refers to the means that the adversary uses to conduct the attack, such as servers, botnet networks, or phishing websites. The victim is the entity that is the target of the attack.

Analysis according to the Diamond model allows for a better understanding and characterization of an incident by understanding how these four aspects are interrelated and how each of them influences the course of the incident.