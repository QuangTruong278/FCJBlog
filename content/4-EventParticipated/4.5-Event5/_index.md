---
title: "Event Report: Agentic AI Journey"
date: "`r Sys.Date()`"
weight: 6
chapter: false
pre: " <b> 4.6. </b> "
---
# Summary Report: “Agentic AI: From High-level Architecture to Hands-on”

### Event Objectives

- Understand the core concepts of Agentic AI and AWS Bedrock Agents.
- Explore real-world use cases for building Agentic Workflows.
- Deep dive into Agentic Orchestration and Context Optimization (Level 300 technical depth).
- Hands-on experience: Building an agent using CloudThinker and AWS Bedrock.

### Speakers

- **Nguyen Gia Hung** – Head of Solutions Architect
- **Kien Nguyen** – Solutions Architect (AWS)
- **Viet Pham** – Founder & CEO
- **Thang Ton** – Co-founder & COO (CloudThinker)
- **Henry Bui** – Head of Engineering (CloudThinker)
- **Kha Van** – Technical Lead/Facilitator

### Key Highlights

#### AWS Bedrock Agent Core
- **Concept:** Moving beyond passive "Chatbots" to active "Agents" that can execute multi-step tasks.
- **Components:** Explained the anatomy of an Agent: Foundation Model (Brain) + Action Groups (Tools/APIs) + Knowledge Bases (RAG).
- **Functionality:** How Bedrock Agents break down a complex user prompt into a chain of logical steps (Chain-of-Thought) and execute them via Lambda functions.

#### Real-world Application & CloudThinker
- **Use Cases:** Creating workflows where AI autonomously handles business processes (e.g., booking, order processing, data analysis) without human intervention.
- **Orchestration (L300 Deep Dive):** Henry Bui shared advanced techniques on managing complex agent interactions. The focus was on **Context Optimization**—ensuring the AI retains relevant information across long conversations without hitting token limits or losing focus.
- **CloudThinker Platform:** Introduction to a specialized framework designed to simplify the orchestration of complex agentic workflows on top of AWS.

#### Hands-on Workshop: CloudThinker Hack
- **Practical Lab:** We didn't just listen; we built. Guided by Kha Van, we set up a working environment to deploy a functional agent.
- **Integration:** Connected the agent to external tools and observed how it reasoned through tasks in real-time.

### Key Takeaways

#### The Shift to "Agency"
- The future of AI is not just generating text, but taking action. "Agentic AI" is the next frontier where models become decision-makers.

#### Context is King
- In complex workflows, managing "State" and "Context" is the hardest challenge. Optimization techniques (like summarizing context or selective retention) are critical for production-grade agents.

#### Orchestration Complexity
- Building one agent is easy; making multiple agents work together requires a robust orchestration layer (which tools like CloudThinker aim to solve).

### Applying to Work

- **Experiment with Action Groups:** I will try adding a simple "Action Group" to my Bedrock test project (e.g., a Lambda function that queries a database) to turn my chatbot into a basic agent.
- **Study Context Management:** Research more on how to optimize prompt context for long-running tasks, as emphasized in the L300 session.
- **Blue/Green Testing for Agents:** Apply the testing concepts learned to evaluate if an agent is performing actions correctly before full deployment.

### Event Experience

The **"Agentic AI"** event was a perfect blend of theory and practice.

#### Technical Depth (L300)
I particularly appreciated the **L300 session** by Henry Bui. Often events stay high-level, but this session went deep into the engineering challenges of Context Optimization, which gave me valuable architectural insights.

#### The "Hack" Component
The hands-on session at the end was energetic and rewarding. Seeing the agent I configured actually execute a task (instead of just replying with text) was a "lightbulb moment" regarding the power of the Bedrock ecosystem.

#### Networking
The lunch buffet and networking time allowed me to discuss with the CloudThinker team about the challenges of latency in agentic workflows, providing practical tips for my own projects.

#### Some event photos
*Add your event photos here*

> Overall, this event bridged the gap between the "hype" of AI Agents and the "how-to" of building them on AWS.