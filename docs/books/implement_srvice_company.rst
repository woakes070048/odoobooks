.. _table-of-contents::

=====================================================
The Odoo Playbook for Service & Consulting Businesses
=====================================================

**Introduction: The Strategic Foundation for Service Business Transformation**

The decision to adopt a new Enterprise Resource Planning (ERP) system is a pivotal moment for any organization. [cite: 1] For service and consulting firms, this decision carries unique weight. [cite: 2] Unlike businesses that trade in tangible goods, service firms deal in an intangible, yet highly valuable commodity: expertise, delivered over time. [cite: 3] The core challenges of this sector—accurately tracking billable hours, managing project scope and profitability, maintaining strong client relationships, and ensuring a seamless flow from sales promises to delivery realities—demand a software solution that is not merely a collection of tools, but a truly integrated ecosystem. [cite: 4] This is where Odoo presents its most compelling value proposition. [cite: 5]

This guide is architected to serve as a definitive implementation playbook for Odoo in the service and consulting industry. [cite: 6] It is intended for the Odoo implementation consultant and the forward-thinking business owner who seeks to leverage technology not just for incremental improvements, but for fundamental business transformation. [cite: 7] We will journey through the entire implementation process, from the high-level strategic decisions of methodology and project governance to the granular, hands-on configuration of Odoo's core applications. [cite: 8]

The inherent complexity of service businesses often leads to fragmented operations. [cite: 9] A sales team might use one CRM, a project team another tool for task management, and the finance department a separate accounting package. [cite: 10] This creates information silos, necessitating manual data re-entry, which is both inefficient and prone to error. [cite: 11] It becomes exceedingly difficult to answer the most critical question for any service firm: "Is this project profitable?". [cite: 12]

Odoo directly confronts this challenge by providing a single, unified platform where every business function resides. [cite: 13] The data from a sales quotation flows seamlessly to create a project, timesheets logged against that project are instantly available for invoicing, and all associated costs and revenues are automatically posted to the correct analytic accounts for real-time profitability analysis. [cite: 14] This end-to-end integration is Odoo's foundational strength for the service sector. [cite: 15]

However, adopting Odoo is more than a software installation; it is an embrace of a particular business philosophy. [cite: 16] The official Odoo implementation methodology, which will be explored in detail, champions simplicity, speed, and a disciplined approach to customization. [cite: 17] It encourages businesses to adopt standard, best-practice workflows wherever possible, rather than rebuilding inefficient legacy processes within a new system. [cite: 18] This philosophy, often called "The Odoo Way," posits that the most successful, cost-effective, and maintainable implementations are those that limit custom development to an absolute minimum. [cite: 19] A successful project, therefore, hinges not only on technical acumen but also on a strategic commitment to process re-engineering and change management. [cite: 20] The role of the implementation consultant, and the mindset of the business owner, must be one of a strategic partner willing to challenge the status quo ("Why do we do it this way?") and guide the organization toward simpler, more efficient workflows that harness the full, out-of-the-box power of the Odoo suite. [cite: 20] This book will equip you with the knowledge to fulfill that role. [cite: 21]

Chapter 1: Charting the Course - The Implementation Methodology
================================================================

Before a single module is configured or a line of data is migrated, the success of an Odoo implementation is predicated on the strategic framework chosen to govern it. [cite: 22] This chapter details the critical decisions surrounding implementation methodology, project governance, and deployment models. [cite: 23] Selecting the right approach is the first and most crucial step in ensuring the project is delivered on time, on budget, and in alignment with the business's strategic goals. [cite: 24]

Section 1.1: Choosing Your Implementation Strategy: Waterfall, Agile, or Hybrid
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The methodology dictates the rhythm and flow of the entire project. [cite: 25] Different vendors and partners adopt various approaches, with the most common being Waterfall, Agile, and a hybrid of the two. [cite: 26]

**Waterfall Methodology:** This is a traditional, linear approach where the project progresses through a series of sequential phases: Requirements, Design, Development, Testing, Deployment, and Maintenance. [cite: 27] Each phase must be fully completed before the next begins. [cite: 28] The Waterfall model is best suited for projects where the requirements are exceptionally clear, well-documented, and stable from the outset. [cite: 29] It provides a structured and predictable path but offers little flexibility to accommodate changes once a phase is complete. [cite: 30] This method is ideal if the organization has predefined workflows, finalized forms and fields, and expects very limited changes during the implementation process. [cite: 31]

**Agile Methodology (Scrum):** In contrast, the Agile methodology is an iterative and incremental approach. [cite: 32] The project is broken down into small, manageable cycles or "sprints." [cite: 33] At the end of each sprint, a potentially shippable piece of functionality is delivered. [cite: 34] This model thrives on continuous feedback from stakeholders and is highly adaptive to change. [cite: 35] It is the preferred method when requirements are expected to evolve, the organizational structure might shift, or when rapid feedback loops are critical for success. [cite: 36] This flexibility makes Agile a natural fit for many Odoo projects, as it allows for adjustments and reprioritization as the business gains a deeper understanding of the software's capabilities. [cite: 37]

**Hybrid Methodology:** A hybrid approach strategically combines the strengths of both Waterfall and Agile. [cite: 38] It uses the Waterfall model for the well-defined, stable parts of the project, such as the implementation of core, out-of-the-box modules like Odoo Accounting. [cite: 39] Simultaneously, it employs an Agile approach for the more fluid and uncertain aspects, such as custom module development or integrating with unique third-party systems. [cite: 40] This provides a predictable foundation while retaining the flexibility to adapt to evolving needs, offering a balanced path for many medium-to-large-scale implementations. [cite: 41]

The choice of methodology is not arbitrary. [cite: 42] It should be a deliberate decision based on a clear assessment of the project's context, particularly the clarity of requirements and the likelihood of organizational change during the implementation lifecycle. [cite: 42]

**Implementation Methodology Comparison**

.. list-table::
   :widths: 15 25 25 25 25
   :header-rows: 1

   * - Methodology
     - Best For
     - Key Characteristics
     - Pros
     - Cons
   * - Waterfall
     - Projects with clear, stable, and well-documented requirements. [cite: 85]
     - Linear, sequential phases. [cite: 85] Low flexibility. [cite: 85]
     - Predictable timeline and budget; clear deliverables for each phase. [cite: 85]
     - Inflexible to change; errors found late are costly to fix. [cite: 86]
   * - Agile (Scrum)
     - Projects where requirements may evolve, and continuous feedback is critical. [cite: 87]
     - Iterative cycles (sprints); high flexibility and stakeholder involvement. [cite: 88]
     - Adaptable to change; faster delivery of value; continuous feedback improves quality. [cite: 88]
     - Less predictable final scope and timeline; requires high client engagement. [cite: 89]
   * - Hybrid
     - Projects with a mix of well-defined core requirements and uncertain, evolving areas. [cite: 90]
     - Waterfall for core modules, Agile for customizations and new features. [cite: 90]
     - Provides a structured foundation with flexibility; balances predictability and adaptability. [cite: 91]
     - Can be complex to manage two different methodologies simultaneously. [cite: 91]
   * - The Odoo Way
     - SMEs and projects prioritizing speed and budget control with standard Odoo features. [cite: 93]
     - Lean, phased delivery (MVP first); strong focus on minimizing customization. [cite: 93]
     - Very fast go-live; lower cost; reduces risk of project failure; aligns with Odoo's design. [cite: 94]
     - Not suitable for highly complex or unique business processes; requires process adaptation. [cite: 94]

Section 1.2: The Odoo Way: A Lean and Focused Approach
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Odoo S.A. and its most successful partners champion a specific implementation philosophy that can be described as a lean, focused version of Agile. [cite: 43] This approach, "The Odoo Way," is built on a set of core principles designed to maximize the probability of project success by rigorously controlling the two factors that most often lead to failure: time and cost. [cite: 44] The primary objective is to get the users onboarded and using Odoo on time and within budget. [cite: 45] All other considerations are secondary. [cite: 46] To achieve this, The Odoo Way emphasizes several key practices:
    * **Minimize Custom Development:** This is perhaps the most critical principle. [cite: 46] Custom development introduces complexity, increases costs, extends timelines, and creates "technical debt" that complicates future upgrades and maintenance. [cite: 47] The default position should always be to adapt business processes to Odoo's standard functionality. [cite: 48] Customization should be reserved only for features that provide a significant, undeniable competitive advantage and cannot be achieved through configuration or third-party apps. [cite: 49]
    * **Phased Rollouts (MVP First):** Rather than attempting a "big bang" implementation of all desired features at once, the project should be divided into phases. [cite: 50] The first phase focuses on delivering a Minimum Viable Product (MVP) that covers the company's most critical, core needs. [cite: 51] This ensures a quick go-live and delivers value early. [cite: 52] Non-mandatory features and "nice-to-haves" can be sold and implemented in subsequent phases after the initial success is secured. [cite: 52] This approach builds client trust and momentum. [cite: 53]
    * **Limit Stakeholders:** To accelerate the decision-making cycle, the number of stakeholders involved in day-to-day project decisions should be kept to a minimum. [cite: 53] The ideal structure involves a single, empowered point of contact from the client side working directly with the Odoo Project Leader. [cite: 54]

This lean methodology requires discipline from both the implementation partner and the client. [cite: 55] It necessitates a focus on project success over immediate customer satisfaction, which sometimes means challenging customer demands that could jeopardize the budget or timeline. [cite: 56]

Section 1.3: Project Governance: Roles and Responsibilities
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Clear roles and responsibilities are the bedrock of effective project management. [cite: 57] A well-defined governance structure ensures clear communication channels and accountability. [cite: 58]

* **The Odoo Project Leader (Consultant Side):** In the Odoo ecosystem, this role is far more than a traditional project manager. [cite: 59] The Project Leader is a hybrid professional who acts as a project manager, business analyst, and product expert simultaneously. [cite: 60] Their responsibilities include:

    * Defining and managing the project plan. [cite: 61]
    * Challenging customer requirements to ensure they align with the project's core objectives and budget. [cite: 62]
    * Configuring the Odoo applications. [cite: 62]
    * Managing data migration. [cite: 63]
    * Writing specifications for any necessary custom development. [cite: 63]
    * Anticipating and mitigating risks. [cite: 63]

    The Project Leader is the central figure and the main point of contact for the customer throughout the implementation. [cite: 64]

* **The Customer's Single Point of Contact (SPoC):** The client must appoint a SPoC who is empowered to make decisions. [cite: 65] This individual is the counterpart to the Odoo Project Leader and is responsible for consolidating feedback from their organization, defining requirements, and ensuring the project stays on track from the client's side. [cite: 66] Projects without a dedicated and decisive SPoC are at high risk of delay due to slow decision-making and conflicting feedback. [cite: 67]

For larger or more complex projects, additional roles may be necessary:
    * **Project Director:** A senior figure who oversees the project from a higher level, managing executive expectations and strategic alignment, while the Project Leader focuses on the day-to-day implementation. [cite: 68]
    * **Steering Committee:** A formal committee composed of key decision-makers from both the client and the partner. [cite: 69] They meet periodically to review progress, decide on major priorities, and resolve high-level issues. [cite: 70]
    * **Key-Users:** Subject matter experts from different departments within the client's organization. [cite: 71] They support the SPoC by defining detailed requirements for their specific areas and are heavily involved in User Acceptance Testing (UAT). [cite: 72]
    * **Sponsor:** Typically a C-level executive (CEO, CFO) who is funding the project and has a vested interest in its strategic outcomes. [cite: 73] They are usually part of the Steering Committee. [cite: 74]

Section 1.4: Deployment Models: Odoo Success Packs vs. Partner-led Implementation
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Odoo offers two primary engagement models for implementation, each tailored to different business needs and project complexities. [cite: 74]
    * **Odoo Success Packs:** These are pre-paid packages of service hours (e.g., 25, 50, 100 hours) purchased directly from Odoo S.A.. [cite: 75] When a business buys a Success Pack, they are assigned a dedicated Odoo consultant who guides them through a rapid implementation. [cite: 75] This model is designed for a fast go-live, typically within 2 to 6 weeks, and is ideal for small to medium-sized enterprises (SMEs) with relatively standard business processes that do not require extensive customization or complex integrations. [cite: 76] The focus is on configuring Odoo's standard modules, training users on best practices, and getting the system operational quickly and at a lower cost. [cite: 77] The primary limitation is that complex workflows and significant custom development are outside the scope of a Success Pack. [cite: 78]
    * **Partner-led Implementation:** This is the traditional consulting engagement model, suitable for businesses with complex operations, unique workflows, or a need for significant customization and integration with other systems. [cite: 79] An official Odoo partner will conduct a detailed business analysis, perform a GAP analysis, design custom solutions, and manage the entire project lifecycle, often using one of the methodologies described earlier (Waterfall, Agile, or Hybrid). [cite: 80] This approach offers a much higher degree of customization and can be tailored to very specific needs, but it requires a larger investment of time and resources. [cite: 81]

The decision between a Success Pack and a partner-led project hinges on a realistic assessment of the business's complexity. [cite: 82] If the goal is a rapid deployment of standard Odoo functionality, a Success Pack is an efficient and cost-effective choice. [cite: 83] If the project involves a major digital transformation with unique process requirements, a knowledgeable Odoo partner is essential. [cite: 84]


Chapter 2: Blueprinting the Business - Process Mapping for Service Firms
=========================================================================

Before a single user is created or an application is installed, the foundation of a successful Odoo implementation must be laid through rigorous business analysis. [cite: 95] This phase is not a preliminary step but the core activity where the most value is created. [cite: 96] Rushing this stage is the most common path to scope creep, budget overruns, and a system that fails to meet user needs. [cite: 97] This chapter provides the framework for blueprinting the business by mapping its processes, identifying its pain points, and designing an optimized future state within Odoo. [cite: 98]

Section 2.1: The End-to-End View: Mapping the "Lead-to-Cash" Journey
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

To effectively implement an integrated system like Odoo, one must first understand the business as an integrated whole. [cite: 99] The "Lead-to-Cash" (L2C) or "Quote-to-Cash" (QTC) process provides the perfect end-to-end framework for this analysis. [cite: 100] It describes the entire customer lifecycle, from the initial point of contact as a lead to the final collection of payment for services rendered. [cite: 101] This holistic view cuts across traditional departmental silos and reveals the critical handoffs that are often sources of inefficiency. [cite: 102]

For a typical service or consulting firm, the L2C journey can be broken down into the following core stages:

    1.  **Lead & Opportunity Management:** The process begins with marketing efforts to generate leads and sales activities to qualify them. [cite: 103] This includes initial contact, needs assessment, and determining if there is a viable opportunity. [cite: 104]
    2.  **Quoting & Contracting:** Once an opportunity is qualified, the sales team develops a proposal or quotation, outlining the scope of services, deliverables, and pricing. [cite: 105] This stage concludes with the client's acceptance and the signing of a contract or statement of work (SOW). [cite: 106]
    3.  **Project Initiation & Planning:** This is the critical handoff from the sales team to the delivery team. [cite: 107] A project is created, resources are assigned, and a detailed project plan is developed. [cite: 108]
    4.  **Service Delivery & Execution:** The core of the business operation. [cite: 109] Consultants and specialists perform the work outlined in the contract. [cite: 109] This stage involves tracking time spent on tasks and logging any reimbursable expenses. [cite: 110]
    5.  **Invoicing & Payment Collection:** Based on the terms of the contract (e.g., fixed fee, time and materials, milestones), the finance department generates and sends invoices to the client. [cite: 111] This stage includes tracking payments and managing accounts receivable. [cite: 112]
    6.  **Post-Project Support:** After the primary project is complete, the relationship often continues through ongoing support, retainers, or ad-hoc assistance. [cite: 112] This involves managing support tickets and potentially new, smaller-scale billing cycles. [cite: 113]
    7.  **Reporting & Analysis:** Throughout and after the cycle, management analyzes data to measure key performance indicators (KPIs), such as project profitability, resource utilization, and customer satisfaction. [cite: 114]

Visually mapping these stages using tools like Business Process Model and Notation (BPMN) or even simple flowcharts is highly recommended. [cite: 115] This documentation provides a clear, shared understanding of how the business operates and highlights the interdependencies between departments. [cite: 116]

.. list-table:: L2C Stage Mapping
   :widths: 30 40 40
   :header-rows: 1

   * - L2C Stage
     - Odoo Application(s)
     - Key Function
   * - Lead & Opportunity Management
     - CRM
     - Pipeline, Lead Scoring, Activities [cite: 141]
   * - Quoting & Contracting
     - Sales, Sign
     - Quotations, Product Catalog, e-Sign [cite: 141]
   * - Project Initiation & Planning
     - Sales, Project
     - SO Confirmation to Project/Task [cite: 141]
   * - Service Delivery & Execution
     - Project, Timesheets, Expenses
     - Task Management, Time Tracking, Expense Logging [cite: 141]
   * - Invoicing & Payment Collection
     - Sales, Accounting
     - Invoice Creation, Payment Reconciliation [cite: 141]
   * - Post-Project Support
     - Helpdesk, Subscriptions
     - Ticket Management, SLA Policies, Retainers [cite: 141]
   * - Reporting & Analysis
     - All (via Dashboards)
     - Project Profitability, KPI Tracking [cite: 141]

Section 2.2: Discovery and Analysis: Uncovering Needs and Pain Points
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

With the end-to-end process map as a guide, the next step is a deep-dive analysis to understand the specifics of the client's business. [cite: 117] The goal is to move beyond a surface-level understanding and uncover the true needs, inefficiencies, and frustrations that the Odoo implementation is meant to solve. [cite: 118] This discovery process involves several key activities: [cite: 119]

    * **Requirement Gathering:** This is the systematic collection of both functional (what the system must do) and non-functional (how the system must perform) requirements. [cite: 119] Effective techniques include:
        * **Stakeholder Interviews:** One-on-one conversations with key personnel from each department (sales, project managers, consultants, accountants) to understand their daily tasks, challenges, and what they need from a new system. [cite: 120]
        * **Workshops:** Facilitated group sessions to map out processes collaboratively and resolve differing perspectives. [cite: 121]
        * **Surveys and Questionnaires:** Efficiently gather quantitative data and opinions from a larger group of users. [cite: 122]
        * **Observation:** Directly observing users performing their tasks in the existing systems to identify undocumented workarounds and pain points. [cite: 123]

    * **Pain Point Identification:** During requirement gathering, the consultant must actively listen for "pain points"—bottlenecks, redundancies, manual work, and sources of frustration. [cite: 124] Common examples in service firms include: "It takes days for the project team to get the details from a new sale," "We don't know if we're making money on a project until months after it's over," or "Consultants hate filling out their timesheets because it's too complicated". [cite: 125] These pain points become the primary targets for improvement. [cite: 126]

    * **GAP Analysis:** This is a formal exercise where the documented business requirements are compared against Odoo's standard, out-of-the-box functionality. [cite: 126] The result of the GAP analysis is a clear list of:
        * **Fits:** Requirements that are fully met by standard Odoo. [cite: 127]
        * **Gaps:** Requirements that are not met by standard Odoo. [cite: 128] For each gap, a solution must be proposed:
            * **Process Change:** Can the business adapt its process to the Odoo standard? (This is the preferred solution). [cite: 129]
            * **Configuration:** Can the requirement be met by creatively configuring Odoo's existing tools? [cite: 129]
            * **Third-Party App:** Is there a pre-built app on the Odoo App Store that fills the gap? [cite: 130]
            * **Customization:** Does this gap represent a critical business need that justifies custom development? [cite: 131]

Section 2.3: Designing the Future State in Odoo
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The analysis of the "As-Is" state is not an end in itself. [cite: 132] Its purpose is to inform the design of an optimized "To-Be" state. [cite: 133] This is not simply about replicating the old processes in a new interface; it is a chance for genuine process re-engineering. [cite: 134] The consultant should guide the client in envisioning new workflows that leverage Odoo's integrated nature to eliminate the identified pain points. [cite: 135] For example:

    * **Old Process:** A salesperson closes a deal, then manually emails a PDF of the contract to the project manager, who then manually creates a project in a separate system. [cite: 136]
    * **New Odoo Process:** A salesperson confirms a sales order in Odoo. [cite: 137] This action automatically creates a project and tasks in the Project app, assigns the correct project manager, and notifies the team—all in a single click. [cite: 138]

This future-state design involves explicitly mapping each stage of the L2C journey to the corresponding Odoo applications. [cite: 139] This creates a tangible blueprint that directly links the business requirements to the software solution, providing a clear roadmap for the configuration chapters that follow. [cite: 140]

Chapter 3: Laying the Foundation - Initial Odoo Configuration
==============================================================

With the strategic and analytical groundwork complete, the process transitions to hands-on system configuration. [cite: 141] This chapter covers the foundational settings that must be established in Odoo before any business-specific workflows can be built. [cite: 142] These initial steps ensure the system has the correct company context, user permissions, and application suite to support the service business model. [cite: 143]

Section 3.1: System & Company Setup
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This section details the configuration of the core system and company parameters. [cite: 144] These settings provide the legal and financial context for all subsequent transactions within Odoo. [cite: 145]

    * **Database Creation:** The very first step is the creation of the Odoo database. [cite: 146] The choice of hosting environment—Odoo Online (SaaS), Odoo.sh (PaaS), or an On-Premise server—should have been made during the initial planning phase based on the client's technical capabilities, customization needs, and budget. [cite: 147] Each has its own process for database creation. [cite: 148]

    * **Company Information:** Once the database is active, the primary task is to configure the company's details. [cite: 148]
        1.  Navigate to the Settings app. [cite: 149]
        2.  In the top-left corner, click on Users & Companies and select Companies. [cite: 149]
        3.  Select the default "My Company" record to edit it. [cite: 150]
        4.  Fill in all the essential information: Company Name, Address, Phone, Email, Website, and Tax ID (e.g., VAT, EIN). [cite: 150] This information will be used on all official documents, such as quotations, sales orders, and invoices. [cite: 151]
        5.  Set the company's default Currency. [cite: 152] This is a critical step that cannot be easily changed after transactions have been recorded. [cite: 152]

        .. figure:: /images/company_configuration.png
        :alt: Configuring the main company information in Odoo Settings.

        *Configuring the main company information in Odoo Settings.* [cite: 153]

    * **Fiscal Years & Chart of Accounts:** Proper financial setup is non-negotiable. [cite: 154]
        1.  Navigate to the Accounting app, then go to Configuration ‣ Settings. [cite: 155]
        2.  Under the Fiscal Periods section, ensure the Fiscal Year dates are correctly set. [cite: 156] Odoo will automatically propose a fiscal year ending on December 31st, but this can be adjusted. [cite: 157]
        3.  The most critical step is installing the correct Chart of Accounts (CoA). [cite: 158] Odoo provides pre-configured, country-specific CoA packages. [cite: 158]
        4.  In the Accounting settings, find the Fiscal Localization section and install the package that corresponds to the company's country. [cite: 159] This will install the standard accounts, taxes, and fiscal positions required for local compliance. [cite: 160] Attempting to build a CoA from scratch is highly discouraged and can lead to significant reporting and compliance issues. [cite: 161]

Section 3.2: User & Access Management
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A secure and efficient ERP system relies on a well-defined access control structure. [cite: 162] Odoo's user management allows for granular control over what each user can see and do. [cite: 163] The guiding principle should be that of least privilege: users should only have access to the information and actions necessary to perform their job functions. [cite: 164]

* **Creating Users:**
    1.  Navigate to Settings ‣ Users & Companies ‣ Users. [cite: 165]
    2.  Click New to create a user. [cite: 165]
    3.  Enter the user's Name and Email Address. [cite: 166] The email address will be their login and is used for system notifications. [cite: 166]
    4.  New users are sent an invitation email to set their password and log in for the first time. [cite: 167]

* **Configuring Access Rights:** Odoo's security model is based on User Groups. [cite: 168] Each application (e.g., Sales, Project, Accounting) comes with several pre-configured groups that correspond to different levels of access, such as "User" or "Administrator." [cite: 169] When editing a user, you will see a section for each installed application. [cite: 170] Within each application section, you can assign the user to a specific group from a drop-down menu. [cite: 171] For example, for the Sales application, the options are typically "User: Own Documents Only," "User: All Documents," and "Administrator." [cite: 172] Assigning a user to a group grants them all the permissions associated with that group. [cite: 173] This includes visibility of menus, access to records (read, write, create, delete), and the ability to perform certain actions. [cite: 174]

* **Role-Based Permission Setup:** For a service business, it is best practice to define standard roles and assign a consistent set of permissions. [cite: 175] This ensures uniformity and simplifies onboarding new employees. [cite: 176]

.. list-table:: Role-Based Permission Setup
   :widths: 20 20 25 35
   :header-rows: 1

   * - Role
     - Application
     - Access Level
     - Rationale
   * - Consultant/Employee
     - Project
     - User
     - Can see and update their assigned tasks. [cite: 176]
   * -
     - Timesheets
     - User
     - Can log their own timesheets. [cite: 176]
   * -
     - Expenses
     - User
     - Can submit their own expenses for reimbursement. [cite: 176]
   * - Project Manager
     - Project
     - Administrator
     - Can create new projects, manage all tasks, and see reporting. [cite: 176]
   * -
     - Sales
     - User: All Documents
     - Can view sales orders to understand project scope and create invoices. [cite: 176]
   * -
     - Accounting
     - Billing
     - Can create and manage customer invoices and vendor bills. [cite: 176]
   * - Salesperson
     - CRM
     - User
     - Manages their own leads and opportunities in the pipeline. [cite: 176]
   * -
     - Sales
     - User: All Documents
     - Can create and manage quotations and sales orders. [cite: 176]
   * - Accountant
     - Accounting
     - Accountant
     - Full access to all accounting functions, including chart of accounts, journal entries, and financial reports. [cite: 176]
   * - System Administrator
     - Settings
     - Administrator
     - Has access to all system settings, including user creation and app installation. [cite: 176]

Section 3.3: Installing Core Applications
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

With the foundational settings in place, the next step is to install the suite of Odoo applications that will power the service business's end-to-end workflow. [cite: 177] While Odoo offers hundreds of apps, a focused selection is key to a lean and effective implementation. [cite: 178]

Navigate to the Apps module from the main Odoo dashboard. [cite: 179] Use the search bar to find and install the following essential applications. [cite: 180] Installing a primary app often installs its dependencies automatically (e.g., installing Sales also installs Invoicing). [cite: 181]

    * **CRM:** For managing the sales pipeline, from lead generation to opportunity qualification. [cite: 182]
    * **Sales:** The core application for creating quotations and sales orders, which will serve as the trigger for project creation. [cite: 183]
    * **Project:** The central hub for service delivery, where all projects and tasks will be managed. [cite: 184]
    * **Timesheets:** Essential for tracking the time employees spend on project tasks, which is the basis for billing in a time-and-materials model. [cite: 185]
    * **Invoicing / Accounting:** While Invoicing is often sufficient for billing, installing the full Accounting app provides comprehensive financial management, including the chart of accounts, bank reconciliation, and financial reporting. [cite: 186] For any serious business, the full Accounting app is a necessity. [cite: 187]
    * **Expenses:** Allows employees to submit and get reimbursed for project-related expenses, which can then be re-invoiced to the client. [cite: 188]
    * **Subscriptions:** Crucial for any service firm that offers retainers, support contracts, or any other form of recurring service. [cite: 189] This app automates recurring billing and revenue management. [cite: 190]
    * **Helpdesk:** For managing post-project support, client inquiries, and bug reports in a structured ticketing system. [cite: 190]

By completing these foundational steps, the Odoo system is now prepared for the detailed configuration of the business-specific workflows that will be covered in the subsequent chapters. [cite: 191]

Chapter 4: From Opportunity to Engagement - The Sales & Quoting Process
=======================================================================

This chapter marks the beginning of the end-to-end "Lead-to-Cash" workflow configuration. [cite: 192] We will focus on the "Quote" portion of the process, detailing how to set up Odoo's Sales and CRM applications to manage the client acquisition and contracting phase. [cite: 193] The central and most critical element in this chapter is the Service Product. [cite: 194] Its correct configuration is the linchpin that connects the sales process with project delivery and financial accounting, enabling the seamless automation that is Odoo's hallmark for service businesses. [cite: 195]

Section 4.1: The Cornerstone: Configuring Service Products
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In Odoo, every line item on a sales order must be a "product." [cite: 196] For service businesses, these products are not physical goods but representations of the services offered. [cite: 197] The configuration of these service products acts as the "DNA" of a transaction, carrying all the necessary instructions for how a sale should be delivered, tracked, and, most importantly, billed. [cite: 198] An incorrectly configured service product will break the entire automated workflow, leading to manual workarounds and revenue leakage. [cite: 199]

To begin, navigate to Sales ‣ Products ‣ Products and click New. [cite: 200]

    * **Product Type:** The first and most fundamental setting is the Product Type, found in the General Information tab. [cite: 201] For any service, this must be set to Service. [cite: 202] This tells Odoo that the product does not have stock levels to manage. [cite: 202]

    * **Invoicing Policies:** This is the most critical setting for determining how and when a client will be billed. [cite: 203] Located in the General Information tab, this field dictates the entire invoicing workflow. [cite: 204] A service firm will typically use one of three main policies:
        * **Based on Timesheets (Time & Materials):** This is the most common policy for consulting and professional services. [cite: 205] The client is billed for the actual hours of work performed. [cite: 206] When this policy is selected, the invoice will be generated based on the hours logged in the Timesheets app for the associated project task. [cite: 207]
        * **Prepaid/Fixed Price:** This policy is used for services sold at a fixed price, such as a monthly retainer, a discovery workshop, or a fixed-scope project deliverable. [cite: 208] The full amount can be invoiced immediately upon confirmation of the sales order, regardless of the time spent. [cite: 209]
        * **Based on Milestones:** For large, long-term projects, this policy allows for progressive billing as specific, predefined milestones are completed. [cite: 210] An invoice can be created for each milestone as it is reached, ensuring a steady cash flow throughout the project's lifecycle. [cite: 211]

    * **Service Tracking (Create on Order):** This setting, located in the Sales tab of the product form, is the magic that automates the handoff from the sales team to the delivery team. [cite: 212] It tells Odoo what to do in the Project app when a sales order containing this product is confirmed. [cite: 213] The options are:
        * **Nothing:** No project or task is created automatically. [cite: 214] This is rarely used for billable services. [cite: 214]
        * **Create a task in an existing project:** This is useful for ongoing work or retainers for an existing client, where new tasks are added to a master client project. [cite: 215] A Project field will appear, requiring you to select the destination project. [cite: 216]
        * **Create a new project for the sales order:** This creates a brand-new project named after the sales order. [cite: 217] This is suitable when a single sales order represents a large, distinct project. [cite: 218]
        * **Create a project and task:** This is the most common and versatile setup. [cite: 219] It creates a new project and a new task within that project. [cite: 220] This is ideal for selling distinct service packages where each line item on the SO becomes a trackable task. [cite: 221]

**Configuration Example: "Consulting Hours" Product**

To illustrate, let's configure a standard time-and-materials consulting service: [cite: 222]

* Product Name: Consulting Services [cite: 222]
* Product Type: Service [cite: 222]
* Invoicing Policy: Based on Timesheets [cite: 222]
* Unit of Measure: Hours (ensure this is enabled in settings) [cite: 222]
* Navigate to the Sales tab. [cite: 222]
* Create on Order: Create a project and task [cite: 223]
* Sales Price: Enter the hourly billing rate (e.g., 150.00). [cite: 223]

.. figure:: /images/product_form_timesheet.png
   :alt: Configuring a service product for timesheet-based billing.
   :align: center
   :width: 80%

   *Fig 4.1: Detailed configuration of a service product for time-and-materials billing, highlighting the critical 'Invoicing Policy' and 'Create on Order' fields.* [cite: 225]

Section 4.2: Managing the Sales Funnel with CRM
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The Odoo CRM app provides the tools to manage the sales process that precedes the quotation. [cite: 225] A well-structured CRM pipeline ensures that potential deals are tracked systematically from initial interest to a successful close. [cite: 226]

    * **Pipeline Configuration:** Navigate to CRM ‣ Configuration ‣ Stages. Here, you can define the stages of your sales process. [cite: 227] A typical pipeline for a consulting firm might look like:
        * New: Initial lead or inquiry. [cite: 228]
        * Qualification: The lead has been contacted, and a potential need is identified. [cite: 229]
        * Proposition: A formal proposal or quotation has been sent to the prospect. [cite: 230]
        * Negotiation: The terms of the proposal are being discussed. [cite: 231]
        * Won: The deal is closed, and the contract is signed. [cite: 231]
        * Lost: The opportunity will not be moving forward. [cite: 232]

    * **Lead Generation and Conversion:** Odoo provides multiple channels to capture leads, including manual creation, an automated email alias (where emails sent to sales@yourcompany.odoo.com create leads), and website contact forms. [cite: 232] Once a lead is deemed to have a genuine potential for business (e.g., after an initial discovery call), it should be converted into an Opportunity. [cite: 233] This action moves the record from a simple list of leads into your active sales pipeline, where it can be tracked through the stages defined above. [cite: 234]

Section 4.3: Building and Managing Quotations
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Once an opportunity reaches the "Proposition" stage, it's time to create a formal quotation. [cite: 235]

* **Creating Quotations from Opportunities:** Odoo provides a seamless link between the CRM and Sales apps. [cite: 236] From an opportunity form, clicking the New Quotation button will create a new quote, automatically linking the customer and other relevant information. [cite: 237] This maintains a clean data trail and ensures the sales team can see all related quotes directly from the opportunity record. [cite: 238]

* **Quotation Templates:** For standardized service offerings, Quotation Templates can be a massive time-saver. [cite: 239] Navigate to Sales ‣ Configuration ‣ Quotation Templates. Here, you can create templates that pre-populate product lines, terms and conditions, and even have an expiration date. [cite: 240] This ensures consistency and dramatically speeds up the process of sending common proposals. [cite: 241]

* **Online Confirmation and Payment:** A key feature for accelerating the sales cycle is the ability for customers to confirm orders electronically. [cite: 242] When sending a quotation by email, the customer receives a link to a web version of the quote. [cite: 243] From this Customer Portal, they can review the details and, if the features are enabled (Sales ‣ Configuration ‣ Settings), they can provide an Online Signature and even make an Online Payment (e.g., a deposit) to confirm the order. [cite: 244] This action automatically converts the quotation into a confirmed sales order in Odoo, triggering the project creation workflows without any manual intervention from the salesperson. [cite: 245] This automation removes friction and delay from the most critical point in the sales process. [cite: 246]

.. figure:: /images/quotation_customer_portal.png
   :alt: Customer view of an online quotation with options to sign and pay.
   :align: center
   :width: 80%

   *Fig 4.2: The customer portal view, which allows clients to digitally sign and pay for a quotation, turning it into a sales order instantly.* [cite: 248]

By meticulously configuring service products and leveraging the integrated workflow between CRM and Sales, a service business can establish a robust, efficient, and largely automated front-end for its entire operation. [cite: 248]

Chapter 5: Delivering Excellence - Project & Task Management
================================================================

With a contract signed and a sales order confirmed, the focus shifts from acquisition to delivery. [cite: 249] This chapter details the operational heart of a service business: managing the execution of projects and tasks using Odoo's Project and Timesheets applications. [cite: 250] The seamless, automated handoff from the sales process, configured in the previous chapter, is where the power of Odoo's integration first becomes truly tangible. [cite: 251]

Section 5.1: Automating the Handoff: From Sales Order to Project
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The manual transfer of information from a sales team to a project team is a common bottleneck in many service organizations, often leading to delays, miscommunication, and incomplete project setups. [cite: 252] Odoo eliminates this friction through the automated workflow configured on the service product. [cite: 253]

* **The Automated Workflow in Action:** When a sales order containing a service product (configured with a Create on Order policy) is confirmed, Odoo automatically executes the specified action in the Project app. [cite: 254] For example, if the product "Website Design Package" was set to "Create a project and task," confirming a sales order for this product will instantly:
    * Create a new Project. [cite: 255] By default, the project will be named after the sales order (e.g., "SO00123 - Smith Corp"), but this can be changed. [cite: 256]
    * Create a new Task within that project, named after the service product on the sales order line (e.g., "Website Design Package"). [cite: 257] The task will be automatically linked to the customer and the specific sales order item, ensuring full traceability from delivery back to the sale. [cite: 258]

* **Project Templates for Standardization:** For recurring types of projects, such as a standard "SEO Audit" or "New Client Onboarding," using Project Templates can further enhance automation and ensure consistency. [cite: 259] A project template can be pre-configured with a standard set of stages and even a list of common tasks that are required for that project type. [cite: 260] When configuring a service product, you can associate it with a specific project template. [cite: 261] Upon confirmation of the sales order, Odoo will create a new project that is a complete copy of the template, with all its predefined stages and tasks ready to go. [cite: 262] This practice is invaluable for standardizing service delivery and ensuring no critical steps are missed. [cite: 263]

.. figure:: /images/project_from_so.png
   :alt: The Project and Task smart buttons appearing on a confirmed Sales Order.
   :align: center
   :width: 80%

   *Fig 5.1: After confirming a sales order with a configured service product, smart buttons provide a direct link to the automatically created project and tasks.* [cite: 265]

Section 5.2: Managing Project Execution
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Once a project and its tasks exist in the Project app, project managers and consultants have a central hub to manage the delivery process. [cite: 265]

    * **The Kanban View:** The default view for a project is a Kanban board, which provides a highly visual way to track task progress. [cite: 266] Each column represents a Stage in the workflow. [cite: 267] Project managers can easily configure these stages to match their delivery process (e.g., Backlog, To Do, In Progress, Client Review, Done). [cite: 267] Team members can then move tasks from one stage to the next via a simple drag-and-drop interface, providing an at-a-glance overview of the project's status. [cite: 268]

    * **Advanced Views for Deeper Planning:** Beyond the Kanban view, the Project app offers other powerful visualization tools:
        * **Gantt View:** Essential for planning project timelines. [cite: 269] It displays tasks on a horizontal time chart, allowing project managers to visualize task durations, set deadlines, and create dependencies between tasks (e.g., Task B cannot start until Task A is complete). [cite: 270]
        * **Calendar View:** Provides a standard calendar interface, useful for scheduling tasks and meetings with specific deadlines. [cite: 271]
        * **Map View:** For field service businesses, this view plots tasks on a map based on the customer's address, helping to plan efficient travel routes for on-site appointments. [cite: 272]

    * **Collaboration and Documentation:** Each task in Odoo serves as a mini-collaboration hub. [cite: 273] The chatter at the bottom of the task form logs all changes, allows team members to post messages, and can be used to attach relevant documents (e.g., design mockups, client feedback). [cite: 274] This keeps all communication and documentation related to a specific piece of work in one easily accessible place. [cite: 275]

Section 5.3: The Lifeblood of Billing: Tracking Time and Expenses
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

For any service business billing on a time-and-materials basis, accurate and consistent time tracking is the lifeblood of its revenue stream. [cite: 276] The Timesheets app in Odoo is fully integrated with Project, making this process straightforward for consultants and transparent for managers. [cite: 277]

    * **Recording Timesheets:** Employees can record their billable hours in several ways, ensuring flexibility and ease of use:
        * **Directly on the Task:** This is the most common method. [cite: 278] Open the specific task in the Project app, navigate to the Timesheets tab, and click Add a line. [cite: 279] The employee selects the date, provides a description of the work performed, and enters the duration in hours. [cite: 280]
        * **Using the Timesheets App:** The dedicated Timesheets app provides a weekly or monthly grid view where employees can quickly enter time against different projects and tasks. [cite: 281]
        * **With the Task Timer:** On the task form, a Start button acts as a timer. [cite: 282] Clicking it starts a real-time clock, and clicking Stop automatically creates a timesheet entry for the elapsed duration. [cite: 283]

    .. figure:: /images/task_timesheet_entry.png
        :alt: Adding a timesheet line to a project task.
        :align: center
        :width: 80%

    *Fig 5.2: The Timesheets tab on a project task, where consultants log their billable hours with descriptions of the work performed.* [cite: 285]

    * **Submitting and Approving Expenses:** Project work often involves costs beyond just time, such as travel, software licenses, or materials. [cite: 285] The Expenses app allows employees to capture these costs and link them directly to the project for accurate profitability tracking and client re-invoicing. [cite: 286] An employee creates a new expense in the Expenses app, filling in the description, amount, and attaching a receipt. [cite: 287] Crucially, they select the correct Analytic Distribution, which links the expense to the specific project's financial account. [cite: 288] If the expense is to be billed back to the client, they also select the corresponding Sales Order in the "Customer to Reinvoice" field. [cite: 289] The expense is then submitted for approval by a manager. [cite: 290] Once approved and posted, it becomes available for invoicing on the sales order. [cite: 291]

This disciplined tracking of all time and expenses within Odoo ensures that no billable work is lost and provides the raw data needed for the accurate invoicing and profitability analysis covered in the subsequent chapters. [cite: 292]

Chapter 6: Monetizing Your Services - Invoicing & Revenue Recognition
===========================================================================

This chapter closes the loop on the primary "Quote-to-Cash" process. [cite: 293] It focuses on how to leverage the data meticulously captured during project execution—the timesheets and expenses—to generate accurate, timely invoices. [cite: 294] This is where the service firm monetizes its efforts and recognizes revenue. [cite: 295] Odoo's integrated nature ensures that the invoicing process is not a separate, manual task but a direct and logical continuation of the work already performed. [cite: 296]

Section 6.1: Invoicing Based on Time & Materials
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This is the most dynamic invoicing model for service businesses, directly linking the work performed to the amount billed. [cite: 297] The setup completed in previous chapters makes this process remarkably efficient. [cite: 298]

    * **The Automated Data Flow:** As consultants log their hours in the Timesheets app against a specific task, Odoo performs a critical background action. [cite: 299] The hours recorded automatically update the Delivered quantity on the corresponding line item of the original sales order. [cite: 300] For example, if the sales order was for 20 hours of "Consulting Services" and a consultant logs 8 hours, the Delivered quantity on the SO will change to 8. [cite: 301] This provides real-time visibility of billable work directly on the sales document. [cite: 301]

    * **Creating the Invoice:** When it's time to bill the client (e.g., at the end of the week or month), the process is straightforward: [cite: 302]
        1.  Navigate to the original Sales Order. [cite: 302]
        2.  Observe that the Delivered column reflects the total hours logged and ready for invoicing. [cite: 303]
        3.  Click the Create Invoice button in the top-left corner. [cite: 304]
        4.  A pop-up window will appear. [cite: 304] Select Regular Invoice and click Create Draft Invoice. [cite: 305]
        5.  Odoo generates a draft customer invoice. [cite: 305] The invoice line will be for the quantity of hours in the "Delivered" field, not the originally ordered quantity. [cite: 306] This ensures you are billing only for the work that has actually been completed. [cite: 307]
        6.  The draft invoice can be reviewed, confirmed, and sent to the customer for payment. [cite: 308]

This workflow eliminates the need for accountants to manually collect timesheet reports and re-enter data, drastically reducing administrative overhead and the risk of billing errors. [cite: 309]

Section 6.2: Invoicing Based on Project Milestones
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

For large-scale projects, billing is often tied to the completion of specific deliverables or phases, known as milestones. [cite: 310] This approach provides predictable cash flow for the service firm and allows the client to pay in installments as they see tangible progress. [cite: 311]

    * **Reaching and Confirming a Milestone:** The project manager is responsible for tracking the progress of the project against the predefined milestones. [cite: 312] When all the work associated with a particular milestone is complete, it must be marked as "Reached." [cite: 313] This is done on the sales order by navigating to the Milestones smart button and checking the box in the Reached column for the completed milestone. [cite: 314]

    * **Invoicing the Reached Milestone:** Once a milestone is marked as reached, it becomes available for invoicing. [cite: 315]
        1.  Return to the Sales Order. [cite: 316]
        2.  Click Create Invoice. [cite: 316]
        3.  Select Regular Invoice and create the draft. [cite: 316]
        4.  Odoo will intelligently create a draft invoice that only includes the line item(s) for the milestone(s) that have been marked as reached. [cite: 317] Milestones that are still in progress will not be included. [cite: 318]

This allows the firm to issue multiple, partial invoices against a single sales order over the project's lifetime, perfectly aligning billing with project delivery. [cite: 319]

Section 6.3: Re-invoicing Expenses and Purchases
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Project-related costs, such as travel, accommodation, or specific materials purchased for the client, are often re-billed. [cite: 320] The key to automating this is the Analytic Distribution set when the expense or purchase was recorded. [cite: 321]

    * **The Automated Flow:** When an employee expense or a vendor bill is approved and posted with an analytic distribution linked to a sales order, Odoo automatically adds a new line item to that sales order. [cite: 322] The product on this new line is determined by the expense category's configuration. [cite: 323] For example, a "Hotel Stay" expense can be configured to create a "Travel Expenses" line on the sales order. [cite: 324] The cost from the original expense/bill becomes the basis for the sales price on this new line, which can be marked up if desired. [cite: 325]

    * **Invoicing the Expense:** This new line item now appears on the sales order with a delivered quantity of 1. [cite: 326] It can be invoiced along with the next batch of timesheets or as a separate invoice, simply by following the standard "Create Invoice" process. [cite: 326]

Section 6.4: Managing Recurring Revenue with Subscriptions
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Many service firms have moved beyond one-off projects to more stable, recurring revenue models, such as monthly support retainers, managed service contracts, or Software-as-a-Service (SaaS) offerings. [cite: 327] The Odoo Subscriptions app is designed specifically to manage this business model. [cite: 328]

    * **The Use Case:** The Subscriptions app automates the entire lifecycle of a recurring service, from initial sale to ongoing billing and renewal management. [cite: 329] This is ideal for any service that requires regular, periodic invoicing without manual intervention each time. [cite: 330]

    * **Configuration:** The setup involves two key components:
        1.  **Recurring Plans:** Navigate to Subscriptions ‣ Configuration ‣ Recurring Plans. [cite: 331] Here, you define the billing cycles (e.g., "Monthly," "Quarterly," "Annually"). [cite: 332] Each plan specifies the billing frequency and duration. [cite: 332]
        2.  **Subscription Products:** Create a new product (or modify an existing one) in the Sales app. [cite: 333] On the product form, ensure the Subscription checkbox is ticked. [cite: 334] This designates it as a subscription product. [cite: 334] You can then link this product to one of the recurring plans you created. [cite: 335]

    * **The Automated Workflow:**
        1.  A salesperson sells the "Monthly Support Retainer" subscription product on a sales order. [cite: 336]
        2.  When the sales order is confirmed, Odoo automatically creates a Subscription record in the Subscriptions app. [cite: 337]
        3.  This subscription record will then automatically generate a new invoice for the client at the start of each billing period (e.g., on the 1st of every month) according to the rules of the assigned recurring plan. [cite: 338]

    * **Customer Portal and Self-Service:** A significant benefit of the Subscriptions app is its integration with the customer portal. [cite: 339] Clients can be given the ability to log in and manage their own subscriptions, view past invoices, update their payment methods, and even upgrade, downgrade, or cancel their plans (depending on the configured self-service options). [cite: 340] This empowers the customer and dramatically reduces the administrative burden on the service firm's staff. [cite: 341]

Chapter 7: Ensuring Client Success - Post-Delivery Support with Helpdesk
=============================================================================

The relationship with a client does not end when the final project invoice is paid. [cite: 342] Ongoing support, whether for bug fixes, user questions, or new requests, is a critical part of the service lifecycle. [cite: 343] Managing this post-delivery phase effectively is key to client retention and can also be a significant source of revenue. [cite: 344] The Odoo Helpdesk app provides a structured, professional system for managing all client support interactions. [cite: 345]

Section 7.1: Configuring Your Support Center
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Setting up a robust support center in Odoo begins with defining the structure through which tickets will be managed and resolved. [cite: 346]

    * **Helpdesk Teams:** The first step is to create one or more Helpdesk Teams. [cite: 347] This is done by navigating to Helpdesk ‣ Configuration ‣ Helpdesk Teams. [cite: 348] Teams can be organized based on function (e.g., Technical Support, Functional Support, Billing Inquiries), client tiers (e.g., Standard Support, Premium Support), or product lines. [cite: 349] Each team has its own dedicated email alias, pipeline, and set of members. [cite: 350]

    * **Ticket Pipeline (Stages):** For each team, you must configure a pipeline of Stages that represent the lifecycle of a support ticket. [cite: 351] These are fully customizable but a typical workflow might include stages such as: New, In Progress, Awaiting Customer, Solved, Canceled. [cite: 352] This Kanban-style view gives support managers an instant overview of the team's workload and the status of every ticket. [cite: 353]

    * **Ticket Creation Channels:** Odoo offers multiple channels for customers to submit support requests, ensuring accessibility and convenience. [cite: 354] These channels can be configured per team:
        * **Email Alias:** Each Helpdesk team can have a unique email address (e.g., support@yourcompany.odoo.com). [cite: 355] Any email sent to this address will automatically create a new ticket in that team's pipeline. [cite: 356]
        * **Website Form:** A customizable form can be embedded on the company website, allowing clients to submit structured support requests directly into Odoo. [cite: 357]
        * **Live Chat:** The Live Chat feature can be used to provide real-time support, and conversations can be converted into Helpdesk tickets with a single click if the issue requires further follow-up. [cite: 358]

Section 7.2: Defining Service Levels with SLA Policies
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A Service Level Agreement (SLA) defines the commitment of service you promise to your customers, such as the maximum time to resolve a critical issue. [cite: 359] Odoo's SLA Policies feature allows you to formalize these commitments and track your team's performance against them. [cite: 360]

    * **Creating SLA Policies:** Navigate to Helpdesk ‣ Configuration ‣ SLA Policies. [cite: 361] Here you can create rules that automatically apply to incoming tickets. [cite: 362] A policy is defined by a set of criteria:
        * **Helpdesk Team:** The policy applies only to tickets in a specific team. [cite: 363]
        * **Priority:** The policy can be triggered based on the ticket's priority (e.g., High, Medium, Low). [cite: 364]
        * **Ticket Type or Tags:** You can create policies for specific types of issues, such as "Bug Report" or "Billing Question." [cite: 365]

    * **Setting Performance Targets:** The core of an SLA policy is its target. [cite: 366] This defines what must be accomplished and by when. [cite: 367] For example, a policy could state that for any ticket with a "High" priority, the team must get it to the "In Progress" stage within 4 working hours of its creation. [cite: 367] Odoo will then calculate a deadline for each ticket that matches this policy, taking the team's configured working hours into account. [cite: 368] This deadline is clearly visible on the ticket, and the system will flag tickets that are approaching or have breached their SLA, providing a powerful tool for prioritizing work and managing customer expectations. [cite: 369]

.. figure:: /images/sla_policy_config.png
   :alt: Configuring an SLA Policy in Odoo Helpdesk.
   :align: center
   :width: 80%

   *Fig 7.1: The SLA Policy form, showing criteria such as Priority and the target to reach a specific stage within a set timeframe.* [cite: 371]

Section 7.3: The Integrated Support-to-Cash Workflow
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

For many consulting firms, post-project support is not a free service but a billable one, often sold in pre-paid blocks of hours or on a time-and-materials basis. [cite: 371] Odoo's ability to integrate the Helpdesk app with Timesheets and Sales transforms the support desk from a pure cost center into a measurable and manageable revenue center. [cite: 372]

    * **Enabling Time Tracking on a Helpdesk Team:** To enable this workflow, you must activate time tracking for the relevant support team. [cite: 373]
        1.  Navigate to Helpdesk ‣ Configuration ‣ Helpdesk Teams and select the team to configure. [cite: 374]
        2.  On the team's settings page, scroll to the Track & Bill Time section. [cite: 375]
        3.  Check the boxes for Timesheets and Time Billing. [cite: 376]
        4.  When Timesheets is enabled, a Project field will appear. [cite: 376] You must select or create a project here. [cite: 377] This project will serve as the container for all timesheet entries logged against tickets in this team. [cite: 377] This is the critical link between Helpdesk and Project management. [cite: 378]

    * **The Complete Billing Workflow for Support:** Once configured, the process for billing support hours is seamless and mirrors the project billing workflow: [cite: 379]
        1.  A customer submits a ticket, which arrives in the configured Helpdesk team's pipeline. [cite: 379]
        2.  The support consultant works on the ticket. [cite: 380] They navigate to the Timesheets tab on the ticket form and log the time they spent resolving the issue (e.g., 2 hours). [cite: 380]
        3.  This timesheet entry needs to be linked to a billable sales order. [cite: 381] This can be done by selecting the appropriate Sales Order Item on the ticket form. [cite: 382] This could be a line item from a pre-sold "Support Pack" or a new time-and-materials sales order created for this specific request. [cite: 383]
        4.  The 2 hours logged on the ticket's timesheet are automatically added to the Delivered quantity on the linked sales order item. [cite: 384]
        5.  The accounting department can then navigate to that sales order and click Create Invoice to bill the client for the 2 hours of support work provided. [cite: 385]

This integrated flow provides full traceability from the initial customer request to the final payment. [cite: 386] It ensures that all billable support time is accurately captured and invoiced, preventing revenue leakage and providing clear data on the profitability of support contracts. [cite: 387]

Chapter 8: Measuring What Matters - Reporting & Business Intelligence
============================================================================

A successful Odoo implementation does more than just streamline day-to-day operations; it creates a centralized repository of high-quality data. [cite: 388, 389] The final, and arguably most strategic, step is to leverage this data to gain actionable insights into business performance. [cite: 389] This chapter explores how to use Odoo's reporting tools, from standard dashboards to custom reports, to measure what truly matters for a service and consulting business: profitability, efficiency, and client satisfaction. [cite: 390]

Section 8.1: The Bottom Line: Project Profitability Analysis
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The single most important question for any service firm is whether its projects are profitable. [cite: 391] Odoo's use of analytic accounting provides a powerful and automated way to answer this question in real-time. [cite: 392]

    * **The Power of Analytic Accounting:** At the core of Odoo's project financial tracking is the concept of Analytic Accounts. [cite: 393] When a new project is created in Odoo (especially from a sales order), the system automatically creates a corresponding analytic account. [cite: 394] This analytic account acts as a financial "bucket" or tag. [cite: 395] Every cost and every piece of revenue related to that project—sales invoices, employee timesheet costs, vendor bills for subcontractors, re-invoiced expenses—is tagged with this specific analytic account. [cite: 396] This creates a dedicated sub-ledger for each project. [cite: 397]

    * **The Project Profitability Dashboard:** This powerful tool consolidates all the financial data from a project's analytic account into a single, easy-to-understand view. [cite: 397] To access it, navigate to the Project app, open the desired project, and click on the Dashboard view. [cite: 398] The profitability report, typically on the right side, is broken down into two main sections:
        * **Revenues:** This section shows all income generated by the project. [cite: 399] It includes invoiced amounts from sales orders, milestone payments, and re-invoiced expenses. [cite: 400]
        * **Costs:** This section shows all expenses incurred to deliver the project. [cite: 401] This includes the cost of employee time (calculated from their timesheets and the hourly cost set on their employee record), costs of materials, vendor bills, and approved employee expenses. [cite: 402]

        Each section is further broken down into columns: Expected (what's on the initial orders), To Invoice/Bill (what's been delivered but not yet invoiced), and Invoiced/Billed (what has been formally invoiced or billed). [cite: 403] This provides a comprehensive view of not just past performance but also future expected revenue and costs. [cite: 404]

    * **Drill-Down for Deeper Analysis:** The profitability dashboard is fully interactive. [cite: 405] Users can click on any number (e.g., the total for Timesheet Costs) to "drill down" and see the individual records (the specific timesheet entries, vendor bills, etc.) that make up that total. [cite: 406] This allows for complete transparency and makes it easy to investigate any discrepancies. [cite: 407]

Section 8.2: Key Performance Indicators (KPIs) for Service & Consulting Firms
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Beyond individual project profitability, a healthy service business needs to track a set of Key Performance Indicators (KPIs) to monitor overall business health. [cite: 408] Odoo's integrated data model makes it possible to track these KPIs without resorting to external spreadsheets. [cite: 409]

Key KPIs for a service business include:

    * **Financial KPIs:**
        * *Project Margin:* (Total Revenue - Total Costs) / Total Revenue. [cite: 410] This is the ultimate measure of a project's profitability. [cite: 411] Found directly on the Project Profitability Dashboard. [cite: 411]
        * *Revenue Per Billable Employee:* Total Revenue / Number of Billable Employees. [cite: 412] A measure of overall team efficiency. [cite: 412] Data can be gathered from Sales and HR reports. [cite: 413]
        * *Monthly Recurring Revenue (MRR):* The predictable revenue generated from subscriptions. [cite: 413] The Subscriptions app has dedicated reports for tracking MRR, churn rate, and customer lifetime value (CLV). [cite: 414]

    * **Operational KPIs:**
        * *Resource/Employee Utilization Rate:* (Total Billable Hours Logged / Total Available Working Hours) x 100. [cite: 415] This is a critical metric for consulting firms to ensure their staff is being used effectively. [cite: 415] It is calculated using data from the Timesheets app reports. [cite: 416]
        * *Order Fulfillment Cycle Time:* The time from sales order confirmation to final project completion. [cite: 417] This measures the overall speed and efficiency of the delivery process. [cite: 418]

    * **Customer KPIs:**
        * *Customer Satisfaction (CSAT):* Odoo's Helpdesk and Project apps allow you to send automated rating surveys to clients when a ticket is closed or a project milestone is reached. [cite: 419] The results are aggregated and provide a direct measure of client satisfaction. [cite: 420]
        * *Customer Acquisition Cost (CAC):* Total Sales & Marketing Costs / Number of New Customers Acquired. [cite: 421] This helps evaluate the efficiency of marketing spend. [cite: 422]

.. list-table:: Key KPIs for Service Businesses in Odoo
   :widths: 25 35 45 25
   :header-rows: 1

   * - KPI Name
     - What it Measures
     - How to Calculate/Find it in Odoo
     - Target Audience
   * - Project Margin
     - The profitability of individual projects. [cite: 434]
     - Project app ‣ Select Project ‣ Dashboard. The margin is calculated automatically. [cite: 435]
     - Project Managers, CEO, CFO [cite: 435]
   * - Employee Utilization Rate
     - The percentage of an employee's time that is spent on billable work. [cite: 435]
     - Timesheets app ‣ Reporting ‣ By Employee. Compare billable hours to total hours. [cite: 436]
     - Head of Services, Team Leads [cite: 436]
   * - Monthly Recurring Revenue (MRR)
     - Predictable monthly income from active subscriptions. [cite: 436]
     - Subscriptions app ‣ Reporting ‣ Subscriptions. Use filters and grouping to analyze MRR, churn, and growth. [cite: 437, 438]
     - CEO, CFO, Sales Director [cite: 438]
   * - Customer Satisfaction (CSAT)
     - Client happiness with the service provided. [cite: 438]
     - Project or Helpdesk apps ‣ Reporting ‣ Customer Ratings. Based on feedback surveys. [cite: 439]
     - Head of Services, Account Managers [cite: 439]
   * - Sales Cycle Length
     - The average time it takes to close a deal from creation to 'Won'. [cite: 439]
     - CRM app ‣ Reporting ‣ Pipeline. Calculate the average duration opportunities spend in the pipeline. [cite: 440]
     - Sales Director, CEO [cite: 440]
   * - Average Time to Resolution (Helpdesk)
     - The average time it takes the support team to solve a customer ticket. [cite: 440]
     - Helpdesk app ‣ Reporting ‣ SLA Status Analysis. Analyze performance against SLA targets. [cite: 441]
     - Head of Support, Team Leads [cite: 441]

Section 8.3: Building Your Own View: Custom Dashboards & Reports
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

While Odoo provides a wealth of standard reports, every business has unique needs. [cite: 422] Odoo's flexible reporting engine and customization tools allow users to create their own views and dashboards. [cite: 423]

    * **Standard Reporting Engine:** Nearly every list view in Odoo has powerful Filters, Group By, and Favorites options. [cite: 424] Users can create complex, multi-level reports on the fly (e.g., group sales orders by salesperson, then by month) and save these custom views as "Favorites" for one-click access in the future. [cite: 425]

    * **Odoo Studio for Simple Customizations:** For users without technical coding skills, Odoo Studio is a powerful tool for making simple customizations to reports and views. [cite: 426] With Studio, you can:
        * **Modify PDF Reports:** Add or remove fields from PDF documents like quotations or invoices. [cite: 427] For example, you could add a product's internal reference to an invoice line or change the layout to make the total more prominent. [cite: 428]
        * **Customize Views:** Add new fields to list, form, or Kanban views across the system. [cite: 429]
        * **Create New Reports:** Studio allows for the creation of new, custom PDF reports based on any model in Odoo. [cite: 430]

    * **Custom Dashboards:** To get a high-level overview of the business, managers need to see KPIs from different applications in one place. [cite: 431] Odoo's dashboard functionality allows users to add reports from any app to a centralized dashboard. [cite: 432] For more advanced data visualization needs, third-party apps from the Odoo App Store, such as Dashboard Ninja, offer drag-and-drop interfaces, a wider variety of chart types, and even AI-powered insights to build sophisticated, real-time business intelligence dashboards. [cite: 433]

Conclusion: A Framework for Continuous Improvement
---------------------------------------------------

This implementation playbook provides a comprehensive, step-by-step guide for configuring Odoo to meet the specific needs of service and consulting businesses. [cite: 441] By following this structured approach—from establishing a sound methodological foundation to meticulously mapping business processes and configuring the integrated suite of applications—organizations can build a powerful platform for growth. [cite: 442]

The journey, however, does not end at "go-live." [cite: 443] The true value of an integrated ERP system like Odoo lies in its ability to provide a continuous stream of data-driven feedback. [cite: 443] The reporting and business intelligence capabilities detailed in the final chapter are not merely for historical review; they are the engine for ongoing optimization. [cite: 444, 445] By regularly monitoring project profitability, resource utilization, and client satisfaction, service firms can identify trends, make proactive adjustments, and refine their strategies. [cite: 445] The successful Odoo implementation is one that transforms the organization from being reactive to being data-driven. [cite: 446] It breaks down departmental silos, automates manual processes, and provides a single source of truth for the entire Lead-to-Cash lifecycle. [cite: 447] By embracing the principles of simplification, integration, and continuous analysis outlined in this guide, service and consulting firms can unlock new levels of efficiency, profitability, and sustained competitive advantage. [cite: 448]