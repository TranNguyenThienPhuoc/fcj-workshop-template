---
title: "Event 2"
date: 2026-05-23
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---

# Summary Report: "In-depth AI & Cloud Sharing Series"

### Event Objectives

- **Shift the AI mindset**: Move from merely "writing basic prompts" to building an "AI context and memory system" for efficiency; raise awareness regarding the Non-Determinism of LLM models.
- **Introduce advanced solutions**: Share insights on Agentic AI (Amazon Quick Suite), enterprise-grade Multi-Agent systems, and Amazon CloudFront as a core platform for optimizing performance, security, and costs.
- **Networking and pushing limits**: Create a space to learn from AWS experts and outstanding developers through in-depth talks and a large-scale Hackathon.

### Speakers

- **Tinh Truong** – Platform Engineer at GoTymeX.
- **Pham Ng Hai Anh** – AWS Community Builder (G-AsiaPacific Vietnam).
- **Nguyen Tuan Thinh** – DevOps Engineer at First Cloud AI Journey (FCAJ).
- **Duc Dao** – Solution Architect at Cloud Kinetics.
- **Vy Lam** – Senior Business Systems Analyst at VPBank.
- **Team VIB (UTMorpho Project)** – Competitors in LotusHacks 2026.

### Key Highlights

#### The Importance of "Context"
- **The root of the error**: Generic or misdirected AI responses are usually due to weak user context, not a poor AI model.
- **3 common mistakes**:
  - **Internet Puller**: Cramming unfiltered documents, causing noise.
  - **Stating the obvious**: Providing default information the AI already knows.
  - **Lacking goals and constraints**: Giving vague requests (e.g., "Make me a website").
- **Evolution trend**: The usage of AI is shifting from single Prompts → Context (attached to documents) → Memory (Long-term memory / Second AI Brain).

#### Amazon Quick Suite (Agentic AI) Solution
- **Enterprise pain points**: Wasting time gathering data from multiple sources and repeating manual tasks.
- **Comprehensive ecosystem**: Includes BI (Dashboard), Automation (Flows), and Insights (Chat/Research) integrated with the Bedrock model and over 40 data connectors.
- **Practical Demo**: A PM Assistant automatically generating Minutes of Meeting (MoM), sending emails to stakeholders, and scheduling follow-up meetings.

#### Amazon CloudFront Platform
- **Enterprise challenges**: Financial risks due to out-of-control CDN costs (bill spikes) caused by fluctuating traffic or DDoS attacks.
- **Exclusive Fixed-Price solution**: A new fixed-price package integrating CDN, WAF, Anti-DDoS, Route 53, and S3 storage credits.
- **Distributed DDoS protection**: Mitigating large-scale (volumetric) attacks right at the Edge via AWS Shield, WAF, and Origin Shield to reduce the load on origin servers.
- **Cost optimization**: Reducing Load Balancer costs from $8.13 to $2.95 (leveraging up to 1TB of CloudFront Free Tier Data Transfer Out).

#### LotusHacks 2026 Hackathon Challenge
- **The Journey**: Going from an "empty mind" in the first hour to a turning point of finding an idea from daily work to create the UTMorpho project.
- **Technical Hurdles**: Successfully handling complex problems like AI Overgeneration and Token Limits within 36 hours.

#### Non-Determinism of "Deterministic" LLM Settings
- **Theory vs. Reality**: In theory, Temperature = 0 (Greedy Decoding) ensures 100% consistent results. In reality, across 5 major models (GPT-3.5, GPT-4o, Llama-3, Mixtral), accuracy can deviate by up to 15% between identical runs.
- **Hardware causes (GPU)**: Floating-point arithmetic on GPUs is non-associative: (a+b)+c != a+(b+c). Parallel processing causes an inconsistent execution order, leading to rounding errors that flip the token selection function (argmax).
- **Commercial causes (Batching)**: Grouping multiple user requests (Inference Batching) to optimize costs indirectly alters the model's computational process.

#### Multi-Agent Systems Application
- **Data asymmetry**: Traditional banks reject Startups due to a lack of financial history (requiring 3 years vs. an actual 6-18 months).
- **Single Agent limitations**: Using only 1 AI Agent easily leads to diluted expertise, context overload, and a lack of cross-checking.
- **Virtual Credit Board**: A coordinated model of specialized Agents (Financial, Market, Team, Risk, Compliance) to make accurate, transparent, and auditable decisions.

### Key Takeaways

#### Context Building & AI Communication
- Understanding the principle: Context quality is more important than quantity.
- **4-element context framework**:
  1. **Goal**: The final desired outcome.
  2. **Relevant info**: Providing only strictly necessary data.
  3. **Constraints**: Limitations on technology, budget, format, and style.
  4. **Success criteria**: What constitutes a satisfactory answer.

#### Enterprise AI Deployment Mindset (Agentic & Multi-Agent)
- The mindset of applying **Agentic AI** to automate complex task chains rather than just using regular chatbots.
- Understanding **Multi-Agent** design thinking: How to break down a complex problem into specialized tasks for parallel AI processing, increasing accuracy and fault tolerance.

#### Cloud Architecture & Defense in Depth
- Deeper understanding of new pricing models and how Regional Edge Caches operate.
- Grasping the principle of defense-in-depth: Blocking malicious traffic at the nearest access point instead of letting it penetrate deep into the system.
- Knowing how to optimize the architecture between EC2/ALB and CloudFront to leverage free bandwidth.

#### Technical Nature of LLMs & Teamwork Skills
- **Shattering illusions**: Realizing the illusion of absolute safety and repeatability when programming with LLMs at default settings. Understanding the probabilistic nature of AI from the hardware level.
- **Professional skills**: Experience in optimal system architecture design and handling AI model errors under immense pressure.
- **Soft skills**: Time management, energy distribution, cohesive teamwork, and staying calm to find solutions during a crisis.

### Applying to Work

- **Applying the 4-element framework**: Writing daily prompts to optimize time spent debugging code, writing emails, and summarizing documents.
- **Building a Second AI Brain**: Planning to build a personal knowledge management system utilizing cloud storage and AI for long-term learning.
- **Deploying automation**: Integrating Automation Flows and Agentic Workflows into project management, administrative reporting, and multidimensional data appraisal.
- **Infrastructure optimization**: Using CloudFront to distribute content, lower ALB costs, and proposing AWS WAF and Rate Limiting to enhance baseline security.
- **Developing Safe AI**: Applying solutions to mitigate LLM unpredictability: Structured output (JSON mode, function calling, regex grammars), Majority Voting (running $N$ times), parameter optimization (setting Temperature to 0.1 with increased repeat penalty), and accepting variability in logic processing.
- **Improving workflows**: Seeking automation opportunities from repetitive tasks; applying accelerated workflows (agile/sprint under pressure) to actual department projects.

### Event Experience

#### Practical and Visual Learning
- The shared content was highly practical, featuring comparative examples (Bad vs. Good Prompt) and scientific data (CloudFront cost charts) that made it easy to understand.
- Practical demos (like the PM Assistant) were highly visual, receiving a lot of interaction and lively discussion from attendees.

#### In-depth Experience and Broadened Perspectives
- The sessions offered a technical yet highly accessible perspective for students and freshers, helping them easily grasp complex DevOps concepts.
- Providing real-world case studies from banking-finance experts helped broaden the mindset of turning proof-of-concept (PoC) AI models into production-ready systems.
- Changing system testing design thinking (Regression testing/A-B testing) when working with AI.

#### Pushing Personal Limits
- Participating in LotusHacks was a thrilling and incredibly fun ("have fun") experience. The team experienced burnout near pitch time but successfully overcame it at crucial turning points to successfully deliver the product.

#### Some event photos
![Event 2](/images/4-EventParticipated/Event2.jpg)
> Overall, the event provided an immense amount of rich and specialized knowledge alongside practical application. It not only provided tools but also reshaped my mindset toward design thinking, teamwork, and maximizing the power of AI/Cloud in actual work.
