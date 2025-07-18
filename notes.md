# Introduction

## The foundations of DevOps

- DevOps is a collaborative method for delivering software and systems that improves technical outcomes, business outcomes, and work environments.
- It aims to unite people with different skills and languages within technology to work together and create solutions.
- The course will teach skills and abilities to apply DevOps principles to people, processes, and technology.
- Key areas of focus will include continuous delivery, infrastructure as code, and site reliability engineering (SRE).

# 1. DevOps Basics

## What is DevOps?

- The term "DevOps" combines two traditional tech roles: **Dev**elopers (who write application code) and **Op**eration**s** engineers (who manage the systems the applications run on).
- It emerged in the late 2000s when it became clear that keeping these roles separate was inefficient.
- **Definition:** The practice of operations and development engineers working together throughout the entire service lifecycle, from design and development to production support.
- **Inclusivity:** DevOps aims to bring all specialized roles together (frontend devs, test engineers, security engineers, DBAs, etc.) to collaborate rather than work in silos.
- **Core Practice:** Operations engineers use software development techniques for systems work.
  - Code is used to create, configure, and operate systems.
  - This code is checked into source control and goes through a build, test, and deployment pipeline.
  - This is a significant change from the manual system administration of the past.
- **Why It Matters:** DevOps is proven to improve both IT and business outcomes.
  - Google's DevOps Research and Assessment (DORA) team's "State of DevOps Report" shows a large and growing gap between elite and low-performing IT teams.
  - **Elite vs. Low Performers (2021 Report):**
    - **Deployment Frequency:** 973x more frequent
    - **Lead Time for Changes:** 6,570x shorter
    - **Failure Rate:** 3x lower
    - **Recovery from Issues:** 6,570x faster
  - High-performing companies spend 22% less time on unplanned work and are twice as likely to achieve their goals.
  - Practitioners in high-performing teams are half as likely to suffer from burnout.
- **What DevOps is NOT:**
  - Not just a new name for an operations team or a job title.
  - Not one person doing every single job.
  - Not dependent on any specific tool.

## DevOps core values: CAMS

- The CAMS model, created by John Willis and Damon Edwards, defines the core values of DevOps.
- CAMS stands for: **C**ulture, **A**utomation, **M**easurement, and **S**haring.
- **Culture:**
  - "DevOps is a human problem." - Patrick Debois (coined the term "DevOps").
  - Culture is about changing human behavior and breaking down "silos" between teams with conflicting goals (e.g., Devs wanting speed vs. Ops wanting stability).
  - The goal is to create mutual understanding and focus on overall business outcomes.
- **Automation:**
  - A critical part of DevOps, but not the only part. It should not be the first focus.
  - Automation is the "accelerator" that helps unlock other benefits.
  - It replaces manual work, which is a major source of inefficiency and quality problems.
- **Measurement:**
  - The ability to observe and measure what is happening with both systems and people.
  - Metrics reveal if changes are actually leading to improvements.
  - Advised approach: Measure key outcomes across the organization, such as "mean time to restore service" (MTTR) and "cycle time," as well as business results like cost, revenue, and employee satisfaction.
- **Sharing:**
  - The heart of collaboration and DevOps.
  - Key attributes include teamwork, transparency, and collaboration.
  - Achieved through practices like documentation, pair programming, peer reviews, and mentoring.

## DevOps guiding principles: The Three Ways

- Developed by Gene Kim and Mike Orzen, "The Three Ways" are strategic principles for implementing DevOps values.
- **The First Way: Systems Thinking & The Principles of Flow**
  - Focus on the performance of the entire system, not just optimizing one part.
  - Optimizing a single component can create bottlenecks elsewhere (e.g., more app servers overwhelming a database).
  - The goal is to improve the overall flow of value from "concept to cash" by reducing handoffs and friction between teams.
- **The Second Way: Amplifying Feedback Loops**
  - Create, shorten, and amplify feedback loops within the value chain.
  - A feedback loop uses its own output to inform the next action.
  - **Example:** Finding a code bug.
    - **Fastest loop (best):** Developer's local unit tests catch it before check-in.
    - **Slower loop:** A QA team finds it, creates a ticket, and sends it back.
    - **Slowest loop (worst):** A customer finds it in production, leading to a long and costly resolution process.
  - Fast, effective feedback leads to a more efficient and higher-quality system.
- **The Third Way: A Culture of Continuous Experimentation and Learning**
  - Create a work culture that encourages learning by doing.
  - Embrace concepts like "work in progress," "if it hurts, do it more often," and "fail fast."
  - Master skills through repetition and practice, and be open to trying new things.
  - This fosters a practical focus on doing rather than just talking about doing.

## Your DevOps practice playbook

- DevOps does not have a single, highly prescriptive framework like Scrum. Instead, it relies on common patterns organized into five major practice areas.
- **The Five Pillars of DevOps:**
  1.  **Culture:** Creating a safe environment for people to learn, share, and experiment.
  2.  **Process:** Using agile and lean methods like working in small batches, limiting work in progress (WIP), and incorporating feedback loops.
  3.  **Infrastructure as Code (IaC):** Managing systems (using cloud, containers, etc.) with code for reproducibility, self-service, and rapid scaling.
  4.  **Continuous Delivery (CD):** Automating the testing and deployment of small, frequent changes to improve speed and quality.
  5.  **Site Reliability Engineering (SRE):** Applying an engineering mindset to build reliable systems and operate them with high observability and automation.
- **Key Insight:** These pillars are interdependent and must be developed together.
  - DORA research shows that high CD performance alone doesn't improve business outcomes unless combined with SRE operational excellence.
  - To build a solid DevOps foundation, you must advance all five pillars in an iterative way.

## Which DevOps tools should I use?

- The focus should always be on **"People over process over tools."** (coined by Alex Honor).
  1.  First, focus on the people and their skills.
  2.  Second, define the process around them.
  3.  Finally, select the tools that best fit the people and the process.
- There is no single "best tool," only the "best tool for you" and your specific situation. The best tools are those that enhance collaboration.
- **Guiding Principles for Choosing Tools:**
  1.  **KISS Principle (Keep It Simple, Stupid):**
      - Avoid "tool sprawl." Every tool adds overhead for learning, maintenance, security, and integration.
      - Complexity is a major problem in modern tech; too many tools can slow you down.
  2.  **Integration & Dynamic Adaptation:**
      - Tools must integrate well with each other to form a cohesive "tool chain."
      - Tools must be able to adapt to dynamic environments (e.g., changing cloud server IPs) and should have APIs for automation.
- **Final Advice:** Choose tools that fit your organization, promote collaboration, are simple, and integrate well in a dynamic environment.

## Chapter Quiz

**Question 1 of 13**

Which practice area of DevOps focuses on creating and maintaining a stable and safe environment where your people can learn, share, experiment, succeed, and even fail?

- Process
- **Culture (Correct)**
- Site Reliability Engineering
- Infrastructure as Code

**Question 2 of 13**

How would you summarize the idea behind DevOps?

- **DevOps is a partnership of all the team members involved in software development and operations. (Correct)**
- DevOps is a collaboration between the development and operations team members.
- DevOps is a software development approach that creates a linear sequential process.
- DevOps is an ever-changing process that focuses on time, deadline, and budget.
- DevOps is the practice of cloud systems administration.

**Question 3 of 13**

A plan to improve the overall throughput of a service would be best served by which DevOps principle?

- **systems thinking (Correct)**
  - _Feedback: Systems thinking requires an engineer to think about the entire system holistically._
- culture
- feedback loops
- continuous experimentation and learning

**Question 4 of 13**

Tools are chosen daily for many purposes. Which qualities should you look for in a tool before combining it into a toolchain?

- Is not too large and complicated for the task at hand
- **all of these answers (Correct)**
- Dynamically adaptable
- Easily integrates with other tools

**Question 5 of 13**

How can DevOps tangibly benefit an organization?

- It helps a company focus on a small group of problems.
- **all of these answers (Correct)**
- It allows a company to deal with high-pressure issues more efficiently.
- It helps a company improve both IT and business outcomes.

**Question 6 of 13**

What would be an example of practicing Infrastructure as Code?

- **creating and maintain systems using a software development approach instead of a manual worker approach (Correct)**
- implementing lean principles in testing and deploying software
- incorporating agile and lean product development and management techniques
- building reliability into your systems at both an application and infrastructure level
  - _Note: This is more characteristic of Site Reliability Engineering._

**Question 7 of 13**

What are the three levels of DevOps understanding?

- Requirements, deployment, and testing
- Tools, principles, and budget
- **Values, principles, and practices (Correct)**
  - _Feedback: That's right - values for what we believe, principles for how we formalize those beliefs into a detailed plan, and practices for how we put them into action._
- Values, documentation, and efficiency

**Question 8 of 13**

Why is the KISS principle important when choosing tools?

- To promote a culture of sharing
- To keep your costs down
- **Extensive complexity degrades your entire toolchain (Correct)**
  - _Feedback: Too much complexity causes your entire stack to break down, jeopardizing your goals._
- To keep technical salespeople in check

**Question 9 of 13**

Which attribute is most detrimental in a DevOps tool?

- promotes collaboration among teams
- only working in an automated manner
- only having a command-line interface
- **only having a UI-driven interface (Correct)**
  - _Feedback: UI-driven interfaces are not well suited to automation and composability._

**Question 10 of 13**

What are the four values in the CAMS model?

- CAMS: Continuous, Assimilation, Microsoft, and Scientific
- CAMS: Control, Automation, Methodology, and Sharing
- **CAMS: Culture, Automation, Measurement, and Sharing (Correct)**
- CAMS: Culture, Acculturations, Mentoring, and Society

**Question 11 of 13**

Which problem type does DevOps address?

- builds
- **business and cultural (Correct)**
  - _Feedback: DevOps promotes understanding among employees, which can lead to better business outcomes._
- automation
- time and recovery

**Question 12 of 13**

How can you implement the Third Way's idea of experimentation and learning in your work environment?

- Force your employees to return to college to learn a new programming language and new computer methodologies.
- **Allow employees to work together to try out new approaches on real projects. (Correct)**
  - _Feedback: Learning by doing is how we advance the state of the art in our organizations._
- Increase competition between the development and operational teams and reward them with incentives.
- Decrease your employees’ pay when they do not demonstrate any new languages in their coding.

**Question 13 of 13**

Accepting goals that cross organizational silos describes which core value?

- **culture (Correct)**
  - _Feedback: Culture is the "C" in CAMS. True change requires changes in approach at the people or cultural level, which then drives how you construct processes and what tools you choose._
- sharing
- automation
- measurement

---

# 2. DevOps and People: A Culture Change

## Why do we need a DevOps culture?

- IT departments are often viewed negatively within businesses due to a history of misalignment between business and technology teams.
- Friction commonly exists between internal technology groups like developers, QA, operations, security, and DBAs.
- **The "Wall of Confusion":** This metaphor illustrates the problem. Groups work in isolation and "throw" their completed work over a wall to the next team in the sequence (e.g., business to developers, developers to operations).
  - This creates one-way, unilateral handoffs that prevent the information flows and feedback loops described in The Three Ways.
- **Real-World Example (Server Provisioning):**
  - A process that took **6 weeks** for a physical server was reduced to a potential **15 minutes** by a virtualization tool.
  - However, due to existing processes (standards, tickets, documentation), the actual time to get a virtual server was still **4 weeks**.
  - This highlights how organizational processes, not just technology, can be the primary impediment.
- Modern business leaders are tech-savvy and question these inefficiencies, leading them to consider outsourcing or creating "shadow IT" departments.
- The solution is to foster a culture that aligns with The Three Ways by focusing on three key areas: **Communication, Collaboration, and Continuous Learning.**

## Communication and trust power DevOps

- A culture of communication and trust is a foundational requirement for successful DevOps. Without it, technical implementations can fail due to competing goals or misunderstandings.
- **Effective Communication:**
  - Requires a plan, not just reminders to "write documentation."
  - Establish published standards for communication channels (e.g., a specific chat channel for outages, a repository for customer information).
- **Building Trust:**
  - Communication and transparency are the primary tools for building trust.
  - **Ron Westrum's Model of Organizational Cultures:**
    - **Pathological:** Power-oriented, characterized by fear and hoarding of information.
    - **Bureaucratic:** Rule-oriented, focused on protecting turf and following protocol.
    - **Generative:** Performance-oriented, focused on the mission, with the most effective information flow. This is the goal for a DevOps culture.
  - A generative culture requires a high-trust environment where "bad news" is welcomed as a learning opportunity.
- **How to Foster Trust:**
  - **Assume Good Faith:** The biggest barrier to trust is misunderstanding due to a lack of context. Most people are trying to do a good job.
  - **Lean into Communication:** When confronted with frustration, use it as an opportunity to share context and create shared goals, rather than fighting back.
  - **Be Transparent:** Let others see your work (wikis, code, monitoring tools). People fear what they don't understand. Challenge "least privilege" justifications that unnecessarily restrict information flow.
  - **Be Curious and Respectful:** Work to understand other teams' perspectives to align your goals with theirs.

## Collaboration: Break silos in case of DevOps

- Collaboration towards a common goal is the "secret sauce" of DevOps.
- The "wall of confusion" is often caused by institutional problems, not just poor people skills.
  - **Conflicting Incentives:** Development teams are often incentivized for speed and change, while operations teams are incentivized for stability. This is an example of **local optimization** hindering **global optimization**.
- **Conway's Law:** States that systems an organization designs will mirror its communication structure. If your organization is siloed, your systems will be too.
- **Important:** Simply renaming an operations team to "DevOps" does not solve the underlying structural problem and will not lead to improvement.
- **A Three-Step Path to Enhancing Collaboration:**
  1.  **Eliminate Silos with Cross-Functional Teams:** Embed specialists (e.g., an ops engineer) directly into product or development teams. The team shares a single backlog and common business goal, which builds respect and shared responsibility.
  2.  **Use Self-Service:** Create automated, self-service tools and platforms (e.g., a portal to provision cloud resources). This eliminates handoffs and wait times, effectively removing other teams as blockers.
  3.  **Align Goals and Promote Shared Responsibility:** For teams that must remain separate, ensure their goals are aligned. Roles must evolve; for example, developers may take on-call duties, and operations engineers may shift to building platforms and providing guidance.

## Continuous learning the DevOps way

- This practice area is directly related to The Third Way: creating a culture of continuous experimentation and learning.
- **Kaizen:** A Japanese concept from the Toyota Production System (TPS) meaning "change for the better" or **continuous improvement**.
  - It is a process that encourages everyone to look for ways to improve their job through small, iterative changes as part of their daily work.
- **Five Guiding Principles of Kaizen:**
  1.  Know the customer.
  2.  Enable smooth workflow.
  3.  Go to the **Gemba** (the "real place" where work happens or problems occur).
  4.  Empower people.
  5.  Maintain transparency.
- **Gemba:** The practice of going to see the problem or process firsthand instead of relying on reports or secondhand information.
- **The Kaizen Improvement Cycle (Kata): Plan, Do, Check, Act (PDCA)**
  - **Plan:** Define what you intend to do and what you expect the results to be.
  - **Do:** Execute the plan.
  - **Check:** Measure and analyze the results.
  - **Act:** If the change was an improvement, it becomes the new baseline. The cycle repeats.
- The PDCA cycle is a tactical version of the scientific method. Its purpose is not only to generate improvements but also to teach critical thinking skills ("building people before building cars").

## Chapter Quiz

**Question 1 of 8**

What is the single biggest impediment to building trust inside a DevOps organization?

- extroverted managers
- renaming teams
- **conflicting goals (Correct)**
  - _Feedback: Having conflicting goals means there are misunderstandings within the organization, so sharing information is discouraged._
- higher-priority work

**Question 2 of 8**

What ends up resulting in more effective information flows in your organization?

- **Focusing on the overall mission (Correct)**
  - _Feedback: Focusing on the mission results in a generative organizational culture, which sports the healthiest communication paths._
- Everyone keeping to their own concern
- Keeping to your team's charter
- Communicate widely about everything
  - _Feedback: Completely lacking focus in communication causes thrash and distraction in your organization._

**Question 3 of 8**

Let’s say you want to employ the Kaizen cultural practice in your company. What are the four main factors in the Kaizen cycle?

- plan, design, review, and launch
- **plan, do, check, and act (Correct)**
- plan, don’t do, lie, and act
- plan, analyze, design, and implement

**Question 4 of 8**

How can you have a team facilitate a value flow without having to directly participate in it?

- Stay in their silo
- Obey Conway's Law
- Align their goals with other teams
- **Provide self-service tooling (Correct)**

**Question 5 of 8**

What does gemba emphasize?

- discussing processes to create value
- **examining where value is created (Correct)**
  - _Feedback: Kaizen emphasizes going right to the source where value is being created._
- reporting where value is created
- developing metrics to create value

**Question 6 of 8**

Companies need to tear down the **\_** since it causes disunity and disharmony between the development and operations departments, instead of allowing them to collaborate collectively and align goals or objectives.

- Chaos Monkey
- Andon Cord
- Status page
- **Wall of Confusion (Correct)**
  - _Feedback: Wall of confusion is a wall that blocks cooperation and a open line of communication between the operations and development teams._

**Question 7 of 8**

Suppose your dev team has frequent issues with an ops team in your company. Blame is often tossed around between both groups. How would you solve this issue?

- Increase competition between both groups by offering a monetary award for being “the most patient group.”
- Remove the one individual from each team who is causing the most chaos and assign them training in social skills.
- Make each group read an article on diverse technology terminologies and have a review session over the article in a separate meeting.
- **Embed Ops engineers in your development teams, assign both teams to be in one chat room, and allow them to read each other's source code. (Correct)**

**Question 8 of 8**

How could you contribute to the wall of confusion?

- having a development team perform production support
- having a network engineer examine application code
- **releasing code that can only be maintained by one person (Correct)**
  - _Feedback: Code maintained by just one person fosters misunderstanding within the team, and can lead to testing failures._
- making frequent revisions to the code

---

# 3. DevOps and Process: The Building Blocks

## DevOps process building block: Agile

- The DevOps movement has its roots in the Agile community. It began when Patrick Debois and Andrew Clay Schaeffer discussed "Agile Infrastructure" at the Agile 2008 conference.
- **Waterfall Model:** The traditional Software Development Lifecycle (SDLC) approach.
  - **Process:** Requirements -> Design -> Implementation -> Testing -> Deployment -> Maintenance.
  - Each phase is completed fully before the next one begins, with work "thrown over the wall" to the next team.
  - **Problems:** Slow feedback loops, loss of context at each handoff, leads to finger-pointing and rigid processes.
- **Agile Model:**
  - Performs the same SDLC steps but in **small, rapid iterations**.
  - Instead of one large delivery, it produces frequent, interim deliverables of working software.
  - Emphasizes active collaboration between all teams, including end-users.
  - **Benefits:**
    - 85% see increased productivity.
    - 80% report faster time to market.
    - 81% have better delivery time predictability.
    - 79% see enhanced software quality.
- **Agile's Shortcoming:** The original Agile Manifesto focused on developers delivering "working software" but did not include **operations** or the systems/infrastructure part of the equation.
- **DevOps and Agile:**
  - DevOps is not the same as Agile, but it can and should be implemented as an **extension of Agile**.
  - DevOps brings the operations and systems work into the iterative, collaborative Agile framework.

## DevOps process building block: Lean

- Lean is a systematic process for **eliminating waste**, originally from the Toyota Production System (TPS).
- It was adapted for tech in books like Eric Ries' "Lean Startup" (Build, Measure, Learn loop) and Mary and Tom Poppendieck's "Lean Software Development."
- **Fundamental Philosophy:** Distinguish between activities that add value and those that don't (waste).
- **Three Major Types of Waste (from Japanese):**
  - **Muda:** Unnecessary effort or activities that don't add value.
  - **Muri:** Waste from overburdening people or systems.
  - **Mura:** Waste from unevenness or irregularity in flow (e.g., delays).
- **Seven Wastes in Software Development (Poppendiecks):** Includes things like bugs, delays, and building features that aren't needed. An eighth waste, "management activities," was added as an example of necessary but non-value-add work (muda type one).
- **Key Lean Techniques:**
  - **Kaizen:** Continuous improvement.
  - **Value Stream Mapping:** Analyzing the entire "concept to cash" pathway to identify waste.
  - **Visual Management:** Using tools like Kanban boards to make work and its flow visible.
  - **Work-In-Progress (WIP) Limits:** Restricting the number of active tasks to improve flow and reduce waste.
- **Lean's Role in DevOps:**
  - Lean's relevance was quickly recognized, leading Jez Humble to propose adding "L" for Lean to the CAMS acronym, creating **CALMS**.
  - Lean principles are a formative part of The Three Ways of DevOps.
  - DORA research has confirmed that Lean management and product development techniques are statistically significant predictors of high performance.

## DevOps process building block: Visible ops change control

- **Premise:** Change is the single biggest cause of IT service outages (around 80%).
- **Traditional Approach (ITSM/ITIL):**
  - IT Service Management (ITSM) frameworks like the IT Infrastructure Library (ITIL) were created to manage this chaos.
  - However, traditional ITIL implementations often create very slow, heavy-handed change management processes.
  - This typically involves extensive documentation and a central "Change Advisory Board" (CAB) that is slow and disconnected from the technical details of a change.
- **The Visible Ops Approach:**
  - Gene Kim's book, "The Visible Ops Handbook," studied high-performing IT organizations and found they used **lightweight, fast, and repeatable change control**.
  - This approach is a key part of DevOps and is proven by DORA research to improve performance and reduce burnout.
- **What Lightweight Change Control Looks Like:**
  1.  **Peer Review:** Most changes are reviewed and approved by another technologist on or close to the team. High-risk changes can be escalated, but the bulk of changes flow smoothly.
  2.  **Small Batch Sizes:** Keep changes as small as possible. This makes them easier to review, test, and troubleshoot if something goes wrong.
  3.  **Early, Automated Testing:** Use Continuous Integration (CI) systems to automatically test every change, providing objective validation. Security safeguards can also be built into this early stage.
- **Conclusion:** Agile, Lean, and lightweight Visible Ops change control are the three core process building blocks that form the foundation of DevOps.

## Chapter Quiz

**Question 1 of 5**

Which software development methodology is discouraged by the DevOps approach?

- **waterfall (Correct)**
  - _Feedback: The DevOps approach aligns more with Agile than waterfall delivery, focusing on small, frequent delivery of value._
- ITIL
- lean
- scrum

**Question 2 of 5**

DevOps is an extension of **\_** infrastructure in which its process is **\_**.

- Spiral Model; business-focused
- Waterfall; consuming
- **Agile; iterative (Correct)**
  - _Feedback: DevOps has roots in Agile and the process are iterative which generates quick product or solution delivery._
- Rapid Application Development (RAD); end-user centric

**Question 3 of 5**

Which term in Lean identifies waste that does not add value?

- **muda (Correct)**
  - _Feedback: The term muda means major waste in Japanese and describes activities that consume effort but do not create customer value in the product._
- majime
- mura
- maiko

**Question 4 of 5**

Let’s say your colleague wants to know more about the central tenet of Lean. How would you explain it to them?

- The purpose of lean is to devalue products according to the amount of “waste” associated with the product.
- The purpose of lean is to undertake product development in quick, iterative sprint cycles.
- The objective of lean is to focus on the manufacturer’s needs more than on customers’ satisfaction.
- **The objective of lean is to ensure that value stream reaches the customer through products and services while eliminating waste. (Correct)**

**Question 5 of 5**

Why are peer reviews the most effective means of review for most changes?

- They reduce the cost of reviewing changes.
- They aren't; you should always have a manager review any change.
- They eliminate the risk of making changes.
  - _Feedback: Nothing removes all risk from changes; the best you can do is reasonably mitigate that risk via review and have other safeguards like testing to further reduce it._
- **They are performed quickly, in a distributed fashion, by people familiar with the system being changed (Correct)**
  - _Feedback: Peer reviews are optimal for the vast majority of changes that aren't explicitly risky or cross-technology._

---
# 4. Infrastructure as Code

## What is infrastructure as code?

- **Infrastructure:** The underlying hardware and software layer of systems, including servers, storage, networks, and operating systems.
- **Traditional Approach (Manual):**
    - Infrastructure was installed and configured manually.
    - Each system was unique, like a "special snowflake," making administration slow, error-prone, and difficult to reproduce.
- **Code Approach:**
    - Code is written, stored in version control, and run through automated build and test systems.
    - The result is a single, standardized artifact that can be deployed identically across thousands of systems.
- **Infrastructure as Code (IaC) Definition:** The practice of provisioning and managing your infrastructure through writing automation code instead of performing manual processes.
    - This is made possible by **programmable infrastructure** (virtualization, cloud APIs, etc.).
- **Mindset Shift:** The biggest challenge is moving from a mindset of manual actions to a full software development lifecycle approach for infrastructure.
- **Why IaC is Essential:** The complexity, scale, and ephemeral (temporary) nature of modern systems (cloud, containers, microservices) make manual management impossible.
- **"Cattle, not pets":** A core DevOps philosophy where servers are treated as a managed herd, not as unique, handcrafted individuals. They can be replaced easily rather than being nursed back to health.

## DevOps applications of infrastructure as code

- **Configuration Management (CM):** The overall process for creating and maintaining systems and software in a desired, consistent state. In DevOps, this is driven by code.
- **Three Pillars of Automated CM:**
    1.  **Provisioning:** Making the underlying computing infrastructure (hardware, OS, network) ready for operation.
    2.  **Deployment:** Automatically installing and upgrading application software on the provisioned systems.
    3.  **Orchestration:** Performing coordinated operations across multiple systems (e.g., rolling deployments, automated failover).
- **Key CM Concepts and Terms:**
    - **Imperative (Procedural):** Defines the specific *commands* to execute to reach a state. (e.g., "Run this command, then copy this file, then start this service").
    - **Declarative (Functional):** Defines the *desired end state*, and the tool determines the necessary steps to get there. (e.g., "This server should be running Nginx version 1.24").
    - **Idempotent:** The ability to run the same operation multiple times and always end up in the same state without causing errors. Declarative tools are typically idempotent by nature.
    - **Self-Service:** The ability for an end-user to initiate an automated process (e.g., provision a new environment) without requiring manual intervention from an operations team.
    - **Drift:** When the actual configuration of a running system no longer matches the state defined in its code. **Drift detection** is the process of identifying this mismatch.

## Configuration management: From golden image to foil ball

- This section covers the historical evolution of configuration management tools and approaches.
- **Early Days (pre-DevOps):**
    - Manual processes and simple cloning tools like Ghost.
    - Large, complex enterprise suites like Tivoli and HP.
- **First Wave of IaC (2000s):**
    - Declarative tools like **CFEngine**, **Puppet**, and **Chef** gained popularity.
    - These tools promoted a "stem cell" approach: start with a minimal base OS image and use the CM tool to configure the rest.
    - The tool would then run incrementally to prevent configuration drift.
- **The "Golden Image or Foil Ball" Debate:**
    - Puppet founder Luke Kanies argued that using only pre-built "golden images" led to image sprawl and unmanageable configuration drift. The declarative, incremental approach was positioned as the solution.
- **Limitations of Early CM Tools:**
    - They used a "pull" model, where each server acted independently. This made **orchestration** of multi-server application deployments very difficult.
    - They primarily solved problems for system administrators, not the entire development and deployment value stream.
- **Second Wave of IaC (2010s):**
    - Tools like **Ansible** and **SaltStack** emerged, using a "push" mechanism for more explicit orchestration.
    - These tools could define workflows (e.g., update the database, then do a rolling update of the web servers).
    - Self-service orchestration tools like **Rundeck** also arose to provide a controlled way for users to run these automated workflows.

## Automating infrastructure, containers, and platforms

- This section describes the shift to modern IaC practices.
- **Rise of Cloud Computing:** Provided APIs to create and manage not just the OS, but the entire infrastructure (servers, networks, storage) with code.
    - **Model-Driven Provisioning Tools:**
        - **Cloud-Native:** AWS CloudFormation, Azure ARM Templates (declarative templates).
        - **Multi-Cloud:** Terraform, Pulumi (use a common DSL).
        - **Pure Code:** Python's Boto3, AWS CDK (use a general-purpose programming language).
- **Rise of Containers (Docker):**
    - Accelerated a shift back towards an image-based model, but with a key difference.
    - **Immutable Infrastructure:** Instead of configuring a running server, you build a new, complete image (a "golden image" container or VM) and replace the old one entirely. You do not change infrastructure once it is deployed; you replace it.
- **Container Orchestration Platforms:**
    - Systems like **Kubernetes** and **Mesos** were developed to solve provisioning, deployment, and orchestration in a single, unified platform.
    - Users define the desired state in templates, and the platform handles the complex work of making it a reality.
- **Serverless and Platform-as-a-Service (PaaS):**
    - These offerings abstract away even more of the infrastructure, allowing teams to focus almost entirely on application code.

## Your DevOps infrastructure as code toolchain

- When building a toolchain, remember to:
    1.  Pick the right tools for your **team and situation**.
    2.  **Keep it simple (KISS)**.
    3.  Design the **toolchain** as a whole, not just pick individual tools.
- **Key Decisions for Your Toolchain:**
    1.  **Infrastructure Provisioning:** Will you use a template-driven tool (CloudFormation), a multi-cloud DSL (Terraform), or a pure code library (CDK)?
    2.  **System Management:** Will you use runtime configuration (Ansible, Puppet) or "bake" immutable images (using a tool like **Hashicorp Packer**)? You can also combine these methods.
    3.  **Orchestration:** Will this be part of your CM tool (Ansible), a platform feature (Kubernetes), or an external runbook tool (Rundeck)?
    4.  **Application Deployment:** Will you use CM tools, immutable deployments, or a dedicated CI/CD system?
    5.  **Testing Strategy:** This is critical. Use the testing frameworks available for your chosen IaC tools to unit and integration test your infrastructure code.
- **Example Toolchains:**
    - A **complex SaaS** might use Terraform for infra, Puppet/Packer for baking images, and Rundeck for orchestration.
    - A **simpler system** might just use CloudFormation for infra and Dockerfiles to build containers deployed to a managed service like AWS ECS or Fargate.
- The right toolchain depends on the technical and business requirements of the service you are building.

## Chapter Quiz

**Question 1 of 9**

Certain companies utilize immutable deployment, in which changes to the system are _____ as opposed to _____.

- updated; replaced
- Agile; Waterfall
- **replaced; updated (Correct)**
- blue; green

**Question 2 of 9**

Why is orchestration an important part of configuration management?

- **Online services require careful sequencing of changes to maintain uptime while upgrading applications. (Correct)**
- It's not, if you want orchestration you don't fully understand configuration management.
- To create repeatable provisioning processes that can be checked into source control.
    - *Feedback: That's infrastructure as code in general.*
- It makes releases faster.

**Question 3 of 9**

What is the primary reason to bake images instead of performing runtime configuration?

- To make configuration management simpler
- To avoid contributing to the heat death of the universe
- To remove flexibility from runtime
- **To move time and risk up into the development and build cycle and out of the production deployment cycle (Correct)**

**Question 4 of 9**

Which of the following explains the concept of containers?

- Containers are applications that orchestrate the deployment of virtual systems.
- Containers are virtualized applications that can be shipped from server to server as needed.
- Containers are iterative backups that can be rapidly deployed in case of system failure.
- **Containers are stand-alone software packages that contain runtime components to function independently. (Correct)**

**Question 5 of 9**

Suppose you and your project manager are interested in the infrastructure as code approach. What is the chief issue that your team may face when utilizing the infrastructure as code approach?

- There are no impediments to employing the infrastructure as code in your system.
- Handling the system as a code instead of deploying systems manually.
- Custom configurations may overwhelm your version control system.
- **The mindset and habits of your team members. (Correct)**

**Question 6 of 9**

What is the benefit to a purely code driven infrastructure provisioning tool?

- **It gives you the most flexibility in what you implement (Correct)**
    - *Feedback: That's right - it's harder and more complex and more costly, but the sky's the limit on what you can do.*
- It provides higher reliability than template based solutions
- It requires less sophisticated technical skills to implement
- It is inherently idempotent

**Question 7 of 9**

You spin up a system from code, but a week later the hosts file has changed. This is an example of what?

- Orchestration
- Idempotence
- **Drift (Correct)**
    - *Feedback: Drift is when your system changes from its intended and defined state.*
- Sabotage

**Question 8 of 9**

Why is infrastructure as code a better approach than making manual changes?

- **It's more repeatable and testable. (Correct)**
- Developers are smarter than operations engineers.
- It can leverage AI more effectively.
- It's faster to get some initial infrastructure in place.

**Question 9 of 9**

What is it called when you install applications on a system?

- Provisioning
- Configuration Management
- Orchestration
- **Deployment (Correct)**
    - *Feedback: Deployment is installing and upgrading applications on a system.*

---

# 5. Continuous Delivery


## What is continuous delivery?

- **Three Key Stages of Software Delivery:**
    1.  **Build:** Compile and unit test code, turning it into a software artifact.
    2.  **Deploy:** Take the artifact, run it in an environment, and perform further testing.
    3.  **Release:** Make the software available to end users, typically by deploying it to a production environment.
- **Old Way vs. New Way:**
    - **Old Way:** Large, complex integration builds and long testing phases happen only at major milestones. This is slow, error-prone, and wasteful.
    - **New Way (DevOps):** Build, deploy, and release with every small change a developer makes.
- **Key Definitions:**
    - **Continuous Integration (CI):** The practice of automatically building and unit testing the entire application on every source code check-in, ensuring the application is **always in a working state**.
    - **Continuous Delivery (CD):** The practice of deploying every change to a production-like environment and performing automated integration and acceptance tests, ensuring the application is **always release-ready**. (CI/CD refers to the combination).
    - **Continuous Deployment:** The practice of automatically releasing the application into its production environment after all automated testing has passed.
- **Why CI/CD Matters (The Benefits):**
    - **Speed (The First Way):** Optimizes the end-to-end flow, decreases the time it takes to deploy a change, and allows for rapid experimentation. High performers deploy in under an hour, while low performers take 1-6 months.
    - **Higher Quality:** Despite the speed, CI/CD leads to a *lower* change failure rate. This is because changes are small and tested early and individually, rather than in large, complex batches.
    - **Fast Feedback Loops (The Second Way):** CI provides immediate feedback on code quality, allowing issues to be found and fixed quickly. This drives up both quality and velocity.
    - **Reduces Waste (Lean Principle):** Code that is written but not delivered is "Work in Progress" (WIP), which is a form of waste that generates risk.
    - **Faster Recovery from Failures (MTTR):**
        1.  It's easier to find the source of a failure because only one small change is deployed at a time.
        2.  A bug fix is treated like any other change and can be rolled out quickly through the same trusted CI/CD pipeline.

## Six practices for continuous integration

- Think of CI/CD as a pipeline: `Build -> Deploy -> Release`. The build stage, powered by Continuous Integration, is the first step.
- A CI system automatically triggers a build on every commit, builds the entire codebase, runs all tests, and packages an artifact. A broken build blocks the entire team.
- **Six Practices for Successful CI:**
    1.  **Builds should run quickly:** The build should pass the "coffee test" (under 5 minutes). Long builds encourage developers to batch changes, increasing WIP.
    2.  **Commit small changes:** Small commits are easier for the team to understand and make it easier to isolate the cause of a failure.
    3.  **Don't leave the build broken:** A broken build blocks delivery for everyone. Fixing it should be the team's highest priority. This is a crucial cultural practice.
    4.  **Use a trunk-based development flow:** This is a hallmark of high-performing teams. Developers commit small changes directly to the main line ("trunk") multiple times a day, avoiding long-running, complex feature branches. Incomplete features can be hidden behind **feature flags**.
    5.  **Don't allow flaky automated tests:** Tests that sometimes pass and sometimes fail for no reason erode trust in the CI system and must be fixed.
    6.  **The build should return a status, a log, and an artifact:**
        - **Status:** A simple pass/fail (red/green).
        - **Log:** A detailed record for troubleshooting and compliance.
        - **Artifact:** The versioned, installable application package that is ready for deployment.

## Five practices for continuous delivery

- After a successful build, a deployment stage deploys the artifact to a production-like environment (e.g., staging, pre-production) for further automated testing.
- **Five Practices for Successful CD:**
    1.  **Use one build artifact for all environments:** The artifact is built once and then promoted through the pipeline. You don't rebuild it for staging or production. This ensures that what you tested is what you release.
    2.  **Make the artifact immutable:** The artifact should not be allowed to change after it's created. This builds trust (everyone is looking at the same bits) and ensures auditability (a clear trace from code to production).
    3.  **Pre-production environment must be identical to production:** The test environment should be a complete clone of production, including load balancers, network settings, and security controls, to ensure both the code and the deployment process will work correctly.
    4.  **Stop the pipeline on any failure:** If any stage of the pipeline fails (e.g., deployment to staging), the entire process must stop. This optimizes for the overall flow of quality software, not for individual convenience.
    5.  **Deployments must be idempotent:** No matter how many times you run the same deployment, you must get the exact same resulting system. This can be achieved with immutable packaging (like Docker) or configuration management tools.

## The role of QA in DevOps

- The "catch" for successful CI/CD is a robust **automated testing strategy**.
- The role of QA professionals shifts from manual testing to helping design and write automated tests alongside developers.
- **The Test Pyramid (from fastest to slowest):**
    1.  **Unit Testing:** Written by developers to validate individual functions. They are fast and run locally.
    2.  **Code Hygiene:** Using tools like linters and formatters to check code for best practices.
    3.  **Integration Testing:** Testing components and dependencies working together in a full test environment.
    4.  **Acceptance/End-to-End Testing:** Testing the entire product from a user's perspective, often at the UI level. This should also be automated (e.g., using Selenium, Cypress).
- **Key Development Practices for Testing:**
    - **Test-Driven Development (TDD) / Behavior-Driven Development (BDD):** The practice of writing the test *before* writing the code. This ensures a comprehensive test suite is built as part of the development process.
- **Handling Slow Tests:**
    - Slow tests (e.g., browser compatibility, large compliance suites) cannot be ignored.
    - **Strategies:**
        1.  Run slow tests in parallel in the pipeline so they don't block the main flow.
        2.  Use scheduled testing (e.g., a nightly test run).
        3.  Run them continuously against a test environment.
    - The goal is to balance the *cost of delay* versus the *cost of bugs*.

## Continuous deployment: The final frontier

- Continuous Deployment (automatically releasing to production) is the final step, but it is **optional**. Some organizations may prefer a manual release step.
- With good CI/CD and feature flags, continuous deployment can be done safely.
- **Crucial Rule:** Your production release procedure, however complex, **must be replicated exactly in your test environment**. An untested release process is a major risk.
- **Common Production Release Patterns:**
    - **Rolling Deployment:** Upgrading one server at a time in a multi-server environment.
    - **Blue-Green Deployment:** Creating a complete new "green" environment and then switching traffic over from the old "blue" one.
    - **Canary Deployment:** Releasing a change to just one or a few servers to monitor its behavior under real load before a full rollout.
    - **A/B Deployment:** Using feature flags to release new features to a specific subset of users for testing or beta access.
- Your choice of deployment pattern depends on your software architecture, infrastructure, and packaging choices, and requires collaboration across teams.

## Your DevOps CI toolchain

- To design a toolchain, think in layers like an **onion**, starting from the desired end state (the outside) and working inward.
- **The Layers of the Toolchain Onion (Outside-In):**
    1.  **Deployment (Outermost Layer):** How will the software be used? (e.g., A/B, Rolling). This decision drives tooling needs (e.g., feature flagging tools like LaunchDarkly, orchestration in Kubernetes or Ansible).
    2.  **Artifact Repository:** Where versioned, immutable artifacts are stored (e.g., Artifactory, Nexus, a cloud container registry, or even just S3).
    3.  **Build and Test:** The collection of tools that validate the code.
        - **Unit/Integration Testing:** Language-specific frameworks (Pytest, TestNG).
        - **Acceptance/E2E Testing:** Selenium, Cypress, Postman.
        - **Specialty Testing:** Infrastructure (InSpec), Performance (JMeter), Security (Dependabot, StackHawk).
    4.  **Build System:** The engine that runs the pipeline and executes the tests (e.g., Jenkins, GitHub Actions, CircleCI).
    5.  **Version Control (Center):** The source of truth for all code (e.g., Git, hosted on GitHub, GitLab, or Bitbucket).
- **Key Metric:** Measure and actively work to improve your **overall cycle time**—the time from a code commit to it running in production.

## Chapter Qui

**Question 1 of 14**

_____ describe when software is deployed quickly into production since the team members make sure the application goes through complete automated testing.

- Blue-green deployments
- Values
- Autonomous teams
- **Continuous deployments (Correct)**

**Question 2 of 14**

Which single metric is most indicative of your CI toolchain's health over time?

- **Overall cycle time (Correct)**
    - *Feedback: That's right. A fast overall cycle time promotes healthy behavior from developers and gets fast feedback.*
- Builds completed per day
- Percentage of failed builds
- Number of unsuccessful release candidates before one passes all the tests

**Question 3 of 14**

Jenkins is an example of _____.

- **a build system (Correct)**
- a version control tool
- a status page generator
- a security monitoring tool

**Question 4 of 14**

Which task becomes easier when code is maintained in the cloud?

- **having similar preproduction and production environments (Correct)**
    - *Feedback: Having similar preproduction and production environments is made easier by using containers.*
- smoke testing a new release
- identifying automation that can be removed
- conducting audits on the codebase
    - *Feedback: This is a content management activity that is usually done on a centralized server.*

**Question 5 of 14**

Artifacts should be _____.

- **built once and deployed as needed (Correct)**
- ignored in favor of build logs
- built several times, changed, and deployed in one environment not several
- sorted by numerically by hash value

**Question 6 of 14**

Suppose some of your tests are slow. Which procedures should you select to handle a slow test?

- Utilize time-scheduled testing.
- Apply monitoring to complete some test objectives.
- Employ a non-blocking test.
- **all of these answers (Correct)**

**Question 7 of 14**

What is the goal for every phase of the continuous delivery process?

- Allow code inspections to be performed regularly.
- Use a mix of off-the-shelf and custom tools.
- **Provide early and rapid feedback (Correct)**
    - *Feedback: By making and validating small changes as soon as they are made, including deploying and using them in a real production environment, you can reduce waste and increase quality.*
- Allow language-independent build tools to be used on the codebase.

**Question 8 of 14**

Which of the following explains the concept of blue-green deployment?

- The end user (Blue) is able to self-serve, allowing them to initiate a process (Green) without any aid.
- A process in which both hardware and software are prepared and ready for operation in two live environments.
- **There are two identical production environments in which one is live (Blue) and the other is idle (Green). When new software is fully tested and deployed to Green, the router switches traffic from Blue to Green (Correct)**
- A method in which “Blue” maintains the control of the system and “Green” upgrades the application on the server.

**Question 9 of 14**

If you are developing end user test scenarios before writing code, then you are engaged in which type of development?

- integration testing
- feature-driven development
- **test-driven development (Correct)**
    - *Feedback: TDD focuses on building tests before you write the code to make them pass.*
- Agile development

**Question 10 of 14**

What is a build log?

- It is the building block of software development.
- **It is a record of all the tests that were run along with their results. (Correct)**
- It is a quick feedback loop for errors.
- It is a list of features that are planned for future product builds.

**Question 11 of 14**

Continuous delivery has all of these benefits except _____.

- increasing velocity
- **increasing fragile artifacts (Correct)**
    - *Feedback: By having a light and practical approach to change control, you can decrease fragile artifacts.*
- decreasing unplanned work
- lowering failure rates

**Question 12 of 14**

Suppose some of your tests are slow. Which procedures should you select to handle a slow test?

- Apply monitoring to complete some test objectives.
- **all of these answers (Correct)**
- Employ a non-blocking test.
- Utilize time-scheduled testing.

**Question 13 of 14**

Which task is part of a trunk-based development flow?

- enforcing commits to occur only once per day
- keeping active long-running development branches
- **having all developers commit to the main branch frequently (Correct)**
    - *Feedback: A trunk-based development flow requires all developers to commit directly to the master branch.*
- large merges of code with other developers

**Question 14 of 14**

Which belief has been disproven by organizations that utilize continuous delivery?

- **A high frequency of change leads to a decrease in quality. (Correct)**
    - *Feedback: A high frequency of change can lead to an increase in quality.*
- The movement from concept to cash is quicker.
- Small commits need to be rolled up into larger batches.
- Making changes directly in production is a best practice.

---

# 6. Site Reliability Engineering


## What is site reliability engineering?

- **Definition:** Site Reliability Engineering (SRE) is the application of engineering principles to solve real-world problems related to system reliability. It's the "operations" part of DevOps.
- **Reliability:** The ability of a system to perform its intended function correctly and consistently. This includes availability, performance, security, and other factors.
- **Holistic Approach:** SRE is not just about "bolting on" reliability after a system is live. It involves a holistic approach that includes:
    1.  **Building for Reliability:** Engineering systems and applications to be resilient from the very beginning.
    2.  **Operational Feedback:** Using observability and incident response practices to feed information from production back into the development process to improve the service.
- **SRE's Impact on Key Metrics:**
    - **Change Failure Rate:** Reduced through reliability testing and automated deployments.
    - **Time to Restore Service (MTTR):** Improved through good problem detection and operational automation.
    - **Availability and Performance:** Maintained through observability and resilience engineering.

## Building for reliability: Theory

- Success in production is heavily influenced by design-time decisions and software architecture.
- **Key Resources for Designing Reliable Applications:**
    1.  **"Release It!" by Michael Nygard:** The equivalent of the classic "Gang of Four Design Patterns" book, but focused on application stability.
        - **Key insight:** Integration points are the #1 cause of issues. **Cascading failures** (e.g., a slow database causing the application server to fail) are a primary threat.
        - **Stability Pattern Example:** The **Circuit Breaker** pattern stops making calls to a failing integration point to prevent the outage from spreading.
    2.  **The Twelve-Factor App (12factor.net):** A manifesto for building service-ready software.
        - **Example (Factor III - Config):** Runtime configuration should be stored in environment variables and kept separate from the application code.
    3.  **Martin Fowler's Work:** A highly experienced software engineer who writes succinctly about architectural concepts and DevOps-related topics.

## Building for reliability: Practice

- SRE brings hard-won operations experience ("street knowledge") into a disciplined engineering practice.
- **Key Concepts from "How Complex Systems Fail" by Dr. Richard Cook:**
    - All complex systems are always running in a partially degraded mode.
    - Change introduces new and unexpected forms of failure.
- **Shift from Prevention to Resilience:**
    - It's impossible to prevent all failures. The goal is **resilience**: the ability of a system to maintain a stable state and continue operations after a disruption.
- **Tools for Resilience Engineering:**
    - **Redundancy:** Running multiple identical copies of components.
    - **Load Balancing:** Directing traffic to healthy parts of the system.
    - **Automatic Scaling:** Adding more components to accommodate increased load.
    - **Automated Failover:** Automatically recovering from component failures.
- **Sociotechnical Systems:** All systems consist of both computers and the people who create, maintain, and use them. Resilience engineering must account for the human element.
- **SREs as Developers:** SREs should spend at least 50% of their time developing tools and automation, not just fixing things manually.
- **"You write it, you run it":** Developers are experts on their code and must be involved in resolving production problems. This means being on call and knowing how to use tools like debuggers and profilers in a live environment.

## Operational feedback: Observability

- **Observability:** A measure of how well the internal state of a system can be inferred from its external outputs (metrics, logs, etc.).
- **Five Key Areas of Observability:**
    1.  **Synthetic Checks (Health Checks):** Programmatically hitting a service to check its uptime and performance. Answers the basic question: "Is it working?"
    2.  **System and Application Metrics:** Time-series numerical data (e.g., CPU, memory, custom application metrics) to understand if a service is functioning normally.
    3.  **End-User Performance:** Using tools to get an accurate look at the user experience.
        - **Application Performance Monitoring (APM):** Reports performance at the code level (e.g., function call duration, database query time).
        - **Real User Monitoring (RUM):** Captures performance as observed directly by end-users, often via front-end instrumentation.
    4.  **System and Application Logs:** Detailed, text-based information that provides context beyond simple metrics. Can be used for troubleshooting, auditing, capacity planning, and more.
    5.  **Security Monitoring:** Using logs, metrics, and specialized tools to detect threats, indicators of compromise, and suspicious behavior.
- **Collaboration is Key:** Observability isn't just for operations. The data is valuable for developers to understand how their application is used and to improve the product.

## Operational feedback: Incident response and retrospectives

- **Incident Response:** The practiced activity of responding to and remediating problems in production. It requires three key skills:
    1.  **Troubleshooting:** In-depth system knowledge to diagnose and fix the problem.
    2.  **Automation:** Pre-built tooling to speed up information gathering and remediation.
    3.  **Communication:** Coordinating a team of specialists and keeping stakeholders informed.
- **Incident Management Process:** Inspired by the Incident Command System (ICS) used by emergency services, this is a defined process for how incidents are detected, reported, and managed.
- **Postmortems (Incident Retrospectives):** A formalized process to analyze an incident and learn from it.
    - **No Single "Root Cause":** Outages are caused by multiple deficiencies (in testing, monitoring, process, etc.), not one single mistake.
    - **Blameless Culture:** The goal is to understand how the system allowed a mistake to become an outage, not to assign blame.
    - **Transparency:** Open communication during and after an outage builds trust with stakeholders and end-users.

## Your DevOps SRE toolchain

- An SRE toolchain has two parts.
- **Part 1: Building for Reliability**
    - This is less about specific tools and more about using libraries (e.g., Java's Resilience4j) and development techniques. Requires collaboration between dev and ops at design time.
- **Part 2: Operational Feedback (Observability & Incident Response)**
    - This is a rich space with many tool options (SaaS, open-source, commercial).
    - **Lean Approach to Tooling (Build, Measure, Learn):**
        1.  **Build:** Create a minimum viable monitoring stack covering all five areas of observability with the quickest, cheapest options.
        2.  **Measure:** Start gathering data.
        3.  **Learn:** Analyze where more detailed information is needed to solve real problems and iterate. This avoids "monitoring waste."
- **Sharing and Customization:**
    - Share observability data widely. Developers, product managers, and business stakeholders can all benefit.
    - Build custom visualizations and dashboards that are meaningful to a non-technical audience.
- **Incident Response Tools:**
    - **On-Call & Alerting:** PagerDuty, VictorOps, OpsGenie.
    - **Runbook Automation:** Rundeck, Ansible Tower, StackStorm.
    - **Status Pages:** Atlassian Statuspage, Status.io.
- The key is to keep it simple, keep people in mind, and iterate on a toolchain that enables collaboration.

## Chapter Quiz

**Question 1 of 12**

What is a term for a well designed service?

- **a twelve-factor app (Correct)**
- a four-pattern app
- a microservice app
- a snazaroo

**Question 2 of 12**

What is the implication of us realizing all our IT systems are sociotechnical systems?

- It takes into account end user error in the perception of outages
- It takes into account larger sociopolitical trends and their influence on computing
- It means there is always someone to blame for system failures
- **It takes into account human activity in creating failures and maintaining system health (Correct)**

**Question 3 of 12**

Why do we focus on resilience instead of just plain reliability?

- Because it is less expensive
- Because it gets us more nines
- **Because failures are routine in a complex system (Correct)**
    - *Feedback: All systems fail; resilience is engineering uptime with that truth in mind.*
- Because avoiding failures is more important than recovering from them

**Question 4 of 12**

You are examining packets to determine whether your database is protected against SQL injections. Which type of monitoring is this?

- performance
- **security (Correct)**
    - *Feedback: SQL injection is a tool employed by hackers to defeat a system's security defenses.*
- application
- component

**Question 5 of 12**

Let’s say your colleagues are debating whether to employ synthetic or real user monitoring. How is real user monitoring different than synthetic checks?

- Real user monitoring monitors the speed of the application. Synthetic checks make sure the hardware is functional.
- Synthetic checks analyze security flaws in the application in real time whereas real user monitoring observers the system from the viewpoint of a hacker.
- Synthetic performance monitoring analyzes software performance in real world scenarios. Real user monitoring observes just the performance of the user, not the system.
- **Real user monitoring records all the actual end user’s engagement with the web application. Synthetic checks simulate how a user might interact with the application. (Correct)**

**Question 6 of 12**

Why is blame not a useful part of a retrospective?

- **It covers up systemic problems by scapegoating an individual (Correct)**
- It is! Blame is transparent communication after all
- It prevents us from improving our observability
- It makes people feel bad

**Question 7 of 12**

Which key metrics do SRE practices improve?

- engineer burnout; cycle time; business outcomes
- **change failure rate; time to restore service; meeting reliability goals (Correct)**
- cycle time; customer satisfaction; lead time
- mean time between failures; mean time to detect; mean time to restore
    - *Feedback: Mean times are poor metrics because they are usually not statistically significant.*

**Question 8 of 12**

What are the three key activities of incident response?

- Resilience, redundancy, and reliability
- Detection, response, and retrospective
- **Troubleshooting, automation, communication (Correct)**
- Observability, design, and operations

**Question 9 of 12**

Site reliability engineering (SRE) the discipline of using a software engineering approach to _____ and _____.

- automate operational processes; perform manual tasks
- **create reliable systems; automate operational processes (Correct)**
    - *Feedback: SRE includes both operational automation and building in reliability in the first place.*
- perform continuous delivery; implement infrastructure as code
- automate operational processes; institute observability

**Question 10 of 12**

Suppose your company is going to purchase a security monitoring tool. How should you select a security monitoring tool?

- **It should integrate well with your other systems and provide APIs so it can be shared across teams and groups. (Correct)**
- The security monitoring tool should suit your system and is compatible with new deployments.
- You should always use the newest and latest security monitoring tools since security threats are becoming more sophisticated although it may not work with your system fully.
- Security monitoring tools are not necessary since hackers are rarely caught although they do leave a trace behind.
- Regardless of the security monitoring tools out there, they are not solid proof against any security threats so it is better to find the cheapest one.

**Question 11 of 12**

Why should we take a Lean approach for tools, using Build-Measure-Learn?

- Because tools are really hard to use.
- **Because we don't want to overinvest resources into tools without knowing what we care about. (Correct)**
    - *Feedback: Yes!*
- Because tools are best chosen up front and then we build the system.
- Because there are only a few tool options and we don't want to get the wrong one.

**Question 12 of 12**

Which pattern would you need to build into your application to prevent cascading outages?

- an integration tester
- **a circuit breaker (Correct)**
    - *Feedback: A circuit breaker can stop an outage from propagating to other connected systems.*
- a disaster plan
- a quality assurance tester

---

# 7. Advanced Topics

## Platform engineering: The paved road

- **Concept:** As DevOps scales, you risk chaos from having too many teams creating diverse, custom solutions. Platform engineering is the discipline of creating standardized, self-service automation to guide teams along a "paved road" or "golden path."
- **Goal:** To solve common problems (like CI/CD, observability, infrastructure) once and provide them as a service to development teams. This reduces waste, decreases delay, and allows improvements to benefit everyone.
- **The Risk:** Platform engineering can devolve into old-school, bureaucratic, centralized IT if not implemented correctly.
- **How to Build a Good Platform:**
    1.  **Manage it Like a Product:** The platform must serve its users (developers), not its creators. Its value should be so high that teams *choose* to use it rather than being forced. Good platforms optimize for the global value stream, not for the central team's convenience.
    2.  **Take a Lean Approach:** Avoid building too much upfront. "Blaze a trail, then pave the road." Understand what users actually need before investing heavily in platform features.

## DevSecOps: Making your systems more secure the DevOps way

- **Concept:** DevSecOps is the practice of integrating security into the DevOps lifecycle to break down the silos between security, development, and operations teams.
- **The Problem:** Security is often an understaffed, downstream team that acts as a blocker, creating friction. Developers care about security but often lack the time and clear guidance to implement it effectively.
- **Applying CAMS to Security (DevSecOps Principles):**
    - **Culture:** The core tenet is: "If security introduces blocking to the organization, it will be ignored, not embraced." Security must work *with* the value stream, not against it.
    - **Automation ("Shifting Left"):** Introduce security testing and tools earlier in the development lifecycle (e.g., in the IDE and CI system), not just at the end. This provides fast feedback when issues are cheapest to fix. **Caveat:** This must be done without bloating build times or dumping undue work on developers.
    - **Sharing:** Use "Security Champions"—deputized volunteers within product teams—to act as a bridge, sharing knowledge and responsibility between the central InfoSec team and developers.
    - **Measurement:** Use metrics and shared goals to drive security improvements, not FUD (Fear, Uncertainty, and Doubt).

## Cloud native and Kubernetes

- **Kubernetes:** An open-source container orchestration system for automating software deployment, scaling, and management.
- **Benefits:**
    1.  **Automation Platform:** It automates much of the "plumbing" required to run applications (deployment, scaling, service discovery, health monitoring).
    2.  **Infrastructure Abstraction:** It provides a consistent service layer that allows applications to run across on-premise data centers and different cloud providers.
- **Cloud Native:** A term that, in modern practice, largely refers to tools and technologies designed to work with Kubernetes. The Cloud Native Computing Foundation (CNCF) maintains a vast landscape of these tools.
- **Challenges and Considerations:**
    1.  **Complexity:** Kubernetes is highly configurable, leading to a steep learning curve and complex systems built from many stitched-together tools.
    2.  **Cost and Overhead:** It is a large, heavy, and expensive system that often requires a dedicated team to administer. It can be overkill for simpler applications.
    3.  **Risk of New Silos:** Without a DevOps mindset, a Kubernetes platform can easily become a new silo that hinders collaboration and value flow.

## DevOps and chaos engineering

- **Definition:** Chaos engineering is the discipline of experimenting on a system by deliberately introducing failures (e.g., shutting down a server, introducing network latency) in order to build confidence in the system's ability to withstand turbulent, real-world conditions.
- **Origin:** Popularized by Netflix with their "Chaos Monkey" tool, which randomly terminates production servers to force teams to build resilient systems.
- **Goal:** To move beyond *assuming* a system is resilient to *proving* it through controlled experiments in a production environment.
- **Practices:**
    - **Validate Automated Remediation:** Confirm that automated failover and recovery systems work as expected.
    - **Game Days:** Test the human part of incident response by creating a controlled outage and having teams work through their practiced response procedures.
- **Connection to DevOps:** It is a direct application of The Three Ways (using feedback loops for learning) and helps create a true learning organization.

## MLOps: Leveraging DevOps to run ML systems

- **Concept:** MLOps is the application of DevOps principles and practices to the unique lifecycle of machine learning (ML) and artificial intelligence (AI) systems.
- **What Makes MLOps Different:**
    1.  **People:** The primary users are often data scientists, who are less systems-focused than developers but whose work is highly dependent on specific hardware (e.g., GPUs).
    2.  **Artifacts:** In addition to code and infrastructure, MLOps must manage and version massive **datasets** and **ML models**.
    3.  **Workloads:** Training jobs are often intensive, long-running batch processes on expensive High-Performance Computing (HPC) clusters.
    4.  **Feedback & Results:** ML models produce outputs of varying quality, not a simple pass/fail, creating a more complex feedback loop.
    5.  **Drift:** You must monitor for drift in model *predictions* and performance, which is more complex than typical application monitoring.
- **Process:** Involves parallel and interrelated CI/CD pipelines for software, infrastructure, and the data/models.

## AIOps: Using AI in your DevOps work

- **Concept:** AIOps is the practice of using Artificial Intelligence (AI) to assist and augment the work of DevOps professionals, helping to manage complexity and reduce cognitive overload.
- **Key Caveat:** AI is an *assistant*, not a replacement. The engineer is always responsible for validating and testing AI-generated output.
- **Use Cases:**
    - **Code & Script Generation:** Creating API integrations, command-line scripts, and code in unfamiliar languages. **Prompt engineering** is a key skill.
    - **Explanation & Documentation:** Explaining what complex code does and generating documentation for it.
    - **Improving Monitoring:** Assisting with alert triage and recommending remediation actions.
    - **Code Conversion:** Translating code from one platform or language to another (e.g., Terraform to AWS CLI).
    - **Security:** Assisting with code reviews and finding risky changes.
- **The Three Waves of AIOps:**
    1.  **Wave 1 (Code):** AI-assisted coding and testing (e.g., GitHub Copilot). **(Happening Now)**
    2.  **Wave 2 (Systems):** AI-driven monitoring, alerting, and system explanation. **(In its Infancy)**
    3.  **Wave 3 (People):** AI-powered self-service platforms and enhanced team collaboration. **(Future)**

## Chapter Quiz

**Question 1 of 12**

Besides developers and operations, what is the other group most necessary to be part of MLOps?

- Networking
- Sales
- **Data Scientists (Correct)**
    - *Feedback: Yep, Data scientists need to be involved with MLOps.*
- Platform Engineering
    - *Feedback: Not usually.*

**Question 2 of 12**

By practicing Chaos Engineering, what is the desired outcome?

- Preventing Chaos
- **Resilience and Reliability (Correct)**
    - *Feedback: Yep, Chaos Engineering advances resilience and reliability.*
- Finding the offending developer
- Root Cause Analysis

**Question 3 of 12**

Shift Left has worked well in every organization and had a positive impact.

- **FALSE (Correct)**
    - *Feedback: While it sometimes works, it doesn't always.*
- TRUE

**Question 4 of 12**

What are benefits of AIOps and using AI for DevOps work?

- Code Reviews and Security
- Language Conversion
- Refactoring and Documentation
- **All of these (Correct)**
    - *Feedback: Yes, all of these*

**Question 5 of 12**

A good example of a paved road approach is a _____.

- ITIL
- **CI/CD Pipeline (Correct)**
    - *Feedback: Yes*
- Shadow IT
    - *Feedback: This isn't' paved road*
- Using a Change Advisory Board

**Question 6 of 12**

What is MLOps?

- Management Line Ops is a way for managers to see what is happening on the line,
- **The extension of DevOps for Machine Learning systems (Correct)**
    - *Feedback: Yes, it extends devops for ML.*
- It is the sales opportunity for ML in an organization.
- Used for calculating cycle time of your system.

**Question 7 of 12**

When you hear people talking about Cloud Native, that usually suggests they are talking about _____.

- Rust programming language components
- Amazon
- **Kubernetes (Correct)**
    - *Feedback: Yes!*
- Large Language Models

**Question 8 of 12**

What is prompt engineering?

- Using AI in your linux command line prompt.
- **The process of structuring a text query that can be interpreted and understood by a generative AI model. (Correct)**
    - *Feedback: Correct! It's how we tune the AI to the task at hand.*
- Asking AI tools to remind you of tasks.
- Using AI to change how ask questions of your team and coworkers.

**Question 9 of 12**

A pattern people use to find security friendly developers to advance security in a team or devops context is called: _____.

- **Security Champions (Correct)**
    - *Feedback: Yes!*
- Security Ninjas
- Security Pros
- Security Wizards

**Question 10 of 12**

What is fault injection?

- being able to find the fault in the system before developers commit the code
- adding a webhook to your system that checks for faults
- **intentionally applying an outage or performance degradation to a live system component (Correct)**
    - *Feedback: Yes, just like Chaos Monkey!*
- a part of observability tools

**Question 11 of 12**

What is Kubernetes?

- **open-source container orchestration system for automating software deployment, scaling, and management (Correct)**
    - *Feedback: Yep!*
- a simple tool that works with a small number of containers
- A tool built and popularized by Microsoft that orchestrates containers and eases the burden of operational maintenance.
- a cloud provider

**Question 12 of 12**

Once you build a paved road you should require that other teams use it.

- TRUE
- **FALSE (Correct)**
    - *Feedback: Try to make it desirable to use, but not forced*

---

# 8. Your DevOps Career

## DevOps and your career

- DevOps is a mindset and a suite of practices, not just a specific job title. Understanding it can benefit anyone in a technology organization.
- **For a Developer:** It provides a better understanding of how to build reliable, observable applications and align work with the overall value stream.
- **For a System Administrator ("DevOps Engineer"):** It means shifting from a manual, siloed approach to building systems with IaC, focusing on reliability, and implementing observability and automation. You understand that collaboration, automation, measurement, and sharing (CAMS) are what create effectiveness.
- **Specialized DevOps Roles:**
    - **Automation/Platform Engineer:** A developer focused on creating automation for system and business outcomes.
    - **Build/Release Manager:** A specialist in creating and maintaining CI/CD pipelines and managing the business communication around releases.
    - **Site Reliability Engineer (SRE):** The most common term for those performing runtime support: observing, managing, and fixing live systems.
- **Benefits Beyond Technical Roles:** Understanding DevOps is valuable for sales, marketing, product managers, and executives to understand the benefits and effectively interact with the ecosystem.

## DevOps learning resources

- A lightning round of key resources to continue your DevOps learning journey. (A full list is available in the course handout).
- **Top 10 DevOps Book List:**
    - **All-Around Reads:** *The DevOps Handbook*, *Accelerate*, *The Phoenix Project*.
    - **Core Practices:** *Continuous Delivery*, *Site Reliability Engineering Book*, *Infrastructure as Code*.
    - **Key Perspectives:** *Release It!* (developer view), *The Practice of Cloud System Administration* (operations view).
    - **Process Foundations:** *The Visible Ops Handbook*, *Lean Software Development*.
- **Online Sources:**
    - **Newsletters:** Many weekly newsletters summarize recent developments.
    - **Websites:** Martin Fowler (expert articles on Agile/DevOps), Julia Evans (zines/comics explaining technical topics).
- **Certifications:**
    - Many are technology-specific (AWS, HashiCorp, Kubernetes).
    - The DevOps Institute offers broader DevOps certifications.
    - University boot camps (e.g., Caltech) are available.
- **Conferences and User Groups:** A highly effective way to learn by meeting other practitioners.
    - **DevOps Enterprise Summit:** A polished event focused on large organizations.
    - **DevOpsDays:** A global series of low-cost, community-organized local events. This is where DevOps started.
    - **All Day DevOps:** A free, 24-hour online conference.

## Your personal DevOps journey

- Experience is the best teacher. Continuous learning combines hands-on practice with frequent feedback.
- **Create a Learning Path:** Your next steps depend on your target role and current skills. You'll need different levels of depth in various technologies.
- **Foundational Technical Skills:** Operating systems, programming languages, cloud, and containerization.
- **The DevOps Foundations Curriculum:** This course is part of a larger series of courses in the LinkedIn Learning library covering each of the major practice areas in more detail.
    - **Core Practices:** Lean and Agile, Visible Ops Change Control, Infrastructure as Code, CI/CD, Site Reliability Engineering.
    - **Security:** Automated Security Testing, Building a DevSecOps Pipeline.
    - **Advanced Drill-Downs:** Observability, Incident Management, Incident Response.
    - **For Leaders:** A specific course on DevOps Management.
    - **Troubleshooting:** A course on DevOps Anti-Patterns and how to combat them.
- The journey continues. Stay curious, keep learning, and connect with the community.