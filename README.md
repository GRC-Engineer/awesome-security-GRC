<img src="https://www.ideagen.com/media/11748/grc-circle.png" width="300" class="center">

# :tada: Grand Repository Challenge accepted!

This is a list of resources for security GRC folks.

Each of you probably has a different title. Cyber Risk Managers, Security Compliance Program Managers, Business Information Security Officers, Head of the Department of **No**, etc.

This variety makes it more challenging to come together as a community compared to software engineer to organize knowledge and share information.

Our field is pretty new and has exponentially grown in the past five years.

We can work for SaaS companies (me! :bowtie:), financial services, healthcare, government, retail or a dozen other industries. Scope, budget, stakeholders and degrees of resentment can vary but some work activities are common to all of us (the resentment as well).

So the thought was, why not build a knowledge bank for GRC. I know it's a GitHub repo but that gives the endeavour some illusion of grandeur. I just thought content curation lists were amazing and that we should have one!

This is GitHub which means, Pull Requests are more than welcome! Nothing here is gospel, definitions are often subject to debates and heated discussions on LinkedIn and everyone has a different opinion on G, R and C (hatred for C is probably consensual IMHO).

Feel free to share your resources or add cooler emojis.

> *This might include expert expert puns and boomer jokes*

## :notebook_with_decorative_cover: Contents

- [:tada: Grand Repository Challenge accepted!](#tada-grand-repository-challenge-accepted)
  - [:notebook_with_decorative_cover: Contents](#notebook_with_decorative_cover-contents)
- [:mortar_board: What is Security GRC?](#mortar_board-what-is-security-grc)
  - [:guardsman: Governance](#guardsman-governance)
  - [:chart_with_upwards_trend: Risk Management](#chart_with_upwards_trend-risk-management)
    - [Risk Management Frameworks](#risk-management-frameworks)
      - [Rapid Risk Assessment](#rapid-risk-assessment)
      - [Factor Analysis of Information Risk](#factor-analysis-of-information-risk)
      - [ISO 27005](#iso-27005)
      - [NIST 800-39](#nist-800-39)
  - [:gun: Audit & Compliance](#gun-audit--compliance)
    - [:octopus: Frameworks and Regulations](#octopus-frameworks-and-regulations)
- [:books: Books](#books-books)
- [:tv: Talks/Videos](#tv-talksvideos)
- [:telephone_receiver: People you should know](#telephone_receiver-people-you-should-know)
  - [:sunglasses: Thought Leaders](#sunglasses-thought-leaders)
  - [:iphone: Follow them on LinkedIn](#iphone-follow-them-on-linkedin)
- [:octocat: Repositories](#octocat-repositories)
- [:microphone: Podcasts](#microphone-podcasts)
  - [Security GRC Podcasts](#security-grc-podcasts)
  - [Security GRC Episodes](#security-grc-episodes)
- [:scroll: Certifications](#scroll-certifications)
- [:triangular_ruler: The Knowledge Trifecta](#triangular_ruler-the-knowledge-trifecta)
  - [:floppy_disk: The Technical](#floppy_disk-the-technical)
  - [:lock_with_ink_pen: The Security](#lock_with_ink_pen-the-security)
  - [:briefcase: The Business](#briefcase-the-business)

# :mortar_board: What is Security GRC?

The security GRC field is covering lots of ground and include a varied number of tasks and responsibilities. Some of them will sound exciting, some will reignite painful memories.

## :guardsman: Governance

Governance, as the name implies, focuses on how security is managed and its oversight. This could include building the security strategy, managing the security programme and ensuring continous monitoring of workstreams.

This would also be the area responsible for orchestration and metrics for your security programme. In other words, the always useful dashboard with 15 graphs and thousands of data points would be include in the governance efforts. Your policies and procedures are also part of Governance as they help shape your vision of security and detail what is expected from everyone.

Managing stakeholders is also central to Governance efforts. Relationship with the different teams, managing upwards and delivering the right level of information to senior executives.

## :chart_with_upwards_trend: Risk Management

How do I know what's the priority for my security programme? Lockdown end-user access or focus on patching? (probably both lol) The only way to make rational decisions regarding what to do is to perform risk assessments.

Risk is traditionally explained as a factor of a threat and a vulnerability. Pretty simplistic (probably false as well) but it gets the job done:
* A threat is a potential harmful event that could impact your organisation
* A vulnerability is a known weakness that could be exploited
* A risk is threat * vulnerability... A risk is the impact if the threat exploits the vulnerability (R = T*V)

A robust risk management program would also include some quantitative features to make sure senior management and business executives understands the financial costs associated with some of the identified risks. Nothing has to be too precise or too detailed, having numbers in the right ballpark and being able to evidence why you chose them is well more than enough.

### Risk Management Frameworks (RMF)

A risk management framework describes the vocabulary, tools and techniques for a coherent approach and ensure that all stakeholders are on the same page.

Enterprise frameworks identifies _any type of risk_ that could prevent the company from achieving its business objectives while others focus on information security, cybersecurity and privacy protection.

#### COSO Enterprise Risk Management

The Committee of Sponsoring Organizations of the Treadway Commission [(COSO)](https://www.coso.org) help organizations improve internal control with the [ERM Framework (2020)](https://www.coso.org/Documents/Compliance-Risk-Management-Applying-the-COSO-ERM-Framework.pdf).

#### Factor Analysis of Information Risk (FAIR)

[Fair](https://www.fairinstitute.org/) is a quantitative model for information security and operational risk.

#### International Organization for Standardization (ISO)

[ISO/IEC 27005:2022
Information security, cybersecurity and privacy protection — Guidance on managing information security risks](https://www.iso.org/standard/80585.html) provides guidelines to managing _information security risks_ faced by organizations. The application of these guidelines can be applied to an Information Security Management System (ISMS) specified in ISO/IEC 27001 and ISO/IEC 27002.

A technical committee named [ISO/IEC JTC 1/SC 27](https://www.iso.org/committee/45306.html) focus on the development of standards for the protection of information and ICT.

[ISO 31000](https://www.iso.org/iso-31000-risk-management.html) provides a common approach to managing _any type of risk_ faced by organizations. The application of these guidelines can be customized to any organization and its context.

The ISO 31000 Risk Management umbrella include some specifications still under development:
ISO 31000:2018
Risk management — Guidelines
 * [ISO 31000 Risk management – Guidelines](https://www.iso.org/standard/65694.html)
 * [ISO 31000:2019 Risk Management – Risk Assessment Techniques](https://www.iso.org/standard/72140.html)
 * [ISO 31022:2020 Risk Management — Guidelines for the management of legal risk](https://www.iso.org/standard/69295.html)
 * [ISO/FDIS 31030 Travel Risk Management — Guidance for organizations](https://www.iso.org/standard/54204.html)
 * [ISO/AWI 31050 – Guidance for managing emerging risks to enhance resilience](https://www.iso.org/standard/54224.html)
 * [ISO/DIS 31073 Risk Management – Vocabulary](https://www.iso.org/standard/79637.html)

A technical committee named[ISO/TC 262](https://www.iso.org/committee/629121.html) focus on the development of standards in the field of risk management. Visit the Technical Committee's own [website](https://committee.iso.org/home/tc262) for more information.

#### NIST

The [NIST Risk Management Framework](https://csrc.nist.gov/Projects/risk-management) provides a process that integrates security, privacy and risk management activities into the system development life cycle to meet the requirements of the Federal Information Security Modernization Act [(FISMA)](https://www.cisa.gov/federal-information-security-modernization-act).

Note that [NIST Special Publications 800-53 revision 5](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-53r5.pdf) describe the Security and Privacy Controls for Information Systems and Organizations and the [special publication 800-53*B*](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-53B.pdf) describe the control baselines.

*Related initiatives**

* [Special Publication 800-37: Risk Management Framework for Information Systems and Organizations: A System Life Cycle Approach for Security and Privacy](https://csrc.nist.gov/publications/detail/sp/800-37/rev-2/final)
* [Special Publication 800-39: Managing Information Security Risk: Organization, Mission, and Information System View](https://csrc.nist.gov/publications/detail/sp/800-39/final)
* [Special Publication 800-30 Rev. 1: Guide for Conducting Risk Assessments](https://csrc.nist.gov/publications/detail/sp/800-30/rev-1/final) 
* [Special Publication 800-53A: Assessing Security and Privacy Controls in Federal Information Systems and Organizations: Building Effective Assessment Plans](https://csrc.nist.gov/publications/detail/sp/800-53a/rev-4/final) 
* [Special Publication 800-161: Supply Chain Risk Management Practices for Federal Information Systems and Organizations](https://csrc.nist.gov/publications/detail/sp/800-161/final)

#### Operationally Critical Threat, Asset and Vulnerability Evaluation (OCTAVE)

The [OCTAVE method](http://www.cert.org/octave) was developed by the Software Engineering Institute (SEI) at Carnegie Mellon University on behalf of the Department of Defense.

#### Rapid Risk Assessment

The [Rapid Risk Analysis (RRA) methodology](https://infosec.mozilla.org/guidelines/risk/rapid_risk_assessment.html) developed by Mozilla helps formalize decisions in 60 minutes.

#### Threat Agent Risk Assessment (TARA)

[Threat Assessment and Remediation Analysis (TARA)](https://www.mitre.org/publications/technical-papers/threat-assessment-and-remediation-analysis-tara) is an engineering methodology used to identify and assess cyber vulnerabilities and select countermeasures effective at mitigating those vulnerabilities. TARA is part of a MITRE portfolio of systems security engineering (SSE) practices.

### Risk Management Tools & Packages

* [*Comply*](https://github.com/strongdm/comply)
  * Comply is a SOC2-focused compliance automation tool.  
    * Policy Generator: markdown-powered document pipeline for publishing auditor-friendly policy documents
    * Ticketing Integration: automate compliance throughout the year via your existing ticketing system
    * SOC2 Templates: open source policy and procedure templates suitable for satisfying a SOC2 audit
* [*CISO Assistant*](https://github.com/intuitem/ciso-assistant-community)
  * One-Stop-Shop solution for Governance, Risk Management and Compliance
  * Support +46 frameworks worldwide
  * Available in +8 languages
  * Suppport multi level frameworks and maturity assessment
  * One-click Audit report generation
  * API available, which gives a lot of options for integration and automation
  * Customizable and extensible with an open format and simple syntax (for custom framework or personalized matrix)
  * Open-source first and Very active community 

#### Netflix's riskquant

[riskquant](https://github.com/Netflix-Skunkworks/riskquant) is a python library used for risk quantification. It can be used to do cool things like calculate annualized loss and generate loss exceedance curve charts.

You can use it to assess individual risks or even build automation to run calculations and build charts for all risks where data are available. For example, you can set up a GitHub Action to pull risks from your GRC tool, get the data to run the calculations, and put the results back into your GRC tool.

## :gun: Audit & Compliance

Once you know what your direction is and you know what to focus on, how do you know you're on track? There's two ways:
* Auditing allows you to know if the controls you chose and your security programme is working effectively
* Compliance is how close are you to the baseline either set by yourself or by a 3rd party body (ISO, AICPA, insert acronyms)

Often hated (often for good reasons), audit and compliance folks have to be annoying by nature. They assess how things you said you'd do are actually done in the real world. More often than not, things are either not done as they should or not done at all. Probably because no one has read the policies you took six months to write!

### :octopus: Frameworks and Regulations

Well...  There are a lot.  Your organization likely uses some of these, but certainly not all. Executive leadership drives policy at a high level based on business objectives. Certain regulations are mandatory. For instance Sarbanes-Oxley Act (SOX) for US publicly traded companies or General Data Protection Regulation (GDPR) applies to any organisation handling data from EU citizens. This is a non-exhaustive alphabet soup of frameworks and regulations:

* :bank: Sarbanes-Oxley Act - [SOX](https://www.congress.gov/bill/107th-congress/house-bill/3763)
* :euro: General Data Protection Regulation - [GDPR](https://gdpr-info.eu/)
* :credit_card: Payment Card Industry Data Security Standard - [PCI-DSS](https://www.pcisecuritystandards.org/)
* :hospital: Health Insurance Portability and Accountability Act - [HIPAA](https://www.hhs.gov/hipaa/index.html)
* :white_flag: International Organisation for Standardization's Information Security Management Standard - [ISO 27001](https://www.iso.org/isoiec-27001-information-security.html)
* :computer: Systems and Organization Controls for Service Organizations: Trust Services Criteria - [SOC2](https://www.aicpa.org/interestareas/frc/assuranceadvisoryservices/aicpasoc2report.html)
* ☁️ Federal Risk and Authorization Management Program - [FedRAMP](https://www.fedramp.gov/)
* :statue_of_liberty: Federal Information Security Modernization Act - [FISMA](https://www.cisa.gov/federal-information-security-modernization-act)
* :oncoming_police_car: Security and Privacy Controls for Information Systems and Organizations - [NIST SP 800-53 Rev. 5](https://csrc.nist.gov/publications/detail/sp/800-53/rev-5/final)
* 🗄️ Protecting Controlled Unclassified Information in Nonfederal Systems and Organizations - [NIST SP 800-171 Rev. 2](https://csrc.nist.gov/publications/detail/sp/800-171/rev-2/final)
* 📏 NIST Cybersecurity Framework - [NIST CSF](https://www.nist.gov/cyberframework)
* 🇪🇺 Directive on measures for a high common level of cybersecurity across the Union - [NIS2 Directive](https://digital-strategy.ec.europa.eu/en/policies/nis2-directive)

Added to that, each country would have specific cybersecurity regulations and standards companies would have to comply with. They could be specific to certain industries (critical infrastructures or financial services) or applicable to every company. As our planet is made of a lot of countries, we won't list the specifics here and as is often the case, US standards are picked up in most of the world anyway!

# :books: Books

* [**Security Risk Management**, *Evan Wheeler*, 2011](https://learning.oreilly.com/library/view/security-risk-management/9781597496155/)
  * Often part of reading lists at universities, this is your first stop in security risk management. This book is both comprehensive, timeless and accessible
  * Great for referencing, it will help you assess and improve your internal risk management program. Focus on the **Action Plans** at the end of each chapter for some great takeaways

* [**Measuring and Managing Information Risk**, *Jack Freund & Jack Jones*, 2014](https://learning.oreilly.com/library/view/measuring-and-managing/9780124202313/)
  * The FAIR book itself. Self explanatory, if you want to know more about risk quantification this is a must-read, the story in the intro is meme material.

* [**How to Measure Anything in Cybersecurity Risk**, *Douglas Hubbard & Richard Seiersen*, 2016](https://learning.oreilly.com/library/view/how-to-measure/9781119085294/)
  * Amazing primer on Cyber Risk Quantification as a whole. Keep these things in mind:
    * Your problem is not **as unique** as you think
    * You **have *more* data** than you think
    * You **need *less* data** than you think

* [**Transformational Security Awareness**, *Perry Carpenter*, 2019](https://learning.oreilly.com/library/view/transformational-security-awareness/9781119566342/)
  * The best Security Awareness book ever written. You'll need this because GRC teams often handle Security Awareness and this will be a great resource to kickstart your program
  * Goes through the tools you need to build an effective awareness strategy, Marketing, Communications, Behavioural Science, Culture Management, etc. If advertisers have been successful for the past half century, we probably have something to learn from them!

* [**Foundations of Information Security**, *Jason Andress*, 2019](https://learning.oreilly.com/library/view/foundations-of-information/9781098122546/)
  * High-level overview of Information Security, touching on every topic relevant for a practitioner or a newcomer to the field
  * This baseline of knowledge is great to ensure you understand every control in your framework of choice

* [**ISO 27001 controls – A guide to implementing and auditing**, *Bridget Kenyon*, 2019](https://learning.oreilly.com/library/view/iso-27001-controls/9781787781467/)
  * Bridget Kenyon has been involved in the development of the ISO 27001 standards for over a decade so you should probably listen
  * This goes through every control from Annex A. and provides guidance and how to implement and audit them. Useful for building your ISMS, performing internal audits or kickstarting your career as a beloved ISO auditor!

* [**IT Auditing Using Controls to Protect Information Assets**, *Mike Kegerreis, Mike Schiller and Chris Davis*, 2019](https://learning.oreilly.com/library/view/it-auditing-using/9781260453232/)
  * IT Auditing stems from the increase of regulations that followed major financial scandals of the early 2000s. This is dominated by the Big Four audit firms for obvious reasons even though major corporations have internal staff dedicated to IT auditing
  * This book is an encyclopedia that goes through how to audit everything from Data Centers to Networking Devices and from Web Applications to Windows Servers
  * Written by industry experts with decades of experience, this will also be useful to GRC folks trying to understand some of the controls to verify with their teams armed with the underlying technical knowledge and know-how necessary

* [**A Leader's Guide to Cybersecurity**, *Thomas J. Parenty and Jack J. Domet*, 2019](https://learning.oreilly.com/library/view/a-leaders-guide/9781633698000/)
  * Great opportunity to understand security when it's written for the business. Down to earth and debunks some of the tropes we often repeat such as Security as a "People Problem"
  * Follows this structure: The Problems => The Principles => The Responsibilities

* [**Rational Cybersecurity for Business: The Security Leaders' Guide to Business Alignment**, *Dan Blum*, 2020](https://learning.oreilly.com/library/view/rational-cybersecurity-for/9781484259528/)
  * Another book about Security, Business and how to align the two. This book is an overview of the most useful controls and how to improve your security posture seamlessly and without impeding productivity

* [**The Cybersecurity Manager's Guide**, *Todd Barnum*, 2021](https://learning.oreilly.com/library/view/the-cybersecurity-managers/9781492076209/)
  * Probably the best information security book you'll ever read, Todd has been the CISO of GoPro for 6 years and worked in a variety of industries in the last three decades
  * What defines our field:
    * Nobody Really Cares
    * Nobody Understands
    * Fear Drives Our Industry
  * The Four Cornerstones of your Security Program:
    * Documentation
    * Governance
    * Security Architecture
    * Communication, Education and Awareness

# :tv: Talks/Videos

* A [great foundational talk](https://www.youtube.com/watch?v=dt2IqidgpS4) to understand how every framework are working into one another:
  * :green_book: **Control Frameworks** such as *NIST 800-53* or *CIS 20 Controls* for building your security baseline
  * :orange_book: **Program Frameworks** such as *ISO 27001* or *NIST CSF* to standardize an overarching security program
  * :blue_book: **Risk Frameworks** such as *NIST 800-37* or *FAIR* to identify, measure and quantify risk

* I have a full playlist of over [80 videos focus on Risk Management and Cyber Risk Quantification,](https://www.youtube.com/playlist?list=PLj4UOrWWdhG-Lqk9DOvShUdbwRZcGWhRH) will update it soon but it already has a lot.
  * This quick live [Quantitative Cyber Risk Analysis](https://www.youtube.com/watch?v=fHUv8TJC6kM&list=PLj4UOrWWdhG-Lqk9DOvShUdbwRZcGWhRH) from *Evan Wheeler* is a great overview of how straightforward a quantitative analysis can be
  * *Steve Reznik* has numerous talks on how FAIR can help build meaningful KRIs but [this one](https://www.youtube.com/watch?v=w4x1tWTiCHg&list=PLj4UOrWWdhG-Lqk9DOvShUdbwRZcGWhRH) is a good suggestion.

# :telephone_receiver: People you should know

## :sunglasses: Thought Leaders

* :dvd: Everything written by [***Ryan McGeehan***](https://scrty.io/).
  * His website references over a dozen articles on Risk Management. Some of them are [*waaaay*](https://magoo.medium.com/hypothesis-risk-and-science-439fc8b05ffb) over my head
  * His various experience at Coinbase and Facebook and as a Start-up security advisor makes his input super relevant if you're working at SaaS company as an example

* :bank: Everything written by [***Phil Venables***](https://www.philvenables.com/home).
  * His take on most subjects are worth the read, he has a great analysis of the [*Compliance vs. Security*](https://www.philvenables.com/post/compliance-vs-security) debate
  * Phil has over 20 years of experience in security leadership at Goldman Sachs and now the CISO of Google Cloud

* :rotating_light: Everything from ***Adobe's Tech GRC Team***.
  * They've been at the forefront of innovation in the field, even building their own [Common Control Framework](https://blog.adobe.com/en/publish/2020/11/19/common-controls-framework-ccf-by-adobe-v4-0-now-available.html#gs.1v9q24). They produced numerous posts I suggest you have a look at:
  * Managing everyone's input, role and expectations into the overall security compliance effort can often be cumbersome. Adobe Tech GRC Team [introduced scalability by creating **four major roles**](https://medium.com/adobetech/scaling-security-controls-across-the-enterprise-5870e14f4865) to map to the CCF standard and help achieve GRC in a [**multi-cloud environment**](https://medium.com/adobetech/enabling-compliance-and-governance-at-scale-in-a-multi-cloud-environment-82847ba5d341)
  * Automating the Common Controls Framework, [Part I](https://medium.com/adobetech/automating-the-common-controls-framework-ccf-part-i-83271bdb0f00) and [Part II](https://medium.com/adobetech/automating-the-common-controls-framework-part-ii-d010bea9bcc4). Adobe as a major SaaS provider has to have a Tech GRC program that scales accordingly and these two articles introduce the **4-layer model** used to automate security compliance
  * A major feature of their Tech GRC program are the [**Strategic Technology Initiatives**](https://medium.com/adobetech/how-our-strategic-technology-initiatives-program-helps-automate-and-scale-key-security-initiatives-bd666440ed4b). They are the equivalent of the DevOps principles but applied to technology GRC efforts. A must-read
  * If articles aren't your thing, check out [this podcast](https://techspective.net/2021/03/23/prabath-karanth-shares-adobes-creative-approach-to-managing-grc/) with former leader from Adobe Tech GRC Prabhath Karanth. Great overview of the program and the STIs

* :ticket: Everything from ***Atlassian's Risk & Compliance Team***
  * Working in a cloud-native, agile, DevOps and innovative (insert buzzwords) environment isn't the most intuitive for a GRC Team. Mapping controls and performing audits when speed trumps everything is challenging to say the least.
  * Guy Herbert wrote a great series based on this talk called [**DevOps vs. Compliance, A Guide to Having it All**](https://www.youtube.com/watch?v=r4vznrYn2Qk).
    * [**Part 1**](https://community.atlassian.com/t5/Compliance-articles/Series-How-to-prioritize-compliance-without-losing-development/ba-p/1095733) explains that:
      * Compliance is being able to show that you follow the rules.
      * Risk management is balancing upsides and downsides.
    * [**Part 2**](https://community.atlassian.com/t5/Compliance-articles/Series-How-to-prioritize-compliance-without-losing-development/ba-p/1100861) walks you through what compliance obligations, control objectives and control activities are and the different planning phases to reach compliance automation
    * [**Part 3**](https://community.atlassian.com/t5/Compliance-articles/Series-How-to-prioritize-compliance-without-losing-development/ba-p/1106264) demonstrates with the Atlassian product suite how compliance is embedded into the CI/CD pipeline
    * [**Part 4**](https://community.atlassian.com/t5/Compliance-articles/Series-How-to-prioritize-compliance-without-losing-development/ba-p/1113058) deals with how to sell such a cutting-edge approach to auditors and why agility and compliance CAN live in harmony :)

## :iphone: Follow them on LinkedIn

* [*Troy Fine*](https://www.linkedin.com/in/troyjfine/), GRC general knowledge and SOC focus.

* [*AJ Yawn*](https://www.linkedin.com/in/troyhunt/), GRC general knowledge and SOC focus.

* [*Aron Lange*](https://www.linkedin.com/in/ajyawn/), ISO 27001 focus.

* [*Jacob Horne*](https://www.linkedin.com/in/jacob-evan-horne/), NIST and CMMC focus.

* [*Ayoub Fandi*](https://www.linkedin.com/in/ayoubfandi/), GRC general knowledge and cloud-native GRC focus.

# :octocat: Repositories

* [*Minimslist Risk Management*](https://github.com/magoo/minimalist-risk-management)
  * Ryan McGeehan, a founder/advisor for HackerOne, has developed minimalist documentation to describe a simple risk management program.

# :microphone: Podcasts

* [*The SecureWorld Sessions*](https://podcasts.apple.com/us/podcast/the-secureworld-sessions/id1478674556)
  * Cybersecurity weekly podcast series featuring industry thought leaders discussing security solutions, best practices, threat intel, and more.

* [*Cloud Security Podcast*](https://cloudsecuritypodcast.tv/)
  * Cloud Security weekly podcast series featuring industry thought leaders in Cloud Security from companies like Linkedin, Netflix, Twilio, CapitalOne & more discussing Cloud security challenges and how they guest solved them, best practices, offensive side of cloud security, and more.

## Security GRC Podcasts

* [*Security & Compliance Weekly*](https://podcasts.google.com/feed/aHR0cHM6Ly9zY3dhdWRpby5saWJzeW4uY29tL3Jzcw) - Hosted by Jeff Man, Scott Lyons and Josh Marpet
  * The name is pretty telling. PCI is often discussed in-depth, useful if you're responsible for your company's PCI-DSS program!

* [*Risk, Governance and Cyber Compliance*](https://open.spotify.com/show/5bHDGCy7HopSh2tpA4ZRoL) - Hosted by Dr. Bill Souza
  * The last episode dates back to late 2020 but the content is top-notch and his views on risk management are worth a listen.

* [*The GRC Podcast*](https://www.thegrcpodcast.com/) - Hosted by Mark Graziano
  * The goal of this podcast is to shine light on GRC security champions and showcase the much of a dynamic security discipline GRC is.


## Security GRC Episodes

* [**Getting Over Our "Security ≠ Compliance" Obsession**, *CISO-Security Vendor Relationship Podcast*](https://podcasts.google.com/feed/aHR0cHM6Ly9kYXZpZHNwYXJrLmxpYnN5bi5jb20vY2lzb3ZlbmRvcg/episode/ZThiNjFmNGU0ZTVhNDAzM2E4YTQxZDkzYjE0M2E3NjA?sa=X&ved=0CAIQuIEEahcKEwiAg7brqqnxAhUAAAAAHQAAAAAQIQ) - Featuring David Spark, Mike Johnson and special guest Chris Hymes (Head of Infosec, Riot Games)

* [**Is Governance the Most Important Part of GRC?**, *Defense in Depth Podcast*](https://podcasts.google.com/feed/aHR0cHM6Ly9kZWZlbnNlaW5kZXB0aC5saWJzeW4uY29tL3Jzcw/episode/NTI2MTAwM2MtZWIyZS00ZmIyLWJjY2UtNzk3MWVmNzhjOTE5?sa=X&ved=0CAUQkfYCahcKEwiAg7brqqnxAhUAAAAAHQAAAAAQLg) - Featuring David Spark, Allan Alford and special guest Mustapha Kebbeh (CISO, Brinks)

* [**Should Risk Lead GRC?**, *Defense in Depth Podcast*](https://podcasts.google.com/feed/aHR0cHM6Ly9kZWZlbnNlaW5kZXB0aC5saWJzeW4uY29tL3Jzcw/episode/MjMyYWUwN2EtYzcxNi00M2I5LWIyMTgtOGM1YjU0M2FjNjZm?sa=X&ved=0CAUQkfYCahcKEwiAg7brqqnxAhUAAAAAHQAAAAAQLg) - Featuring David Spark, Allan Alford and special guest Marnie Wilking (Head of Security and Technology Risk Management, Wayfair)

* [**IT Governance**, *CISO Tradecraft Podcast*](https://podcasts.google.com/feed/aHR0cHM6Ly9mZWVkLnBvZGJlYW4uY29tL2Npc290cmFkZWNyYWZ0L2ZlZWQueG1s/episode/Y2lzb3RyYWRlY3JhZnQucG9kYmVhbi5jb20vZGRkYTUyNDYtNGRjYi0zMmM5LWJmZGQtMDc0NWVmODE4NWRj?sa=X&ved=0CAUQkfYCahcKEwjItYv_qqnxAhUAAAAAHQAAAAAQIQ) - Featuring G Mark Hardy and Ross Young

* [**Cyber Frameworks**, *CISO Tradecraft Podcast*](https://podcasts.google.com/feed/aHR0cHM6Ly9mZWVkLnBvZGJlYW4uY29tL2Npc290cmFkZWNyYWZ0L2ZlZWQueG1s/episode/Y2lzb3RyYWRlY3JhZnQucG9kYmVhbi5jb20vZWEwZjlkNjEtZjc5Zi0zOWQ2LWE0ZDQtMWZhMzg3ODA5ZWU4?sa=X&ved=0CAUQkfYCahcKEwjItYv_qqnxAhUAAAAAHQAAAAAQIQ) - Featuring G Mark Hardy and Ross Young

# :scroll: Certifications

Probably [the only resource you'll need](https://pauljerimy.com/security-certification-roadmap/) for certifications. Paul Jerimy has done an incredible job with input from lots of practitioners and experts in InfoSec. If one certification had to be mentioned, it would be the CISSP for obvious reasons (:heavy_dollar_sign::heavy_dollar_sign::heavy_dollar_sign:).

# :triangular_ruler: The Knowledge Trifecta

**We are offered jobs but we have a career.** We're the only one accountable for our career path and the best way to make the best of this is to continuously learn.

This section might seem out of place for a content curation repository but I'm passionate about this, sorry.

Security is a very young field and ours is even younger. Career pathways are still developing and no one *actually* knows the sureway to a GRC leadership role or a CISO position.

The only thing that's certain is that this is the best thing that could happen to us. We can build our own paths. The only way we do this is through learning. Our field is about understanding, managing and translating. We understand the technical, manage security projects and translate into security terms business requirements.

If you're a jack-of-all-trades, love learning new things, being inquisitive but always having the business goals in mind, then it's the field for you. If you're not, it's probably the field for you anyway or you wouldn't be here!

## :floppy_disk: The Technical

Understanding the technical landscape.

How do we know GRC is being done at all?  It is measured!  Put simply, businesses collect and measure data to make decisions.  GRC broadly ensures that decision makers "appetite" for risk is being achieved.

Measurement can occur in many ways, though primarily GRC is concerned with audit.

## :lock_with_ink_pen: The Security

Understanding the security measures.

## :briefcase: The Business

Understanding the business language.

Business can be empowered by a strong, comprehensive, and adaptive GRC foundation.  GRC largely exists to support business objectives and corresponding legal (but not always) requirements.  

Some regulations are compulsory to conduct business within geographic areas - Such as Sarbanes-Oxley (SOX) for publicly traded US companies...  While some requirements are set within industry without governmental oversight (see - Payment Card Industry Data Security Standard (PCI DSS)).
