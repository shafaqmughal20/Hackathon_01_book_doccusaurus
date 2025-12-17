<!--
Sync Impact Report:
Version change: N/A → 1.0.0
Modified principles:
- Spec-Driven Development: New principle added
- AI-Assisted Authoring: New principle added
- Reproducibility: New principle added
- Clean Separation of Concerns: New principle added
- Production-Ready Deployment: New principle added
- Technical Writing Clarity: New principle added
Added sections: Stack and Infrastructure Standards, Development Workflow
Removed sections: None
Templates requiring updates:
- .specify/templates/plan-template.md ✅ updated to reflect new principles
- .specify/templates/spec-template.md ✅ updated to reflect new principles
- .specify/templates/tasks-template.md ✅ updated to reflect new principles
- .specify/templates/commands/*.md ⚠ pending review
Follow-up TODOs: None
-->

# AI-Native Unified Book with Embedded RAG Chatbot Constitution

## Core Principles

### Spec-Driven Development
All development follows Spec-Kit Plus methodology with formal specifications, plans, and testable tasks; Every feature must have clear acceptance criteria before implementation begins; Accuracy and consistency across content, code, and deployment are maintained through structured artifacts.

### AI-Assisted Authoring
Claude Code and AI tools are leveraged for development with human-verifiable outputs; Technical claims must be internally consistent and verifiable through automated checks; All code and content must be reviewable and modifiable by humans.

### Reproducibility
All steps must be scripted, documented, and deployable in any environment; Build and deployment processes must be deterministic and repeatable; Production environments must be identical to development configurations.

### Clean Separation of Concerns
Clear separation between content, retrieval, and generation layers; Book content layer (Docusaurus), RAG retrieval layer (Qdrant), and AI generation layer (OpenAI Agents) must be independently maintainable; Dependencies between layers must be well-defined and minimal.

### Production-Ready Deployment
All implementations must be deployable on GitHub Pages for book content and production-grade API services for chatbot; No hard-coded secrets allowed; Environment-based configuration required for all deployments.

### Technical Writing Clarity
Content must be clear and accessible for AI, software, and robotics learners; Documentation must be precise and technically accurate; Code comments and documentation must enhance understanding for educational purposes.

## Stack and Infrastructure Standards

- Book authored in Docusaurus and deployed on GitHub Pages
- Chatbot stack: OpenAI Agents / ChatKit SDKs, FastAPI backend
- Neon Serverless Postgres for metadata & sessions
- Qdrant Cloud Free Tier for vector search
- Single unified repository (book + chatbot)
- No hard-coded secrets; environment-based configuration
- Clear setup, build, and deployment instructions

## Development Workflow

- All content structured, versioned, and generated via Spec-Kit Plus
- RAG chatbot must answer questions about the full book and questions based only on user-selected text
- Clear technical writing for AI, software, and robotics learners
- End-to-end reproducible build and deployment process

## Governance

- Constitution supersedes all other practices and must be followed strictly
- All PRs/reviews must verify compliance with Spec-Kit Plus methodology
- Amendments require documentation, approval, and migration plan
- Version changes must follow semantic versioning principles
- Compliance reviews must be conducted regularly

**Version**: 1.0.0 | **Ratified**: 2025-12-17 | **Last Amended**: 2025-12-17
