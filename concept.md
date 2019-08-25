# Introduction

Much of the technology that people use to access safety net programs and States use to administer those programs is aging and crumbling, despite ssignificant spending and effort to modernize.

**Our current approaches to fixing this situation play right into government’s weaknesses.**

We ask over-stretched, insufficiently technical state staff to modernize massively complex computer systems by adhering to federally-provided checklists and oversight regimes, working with massive vendors through multi-year contracts worth tens or hundreds of millions of dollars.

But states are not well positioned to build software, modernize legacy systems, productively manage vendors, easily comply with oversight, or deliver timely and trustworthy data. Federal agencies are not well positioned to quickly drive change in the market or provide technical oversight that accelerates modernization rather than impedes it.

The way we approach technology for safety net programs forces states to dwell on their weaknesses, buckling under the weight.

**We need to move to a position of strength** if we are to repair these aging systems to deliver the services people need and Congress has defined.

**This piece attempts to envision a position of strength.** This position of strength includes:

- An eco-system of loosely-coupled products, services, and data powers rapid modernization and ongoing evolution across states _(rather than disconnected, proprietary, monolithic systems)_
- Effective federally-built software is available for states to use (rather than every state building every part)
- Eligibility policy is delivered as functional code _(rather than just written guidance)_
- Client data is secure, structured, and API-accessible _(rather than locked in inaccessible databases)_
- Client experiences are intuitive, appropriate, and empowering _(rather than opaque and demoralizing)_
- State staff have tools that help them help them achieve their mission _(rather than just compliance)_  

**By developing these strengths at the federal level, we can create tools states would _choose_ to use because they are preferable and allow them to focus on service delivery and meeting the needs of the people who need the services.**

That’s the whole point, after all.

> _Please note: Big, grandiose concept pieces like this are always wrong. Or rather, they get a lot of things wrong. The point is not to get everything exactly right, but to move the conversation along and attract participation in rethinking broad assumptions and conventions._

### Inside this concept

[**Exhibit A: An ecosystem of products**](#exhibit-a-an-ecosystem-of-products) - Recent work on the applicant experience has largely figured out what applying should look like.

[**Exhibit B: Client experiences**](#exhibit-b-client-experiences) - Recent work on the applicant experience has largely figured out what applying should look like.

[**Exhibit C: A general model for data collection**](#exhibit-c-a-general-model-for-data-collection) - A look at how we might receive data from clients, use it to find programs that can meet their needs, and make data reporting easy.

[**Exhibit D: Eligibility rules as a service**](#exhibit-d-eligibility-rules-as-a-service) - Recent work on codifying program policy into rules that can be accesses via web services has shown the feasibility of the approach.

[**Exhibit E: State Eligibility & Enrollment App**](#exhibit-e-state-eligibility--enrollment-app) - A concept for what a tool that empowers eligibility workers to meet their mission could look like.

[**Exhibit F: Models for building products**](#exhibit-f-models-for-building-products) - A look at how we might shift our system development models to more efficient, less redundant, more successful methods of production.

[**Exhibit G: Design systems**](#exhibit-g-design-systems) - Government design systems have defined good practice for how public-facing systems should look and function.

# Exhibit A: An ecosystem of products

### The current organizing principles around eligibility systems need to change.

We should shift away from single state-based, monolithic (in both the architectural sense and the de facto monolithic nature of dependency on a single locked-in vendor), disconnected, does-everything state systems towards a more interconnected ecosystem of loosely-coupled products, each part with focused responsibility and capable ownership, connected with APIs, creating usable experiences designed around the needs of their users.

The diagram below can be used as a map to explore this piece. The ecosystem described below is in no way complete, but describes what’s covered in this piece.

![diagram visualizing the four aspects described below](/concept_assets/a_diagram.png)

**Clients experiences** - Clients apply, submit documents, have visibility into status, notices/notifications, through government and non-government channels - See exhibits:
> - [Exhibit B: Client experiences](#exhibit-b-client-experiences)
> - [Exhibit G: Design systems**](#exhibit-g-design-systems)
> - [Exhibit F: Models for building products](#exhibit-f-models-for-building-products)

**Modern data storage** - Source of truth, data coming in from multiple sources, data going out powering multiple products, commodity databases on cloud infrastructure - See exhibits:
> - [Exhibit C: A general model for data collection](#exhibit-c-a-general-model-for-data-collection)
> - [Exhibit F: Models for building products](#exhibit-f-models-for-building-products)

**Worker experiences** - Eligibility workers, managers, and directors have empowering tools that allow them to do their work efficiently and serve their mission - See exhibits:
> - [Exhibit F: Models for building products](#exhibit-f-models-for-building-products)
> - [Exhibit E: State Eligibility & Enrollment App](#exhibit-e-state-eligibility--enrollment-app)

**Eligibility rules services** - Policy is delivered as working code, accommodating state options and avoiding the uncertainty of interpretation and implementation - See exhibit:
> - [Exhibit D: Eligibility rules as a service](#exhibit-d-eligibility-rules-as-a-service)

# Exhibit B: Client experiences

The rules, requirements, and actions people need to take to qualify and receive benefits from public assistance programs are inherently complicated. Improving the experiences people have as they interface with these programs is also a very complex undertaking. The client experience should be thought of as a number of constituent parts that can be addressed separately as part of an incremental improvement strategy.

**Applying to programs should   be easy enough that a parent can apply with one hand on their phone while rocking their baby to sleep.**

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


# Exhibit C: A general model for data collection

Traditional paper applications for individual programs established the precedent of gathering the data needed to determine program eligibility separate from data needed to determine eligibility for other programs. The move to digitize those applications largely recreated this practice.

Other methods of bridging the distinctions, such as presumed eligibility or data sharing, aim to ease the burden of duplicative re-entry of data.

Yet if we’re working to establish a truly intergrated eligibility experience, where a person or household can apply once and eligibility can be determined for a variety of programs, we need to break data collection and individual program applications.

Data should be entered in aggregate for all relevant programs in the most intuitive way for the applicant ([See Exhibit B: Client experiences](#exhibit-b-client-experiences)) and then used to determine individual programs behind the scenes.

![Illustration visualizing the 7 points below](/concept_assets/c_illustrations.png)

1. Structure aggregate data and understand which programs need what data
2. Identify the services/programs applicants may need
3. Collect the data needed for all relevant programs at once
4. State staff review/verify data
5. Use the collected data to concurrently apply to programs separately
6. Determine eligibility based on each application
7. Issue benefits to applicants

# Exhibit D: Eligibility rules as a service

# Exhibit E: State Eligibility & Enrollment App

# Exhibit F: Models for building products

# Exhibit G: Design systems
