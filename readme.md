# What is GrapRAG and why it matters?
## The RAG ##

**Generative AI** (gen AI) models are **trained on large datasets** limited to the information that can be access in public domain works, internet articles, social media content and other publicly accessible data.  The generated output from Gen AI is so limited to general information only.

**RAG** allows generative AI models to **access additional external knowledge bases**, such as internal organizational data, scholarly journals and specialized datasets. By integrating relevant information into the generation process, chatbots and MCP agents can create more accurate domain-specific content without needing further training.

In conventional RAG processes and pipelines, large documents will be **chunked** and break into smaller segments, and **vectorization** converts each chunk into an embedding for semantic search.  However, chunking and vectorization cannot preserve well and even **lose the relationship information** between entities.

The relationship among data entities is important information for gen AI models to calculate the near similarities between the prompt (queries of users) and the relevant data (output or answer from chatbot).

## The Knowledge Graphs ##

A knowledge graph is a structured representation of information that organizes data **entities** and their **relationships** in a network format. Knowledge graphs utilize LLM to construct a comprehensive view of **nodes, edges, and labels** through a process called semantic enrichment. Once a knowledge graph is complete, it allows question answering and search systems to retrieve comprehensive answers to given queries.

<img width="894" height="650" alt="image" src="https://github.com/user-attachments/assets/e7ce8442-3ad3-4207-9c66-0aaa9553a601" />

The knowledge graph of the SOC services I am providing to the company.  Using LLM, it is amazingly easy to generate a knowledge graph with nodes and edges in a minute.  It normally took few days by hand in the past.  

* Organizations: CompanyM, Contractor, SOC (HK-based), ISA, Subcontractors
* Domains: IT Network, OT Network
* Platforms: Elasticsearch SIEM, JIRA, secure remote access (IPSec/SASE)
* Log sources / tools: Firewalls, Imperva WAF, Akamai DDoS/WAF, F5, Microsoft Defender stack, AD/Entra, Trellix, Vectra NDR, Nozomi, Zscaler, OS logs, web servers, CyberArk, Symantec EPM, Tenable Nessus
* Capabilities: 24×7 monitoring, detection engineering/use cases, threat intel, threat hunting, incident triage/response, quarantine via EDR, evidence collection, reporting; optional MDR, Vulnerability Management, on site OT support
* Processes: Onboarding → UAT → Parallel run → Production launch, BCP/DR, audit & KPIs, SLA Management, exit & data return
* Compliance: ISO/IEC 27001:2022, HK Protection of Critical Infrastructures Ordinance, IEC 62443, MITRE ATT&CK
* SLA highlights: Availability, response SLAs by severity (15/30/60/180 mins), on site dispatch



