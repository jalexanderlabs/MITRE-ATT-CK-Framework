This Write-up is to learn about the MITRE organization and the different areas they research. These areas include the ATT&CK framework, CAR Knowledge Base, ENGAGE, D3FEND and AEP.

First off, what is MITRE exactly? 
MITRE is a non-profit organization that provides guidance and research on advanced technology, this also includes security, whichn is what I will be focusing on. 

Basic Terms to Note:

APT(Advanced Persistent Threat): This is a team/group or even a country that engage in long-term attacks against other organizations and/or countries.

TTP(Tactics, Technics, and procedures): TTP is an acronym that gives a basic outline of what a milicious actor, or adversary will perform in order to reach their goal.
Tactic: This is the adversaries goal or obvjective.
Technique: This is how the adversary achieves the objective.
Procedure: This is how the technique is executed. 

ATT&CK Framework

What is the ATT&CK Framework exactly?

This framework is essentially a giant database of adversary tactics and techniques. This heavily includes the before-mentioned APTs and their TTPs that they implement. This tool is useful for individuals who work in a red team environment, but I believe it is quintensential to security teams who defend their organization's network. 

Within the MITRE ATT&CK official website, there is the ATT&CK Matrix, there are 14 categories of techniques an adversary can use to perform their tactics. A lot of these technique sections also include sub techniques. For example, one of the most popular attacks, phishing, has a sub set of techniques like spearfishing, which aims at more important individuals through emails in hopes that the individual will think that the link is legit and click on it. The links can also be used to redirect the target to a site that persuades them to give sensitive information such as passwords to accounts.


CAR Knowledge Base

What is CAR?

CAR stands for "Cyber Analytics Repository". It is a knowledge base of analytics that is based on the MITRE ATT&CK adversary model. This repository is aimed at specific tools such as Splunk and EQL(Event Query Language)

Note: EQL is a query language for event-based time data, such as logs, metrics and traces. Basically it is a similar language to Splunks proprietary language SPL. 

In the lab, they use the technique  CAR-2020-09-001: Scheduled Task - File Access as an example. It is broken into three sections. The Technique, Subtechnique(s) and Tactic(s). 
It explains that in order to gain persistence, priviledge escalation, or remote execution, the actor can use the Windows Task Scheduler to schedule a command to run at a specific time,data, and even a select host machine. The scheduler is commonly know to reside in the path C:\Windows\System32\Tasks\. 

Note:This can be especially dangerous due to the set of folders on the way to the tasks, System32. If the melicious actor where to get access to say, a critic server through a pivot, they could delete this folder and render that server unsusable. This can do significant damage to any organization. 

MITRE Engage

What is MMITRE Engage?

MITRE Engage is a framework for planning and discussing adversary engagement operations that empowers you to engage your adversaries and achieve your cybersecurity goals. This is essentially a method of how to engage the adversary by implementing tactics such as Cyber Denial and Cyber Deception.

Note: Cyber Denial simply means to prevent the adversary's ability to conduct their normal oprations and Cyber Deception misleads them (EX: Honeypots and false data)

Engage also has its own matrix, which includes five main sections:

Prepare the set of operational actions that will lead to your desired outcome. (Input)
Expose adversaries when they trigger your deployed deception activities. 
Affect adversaries by performing actions that will have a negative impact on their operations.
Elicit information by observing the adversary and learn more about their methods(TTPs).
Understand the outcomes of the operational actions. (Output)

MITRE D3FEND

What is MITRE D3fEND


