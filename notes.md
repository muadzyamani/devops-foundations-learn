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
