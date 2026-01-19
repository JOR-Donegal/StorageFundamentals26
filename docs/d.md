# Management Processes

When we utilise storage technologies, we need to make sure we can carry out the required management tasks. In anything bigger than an SME, these are formal tasks which will have associated SOPs, controls, etc. and there may be teams of people associated with each process. The tasks listed apply to most technical silos in a data centre. 

## Monitoring 
Every subsystem in the datacentre needs to be monitored in real time. There may be an Operations Centre, normally identified by the large plasma screens and bewildered staff with 1,000-yard stares. _Key Performance Indicators_ (KPIs) are displayed, in addition to status, configuration, availability, performance, alarms, events and security status. 

## Reporting 
Data which is gathered by the monitoring systems needs to be summarised and relevant, consumable reports are generated. 

## Planning and Projects 
Based on report summaries, we should be able to understand our capacity and our resilience and contingency capabilities. If this information is combined with business projections, there may be sufficient information to plan. __I define projects as activities that have a start and a finish__. 

There is some variation in style and terminology, but most managers will plan at three distinct levels: 

Operationally, what are we doing now?
- What staff are available for shift work at weekends this month?

Tactically, what changes do we need to make over the next budget cycle, 18 months or so.
- What is End of Support (EOS) for Windows 2022, when do we need to decommission the last system?

Strategically, what changes do we need to make in the long term, 2-5 years.
- Should we move systems to public cloud or continue to run our own data centres? 

## Provisioning 
Resources are allocated as required and the general term we use is provisioning. Some engineers refer to “standing up storage” which is another way of saying the same thing. 

## Service and Maintenance 
Service activities differ from projects. __Services run perpetually, without a start or finish, until the end of service lifetime__. Anyone who is ITIL trained will cringe at that definition! 

Feel free to do some research to get a more complete definition. A successful operation aims to have no unscheduled outages. Almost every environment allows for scheduled outages and maintenance windows, but this should all be planned and communicated. In a modern data centre with resilience and high availability, we should be targeting an SLA with five nines (look it up!) and effectively no unscheduled outages.
