# n8n-prd-generator
Multi-agent PRD generator built on n8n — nine sequential and parallel GPT-4o agents that turn a product idea into a formatted PRD delivered by email.

▶️ **[Watch the workflow demo on Loom](https://www.loom.com/share/1c588f3ea80a44c88c8b1e81a290fd78)**

---

## The problem

Writing a first-draft PRD takes product managers hours: framing the problem, defining users, scoping requirements, thinking through metrics and risks. Much of that first pass is structured and repeatable — which makes it a good fit for a coordinated set of AI agents, leaving the PM to focus on judgement and refinement.

## What it does

- Takes a product idea as input
- Runs it through **nine specialised AI agents**, each responsible for one part of the PRD
- Combines their outputs into a single, structured PRD
- Delivers the finished document as a **formatted HTML email**

## How it works

1. A product idea is submitted to the workflow
2. Agents run in a mix of **sequential** steps (where one section depends on another) and **parallel** steps (where sections can be drafted independently, to save time)
3. Outputs are merged and formatted into HTML
4. The completed PRD is emailed to the user

## Design decisions

- **Specialised agents over one big prompt** — each agent has a narrow job, which produces more focused, higher-quality sections
- **Parallel where possible** — independent sections run simultaneously to cut total generation time
- **Email as the output** — the PRD lands where PMs already work, ready to review and share

## Built with

- **n8n** — workflow orchestration
- **OpenAI GPT-4o** — agent reasoning and generation

---

*Built by [Shivang Jindal](https://www.linkedin.com/in/shivang-jindal-pm) — Senior Product Manager, fintech & enterprise SaaS.*
