# Sample FDE Interview Problem

## Design a Customer Support AI Agent

### Scenario
A company wants an AI agent that can assist support teams using:

- Customer records stored in Snowflake
- Internal policy documents
- Previous support transcripts
- Case notes

### Requirements
Design a system that can:

1. Retrieve relevant customer information.
2. Retrieve applicable company policies.
3. Generate grounded responses.
4. Escalate uncertain or high-risk cases.
5. Log decisions for auditing.
6. Measure response quality and business impact.

### Discuss

#### Architecture
- What services are required?
- Where should retrieval happen?
- How should the LLM be invoked?
- Which parts should be synchronous vs asynchronous?

#### Retrieval
- How should documents be chunked?
- Which metadata is important?
- When should keyword retrieval complement vector retrieval?
- Would reranking help?

#### Tool Calling
- Which tools should the agent have?
- How are permissions enforced?
- How do you validate tool arguments?

#### Safety and Security
- How do you prevent data leakage?
- How do you protect against prompt injection?
- Which actions require human approval?

#### Evaluation
Define metrics for:
- Groundedness
- Retrieval quality
- Resolution rate
- Escalation quality
- Latency
- Cost

#### Reliability
Explain how you would handle:
- Model API failures
- Timeouts
- Partial tool failures
- Stale data
- Retrieval failures
- Duplicate requests

### Interview Goal
The goal is not to produce one perfect architecture. Explain assumptions, ask clarifying questions, identify trade-offs, and connect technical decisions to business outcomes.
