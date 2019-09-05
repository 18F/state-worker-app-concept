# _Strength #4:_ Client experiences are intuitive, appropriate, and empowering.

The rules, requirements, and actions people need to take to qualify and receive benefits from public assistance programs are inherently complicated. Improving the experiences people have as they interface with these programs is also a very complex undertaking. The client experience should be thought of as a number of constituent parts that can be addressed separately as part of an incremental improvement strategy.

**Applying to programs should   be easy enough that a parent can apply with one hand on their phone while rocking their baby to sleep.**

The good news is that we _already know what this should look like._ Prior work has produced very good examples of how to do this. There's no need to start from scratch in this area.

## Design research

Research into the experiences people have before, during, and after applying, receiving, and using benefits helps us understand how we should design the systems they will interact with. This research should be ongoing, but we also need to utilize research that has already been conducted. There has already been quite a bit of thoughtful design research that provides great insight and is available today. While not nearly comprehensive, these reports provide a great jumping-off point.

Research: Mapping the applicant experience of benefit enrollment | Report: Streamlining Access to Public Benefits in Michigan
------------ | -------------
![cover of USDS report](/concept_assets/b_usds_cover.png) | ![cover of civilla / CfA report](/concept_assets/b_mi_cover.png)
USDS / CMS / 18F | CIVILLA / CODE FOR AMERICA
In 2016, applying a human-centered design approach, USDS and CMS explored the current state of benefit enrollment and delivery across agencies and states in an extensive qualitative user research field study. They had two aims. First, to better understand the applicant experiences of enrolling in programs such as food assistance, cash assistance and Medicaid. Second, to gather needs and best practices from state and county program administrators working to improve their systems. In partnership with state program offices, community based organizations and 18F, the team conducted 80 contextual interviews, site visits and service trials with applicants, non-profit staff and local program administrators across seven states. | “This report documents the findings and outcomes of two technology pilots led by Civilla and Code for America in partnership with the Michigan Department of Health and Human Services (MDHHS). The work in Michigan was focused on prototyping a faster, simpler, and more user-centered enrollment experience for food and healthcare benefits.”
[More on the USDS research](bit.ly/2LlC8aP) | [More on the Civilla/CfA report](bit.ly/michigan-report)


## Applying

Over the last several years, quite a bit of research and design work has been put into learning and developing a user-friendly approach to applying to public assistance programs. These efforts have produced an approach characterized by brief pages, plain and friendly language, personalized questions, and responsive interfaces.

With so much work needed to modernize these systems, it’s reasonable to consider the approach modeled by the following projects as “sufficiently solved”, meaning that if you don’t have a very good reason, you should just repurpose their approach as your starting point.

Improving the application experience is, of course, beneficial to the client. But it is also be a key aspect of modernizing the data intake and storage of a state system as well as adopting an encasement strategy. See [Exhibit C: A general model for data collection](#exhibit-c-a-general-model-for-data-collection)

### USDS/CMS Prototype: Multi-benefit application and enrollment

This prototype front-end experience builds on the research described in [_Mapping the applicant experience of benefit enrollment_ ](#design-research). It implements design principles and lessons-learned from working directly with applicants and state program staff. This open source project can be directly reused. It is a great starting point for any new client-facing applications and fits in well with an iterative, user-centric design process.

[**View the prototype**](https://bit.ly/2fl825t)

![screenshots of USDS prototype](/concept_assets/b_usds_prototype.png)

### Code for America / Civilla

Following a similar approach to the USDS/CMS prototype described to the left, the application experience initially implemented for GetCalFresh.org and subsequently for a pilot with the State of Michigan, utilizes many of the same design techniques to create an understandable, manageable experience.

[**View the Michigan repo**](bit.ly/2G5nEre)

![screenshots of Code for America application prototype](/concept_assets/b_cfa_getcalfresh.png)

## Design systems

Design systems are pre-built libraries of styles and interaction patterns that allow teams to inherit good decisions from other teams who have focused on developing usable, accessible, mobile-first front-end interfaces. By reusing these decisions, teams can avoid duplicative work and instead focus on their product needs.

### U.S. Web Design System

The U.S. Web Design System is a design system built for the federal government backed by user research. The USWDS provides a variety of patterns appropriate for customer-facing applications. As the USWDS website states, “It’s counterproductive and wasteful to recreate basic components and patterns for every new government website...Enable teams to focus on the their users and their mission, and less on reinventing existing solutions. Do less to do more.”

![Sample screenshots of U.S. Wed Design System](/concept_assets/b_uswds.png)

### CMS Design System

CMS’s Web & New Media Group built upon the U.S. Web Design System to create a version appropriate to their needs. The CMS Design System is currently in use for HealthCare.gov. That means that the system is already in use with the same population as state E&E systems and expertise currently exists within CMS related to its use.

![Sample screenshots of CMS Design System](/concept_assets/b_cmsds.png)
