## Landing Zones for Azure Artificial Intelligence Applications

This repository contains guidance on tips, strategies and best practices on how to design, architecture, implement and maintain AI applications on Microsoft Azure.

The Azure ecosystem provides a comprehensive set of out-of-the-box and customizable AI tools, APIs, and models that help modernize your business with less effort and faster turn around times.

Azure has capabilities including but not limited to the following areas:

- Azure OpenAI
- Search
- Vision
- Speech
- Language Analysis
- Document Intelligence
- Video and Audio
- Decision Capabilities

Any of the AI applications build for deployment on Microsoft Azure is going to leverage one more AI services from the categories listed. 

The goal of this framework is to provide comprehensive guidance on how to leverage these capabilities alongside Azure data services and other foundational infrastructure to build intelligent applications that can perform and scale efficiently in production environments.

The following sections summarize the various areas covered in this framework:

## Framework Sections
- **[Building AI Applications Responsibly](Sections/00-Responsible-AI.md)**
  - It is crucial that we build any application responsibly and this is even more critical when these system can have significant impact. Responsible Artificial Intelligence (Responsible AI) is an approach focused on creating, evaluating, and using AI systems in a manner that prioritizes safety, trustworthiness, and ethics. It involves guiding decisions made during AI system development and deployment to ensure they align with beneficial and equitable outcomes. This approach emphasizes keeping people and their objectives central to system design and upholding core values such as fairness, reliability, and transparency.

- **[Securing AI Resources](Sections/01-Securing-Data-and-Resources.md)**
  - It is always important to ensure that data is secured at rest and while in transit across components of the architecture. We also have to ensure that the credentials used to 

- **[Costs & Performance Optimizations](Sections/02-AI-Apps-Cost-and-Performance-Optimizations.md)**
  - Financial costs and application performance are crucial to the long term operations of any production-grade app. It is always easier to focus on building the application by selecting the latest and greatest without necessary considering how these components will perform or how much they are going to cost to use in the architecture.

- **[Quota Consumption Monitoring & Enforcement](Sections/03-Quota-Monitoring-and-Enforcement.md)**
  - Having an efficient and effective mechanism to track usage and enforce usage constraints is critical in all production-grade AI applications. This section covers the strategies you can leverage to do so.

- **[Batch & Near Realtime Synchronization of Search and Vector Stores](Sections/04-Datastore-Synchonization-Mechanisms.md)**
  - This section covers how to build data pipelines that tracks changes to the structure and unstructured data stores such as (object stores, relational databases, NoSQL databases) and automatically processes the embeddings for these documents (if necessary) and stores these dense vectors in the appropriate vector databases for usage in vector, sparse and hybrid search. This challenge covers vector store selection based on performance, capacity, available algorithms etc as well as various data synchronization strategies for batch & near realtime scenarios.

- **[Content Intelligence & Analysis](Sections/05-Content-Intelligence-and-Analysis.md)**
  - In this section we cover how to use the Document Intelligence service and other cognitive services to process documents, images, videos and audio content to extract insights and useful data that can be used to build intelligent AI applications 

- **[Retrieval Augmented Generation & OpenAI Function Calling](Sections/06-RAG-Architectures-and-OpenAI-Function-Calling.md)**
  - In this section we cover strategies for building efficient applications that leverage RAG architectures and OpenAI function calling to build apps that can interactively retrieve, update, delete and create records in external databases and APIs using OpenAI Function calling, Vector Search and hybrid search.
