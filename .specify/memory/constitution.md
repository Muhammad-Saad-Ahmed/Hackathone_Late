<!--
Sync Impact Report:
- Version change: 1.0.0 → 2.0.0
- List of modified principles:
  - Principle 1: "Technical Accuracy" → "Spec-first"
  - Principle 2: "Hands-on Learning" → "Reproducibility"
  - Principle 3: "Clear, Structured Teaching" → "AI discipline"
  - Principle 4: "Consistent Python/ROS 2 Examples" → "Transparency"
  - Principles 5-9 removed.
- Added sections:
  - Book Standards
  - Tooling
  - RAG Chatbot Requirements
- Removed sections: None
- Templates requiring updates:
  - ✅ .specify/templates/plan-template.md
  - ✅ .specify/templates/spec-template.md
  - ✅ .specify/templates/tasks-template.md
- Follow-up TODOs: None
-->

# [PROJECT_NAME] Constitution

## Core Principles

### I. Spec-first
No content or code without an approved spec.

### II. Reproducibility
Builds and deployments must be deterministic.

### III. AI discipline
The designated AI agent (Claude Code) must implement specs precisely, without making unverified assumptions.

### IV. Transparency
All architecturally significant decisions and data flows must be documented in a transparent and accessible manner.

## Book Standards
- **Format**: The book will be authored in Docusaurus-compatible Markdown (MDX).
- **Audience**: The target audience is software developers with an interest in physical AI and robotics.
- **Chapter Structure**: Each chapter is required to contain the following sections:
  - Objective
  - Core concepts
  - Examples (where applicable)
  - Summary
  - Acceptance criteria

## Tooling
- **Spec-Kit Plus**: The single source of truth for all specifications.
- **Claude Code**: The designated AI agent for writing and implementation tasks.
- **Docusaurus**: The framework for building the book.
- **GitHub Pages**: The platform for hosting and deploying the final book.

## RAG Chatbot Requirements
- **Stack**:
  - **Backend**: FastAPI
  - **Database**: Neon Serverless Postgres
  - **Vector Store**: Qdrant Cloud (Free Tier)
  - **AI SDKs**: OpenAI Agents / ChatKit SDKs
- **Capabilities**:
  - The chatbot must only answer questions using the indexed content of the book.
  - It must support answering questions based solely on user-selected text from the book.
  - It must clearly indicate when an answer cannot be derived from the provided context.

## Constraints
- No undocumented customizations are permitted.
- The project must not rely on any private or proprietary datasets.
- All infrastructure must be compatible with free-tier service levels.

## Success Criteria
- The Docusaurus book must build and deploy successfully to GitHub Pages.
- All chapters must conform to their approved specifications.
- The RAG chatbot must function correctly, including its selection-based context feature.
- The chatbot must not provide answers that are hallucinated or derived from outside the retrieved content.

## Governance

This Constitution is the single source of truth for project principles and governance. All development activities, reviews, and artifacts must align with it. Amendments require a documented proposal, review, and an approved migration plan.

**Governing Rule**: If a feature, behavior, or component is not explicitly defined in a specification, it must not be implemented.

**Version**: 2.0.0 | **Ratified**: 2025-12-07 | **Last Amended**: 2025-12-19
