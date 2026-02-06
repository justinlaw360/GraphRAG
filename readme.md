# What is GraphRAG and why it matters?


Generative AI (GenAI) models are trained on vast datasets composed primarily of publicly accessible information, including open-source publications, internet articles, social media content, and other public-domain materials. As a result, the outputs produced by these models are limited to general knowledge.

Incorporating proprietary information—such as personal research notes or organization specific data—directly into a large language model would require retraining the model. However, this approach is both costly and operationally impractical, especially when updates occur frequently. Continuous retraining to reflect revisions or new internal documents is simply not feasible.

To address this challenge, researchers advocate the use of Retrieval-Augmented Generation (RAG), an approach that enables AI models to access and leverage private or domain-specific information without the need for full model retraining.

## The RAG ##

RAG allows generative AI models to access additional external knowledge bases, such as internal organizational data, scholarly journals and specialized datasets. By integrating relevant information into the generation process, chatbots and MCP agents can create more accurate domain-specific content without needing further training.

In conventional RAG processes and pipelines, large documents will be chunked and break into smaller segments, and vectorization converts each chunk into an embedding for semantic search.  If you are interested to know more about RAG, you may read my another article in  https://github.com/justinlaw360/RAG: Retrieval-Augmented Generation using Azure OpenAI.

However, chunking and vectorization cannot preserve well and even lose the relationship information between entities.   The relationship among data entities is important information for gen AI models to calculate the near similarities between the prompt (queries of users) and the relevant data (output or answer from chatbot).

## The Knowledge Graphs ##

A knowledge graph is a structured representation of information that organizes data entities and their relationships in a network format. Knowledge graphs utilize LLM to construct a comprehensive view of nodes, edges, and labels through a process called semantic enrichment. Once a knowledge graph is complete, it allows question answering and search systems to retrieve comprehensive answers to given queries.

Building a knowledge graph is a complex undertaking. It requires collecting data from hundreds—sometimes thousands—of documents, identifying entities, understanding domain‑specific relationships, and designing an appropriate schema. Even for relatively simple domains, this process can take several hours when done manually.

A simple knowledge graph represents the SOC services that I provide to my company.  In the past, developing such a graph required several days of manual effort—from identifying entities to mapping relationships and labelling connections. With the support of large language models, however, the process has become significantly more efficient. An LLM can now generate a complete, well structured knowledge graph—with nodes, edges, and labels—in just minutes, transforming what was once a labor intensive task into a rapid, streamlined workflow.


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



