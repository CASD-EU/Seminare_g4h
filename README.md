# Seminar data catalog

In this seminar, we will learn:
- What is data governance?
- What is metadata management? 
- What are the popular metadata management tools?
- How to use Open-Metadata(OM) as a metadata management tool?

## 1. What is data governance?

**Data governance is a collection of processes, roles, policies, standards, and metrics** that ensure the data
- availability, 
- usability/interoperability,
- security (i.e. confidentiality, integrity, privacy). 

It makes the use of data **consistent, trustworthy, effective and efficient.** 

**Data governance is a strategy, not a technology**. It consists of a set of decision-making process and rules which 
 govern data throughout their entire data life-cycle. It defines mainly three things:
- **People**: who have the right to make the decisions and accountable for them. For example, if someone asks to access data,
  who can decide whether we grant access to the user or not.
  
- **Policies**: what `decisions/rules` must be made to ensure effective management and use of data (decision domains). For example, 
  before publishing data, the data must pass the `quality control` and `privacy control`, etc.

- **Metrics**: how to `measure/evaluate` if `decisions/rules` are respected. For example, to control the `data quality`, we need 
  to define the `metrics for data accuracy, completeness, etc`.

### 1.1 What is data management

**Data management is an entire suite of practices, processes,  systems and tools which implement the data governance definitions**. 

The five elements of an integrated Data management framework:

- Data Principals: define governance.
- Data Lifecycle: tracks data’s journey.
- Data Quality: ensures usability.
- Metadata management: provides context of data.
- Data Security: protects data assets.

The Below figure shows a general representation of data governance and management

![introduction_of_data_governance_terms.jpg](assets/introduction_of_data_governance_terms.jpg)


## 2. What is metadata management?

Managing metadata involves:

- **Collecting metadata**: gathering information(e.g. schemas, formats, transformations, provider, etc.) about data.
- **Lineage tracking**: Understanding where data came from and how it changed.
- **Term definitions**: Standardizing terms, so `sedona` means the same everywhere for everyone.
- **Cataloging**: Building searchable inventories of data assets.

### 2.1. What is metadata?

### ISO definition

In **ISO/IEC 11179**, the `metadata (information objects) are data about Data Elements, Value Domains, and other reusable 
semantic and representational information objects` that describe the `meaning and technical details` of a data item.

### My definition 

**Metadata** is `structured information` that describes one or more aspects of a data entity. 
In general, Metadata is used to summarize basic information about data which can make `finding, tracking, using,
and managing` data easier. 

### 2.2 what are the objectives of the metadata?

In general, metadata should answer the following questions:
- What is the data asset about? → Descriptive Metadata
    - Purpose: Explains content and meaning. 
    - Examples:
         - Descriptions (tables, columns): Contains purchase history of retail customers
         - Keywords or tags: sales, transaction, retail, invoice
         - Themes or categories
    - Use case: Helps users discover and understand data.
- Why does the data asset exist?
    - Data source
    - Lineage
    - Impact analysis
- Where is the data asset from?
    - Spatial coverage
    - Language
    - Business domains
- Who is responsible for the data asset?
    - Creator or owner
    - Contributors or experts
    - Point of contact
- When was the data asset created and updated?
    - Creation date
    - Last updated or modified date
    - Update frequency
- How can the data asset be used?
    - License
    - Classification
    - Use cases




2. Why does the data asset exist? → Purpose/Business Metadata

Purpose: Explains business context, goals, and justification.

Examples:

“Collected to support regulatory reporting”

“Created for customer segmentation in marketing campaigns”

Use case: Ties data to organizational objectives and compliance.

3. Where is the data asset from? → Lineage Metadata

Purpose: Tracks origin and transformations.

Examples:

Source: “Extracted from ERP system X”

Transformation: “Aggregated daily, filtered by active customers”

Destination: “Loaded into Data Warehouse fact table”

Use case: Enables traceability, impact analysis, and debugging.

4. Who is responsible for the data asset? → Ownership & Stewardship Metadata

Purpose: Assigns accountability.

Examples:

Data Owner: Finance Department

Data Steward: Jane Doe, Data Quality Manager

Use case: Clarifies responsibility for quality, compliance, and issue resolution.

5. When was the data asset created and updated? → Temporal Metadata

Purpose: Captures timestamps and version history.

Examples:

Creation date: 2023-07-15

Last updated: 2025-09-01

Version: v2.3

Use case: Supports auditing, compliance, and time-sensitive decisions.

6. How can the data asset be used? → Administrative & Technical Metadata

Purpose: Defines usage constraints, format, and access methods.

Examples:

Format: Parquet, UTF-8

Access method: API endpoint / SQL schema

Security: “Contains personal data, GDPR applies”

Retention policy: “Keep for 7 years”

Use case: Guides safe, legal, and efficient data usage.


> In this seminar, we use **OpenMetadata** as the metadata management tool.
> 

## 2.4 Metadata management key stages

There are stages of metadata management:
 - Designing metadata model : Gathering requirements, and identifying which metadata need to be collected
 - Creating metadata: Gathering the metadata of essential data entities(e.g. file, table, data pipeline, etc.)
 - Storing metadata: Centralizing and standardizing metadata in a repository.
 - Using metadata: Providing tools to search/discover, understand and trace data by using metadata.
 - Auditing metadata: Check if the collected metadata is correct and fulfils the requirements.


## 3. What are the popular metadata management tools?


## 4. How to use Open-Metadata(OM) as a metadata management tool?
### 4.1 Metadata ingestion
#### 4.1.1 Load data entity
#### 4.1.2 Load Classification
#### 4.1.3 Load Glossary
#### 4.1.4 Load data lineage

### 4.2 Use metadata
####  4.2.1 Discover data with keywords

Suppose I am a newcomer, and all I know is that the data is about `hospital in french communes`. 

#### 4.2.2 Use the lineage metadata to trace data provenance 

#### 4.2.3 Collaboration 

Announcements, tasks, Activity feed, and team conversations







