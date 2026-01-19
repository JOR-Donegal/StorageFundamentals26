# Priorities
On any security course, the introductory notes will mention the _CIA triad_: confidentiality, integrity, and availability. I am a big critic of this as is over-simplistic and ignores characteristics which might be important in specific cases, like safety or non-repudiation. Every student report (and many highly paid consultants) treat this as a axiomatic: this is science and engineering, axioms better have provenance! 

It might be useful to apply the same thinking and arguments to storage; what are the management priorities? 

I will start with the obvious ones! 

## Confidentiality and Data Security 
We look aghast at incidents around the world, where millions of people are affected on an apparently on-going basis by massive data breaches. The cost is apparently borne by the victims with limited blow-back to the companies which were the cause of the data breaches. Europe is at the forefront of a change in the way we think about personal data and our approaches are world leading. With the advent of GDPR, a data breach where a company is culpable may be financially ruinous. Controls are required, along with policies, SOPs, and strong access controls. 

## Integrity 
A well-designed storage system implements data integrity using techniques which give predictability; we should be able to calculate a mean time to data loss (MTTDL). During this module, we will look at error-correcting codes (ECC), parity, RAID, and newer techniques like erasure coding. 

## Availability and Reliability 
This applies as it does in the security realm. If data is not available when its required, it may lead to contractual breach, financial loss and reputational damage. 

## Capacity, Scalability and Performance 
How do you predict how a system will grow over its lifetime and what are the implications if you get it wrong? If my laptop’s single hard drive is too small, I will need to scale-up and replace it with a bigger one. However, if I have the same problem of my desktop, I have spare slots, SATA/NVMe ports and power supply leads, I can just add hard drives; I can scale-out. And if I'm using a volume manager I can do this non-disruptively. ## These are important concepts in data centres and a well-planned system will have the ability to increase capacity without affecting availability and disrupting business. These concepts should apply to all the assets we deploy: compute, storage, network and as a result, applications and throughput. 

## Manageability 
Everything we do in the data centre environment must be manageable. In a modern software-defined environment, we can script and automate much of what we must configure; this makes it efficient, repeatable and in most cases, less prone to error. In the data centre world, we call this provisioning. We need to monitor, to be able to see what is going on. We need dashboards with key performance indicators to understand and respond to status. Our management systems should facilitate maintenance and response to incidents. These systems should allow for consistent reporting, we can use these reports as a basis to foresee requirements and plan for change. 

## Maintainability 
Systems need regular updates. The sequence of finding bugs, writing and testing updates and then deploying them is terrible, but it’s the only strategy we currently have. The ability to update needs to be designed into any storage system.

## Safety
In an industrial plan, or a health setting, if we cannot operate safely, we should not operate. In critical infrastructure, this may be the lead priority.