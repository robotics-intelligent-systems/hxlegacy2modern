# JFXLEGACY2MODERN — AI-Powered Legacy Software Modernization Platform

[![Architecture](https://img.shields.io/badge/architecture-AI--Driven%20Modernization-blue.svg)](#architecture)
[![AI Agents](https://img.shields.io/badge/AI-Agentic%20Engineering-purple.svg)](#ai-agent-platform)
[![Legacy Modernization](https://img.shields.io/badge/legacy-modernization-orange.svg)](#legacy-modernization)
[![Open Source](https://img.shields.io/badge/open-source-green.svg)](#license)
[![MBSE](https://img.shields.io/badge/MBSE-SysML%20%7C%20Arcadia-lightgrey.svg)](#mbse-and-software-architecture)

> **Open-source AI agent architecture for analyzing, refactoring, migrating and modernizing legacy software systems from one development framework, language or architectural paradigm to another.**

---

## Table of Contents

- [Description and Context](#description-and-context)
- [Problem Statement](#problem-statement)
- [Objectives](#objectives)
- [Functional Scope](#functional-scope)
- [Architecture](#architecture)
- [AI Agent Platform](#ai-agent-platform)
- [Legacy Modernization Pipeline](#legacy-modernization-pipeline)
- [Software Analysis](#software-analysis)
- [Code Transformation](#code-transformation)
- [Architecture Recovery](#architecture-recovery)
- [Target Architecture Generation](#target-architecture-generation)
- [Multi-Agent Modernization](#multi-agent-modernization)
- [Software Dependency Compendium](#software-dependency-compendium)
- [Dependency Classification](#dependency-classification)
- [Dependency Matrix](#dependency-matrix)
- [Recommended Technology Stack](#recommended-technology-stack)
- [MBSE and Software Architecture](#mbse-and-software-architecture)
- [User Guide](#user-guide)
- [Installation Guide](#installation-guide)
- [Docker Architecture](#docker-architecture)
- [Kubernetes Deployment](#kubernetes-deployment)
- [Security](#security)
- [Testing and Validation](#testing-and-validation)
- [Repository Structure](#repository-structure)
- [CI/CD](#cicd)
- [Contribution](#contribution)
- [Code of Conduct](#code-of-conduct)
- [Authors](#authors)
- [Additional Information](#additional-information)
- [License](#license)
- [Roadmap](#roadmap)

---

# Description and Context

**JFXLEGACY2MODERN** is an open-source AI-powered software modernization platform.

Its primary purpose is to automate or assist the migration of legacy software from an existing implementation technology toward a modern target architecture.

The current repository describes the project as an **open-source AI agent that modernizes legacy code from one development framework to another**.

The repository also references technologies and projects related to:

- AI coding agents
- agent-oriented programming
- legacy Java modernization
- automated refactoring
- software architecture recovery
- code quality analysis
- multi-agent systems
- LangGraph
- AutoGen
- OpenHands
- Haystack
- Dify
- JADE
- MBSE
- Arcadia
- Capella
- CAD
- CAM
- CAS

This makes the project suitable as a foundation for a broader **AI Software Modernization Engineering Platform**.

---

# Problem Statement

Legacy systems frequently contain:

- obsolete frameworks
- unsupported dependencies
- outdated programming languages
- monolithic architectures
- tightly coupled modules
- undocumented business rules
- obsolete APIs
- unsupported operating systems
- obsolete build systems
- insufficient test coverage
- architectural drift
- duplicated code
- undocumented integrations

Traditional modernization projects require significant manual effort.

Typical migration activities include:

```text
Legacy System
     │
     ▼
Source Analysis
     │
     ▼
Architecture Recovery
     │
     ▼
Dependency Analysis
     │
     ▼
Business Rule Extraction
     │
     ▼
Refactoring
     │
     ▼
Target Architecture
     │
     ▼
Code Transformation
     │
     ▼
Testing
     │
     ▼
Validation
     │
     ▼
Production Migration
```

JFXLEGACY2MODERN introduces AI agents into this lifecycle.

---

# Objectives

## Primary Objectives

1. Analyze legacy source code automatically.
2. Recover implicit software architecture.
3. Identify obsolete dependencies.
4. Extract business rules.
5. Detect technical debt.
6. Generate modernization plans.
7. Refactor source code.
8. Translate code between frameworks.
9. Generate target architecture.
10. Generate tests for migrated code.
11. Validate semantic equivalence.
12. Maintain traceability between legacy and modern implementations.

---

# Modernization Philosophy

The platform should follow these principles:

- **Understand before transforming**
- **Preserve business behavior**
- **Automate repetitive transformations**
- **Keep humans in control of architectural decisions**
- **Generate tests before risky transformations**
- **Maintain traceability**
- **Prefer incremental modernization**
- **Support rollback**
- **Measure modernization quality**

---

# Functional Scope

JFXLEGACY2MODERN can support the following capabilities.

## Legacy Code Analysis

- source parsing
- AST generation
- dependency discovery
- call graph generation
- package analysis
- class analysis
- method analysis
- complexity analysis
- code smell detection

## Architecture Recovery

- component identification
- service identification
- dependency graph
- module boundaries
- architectural patterns
- coupling analysis
- cohesion analysis

## AI-Assisted Refactoring

- rename
- extract method
- extract class
- dependency replacement
- API migration
- framework migration
- design pattern transformation

## Framework Migration

Examples:

```text
Legacy Java Framework
        │
        ▼
AI Analysis
        │
        ▼
Intermediate Representation
        │
        ▼
Target Architecture
        │
        ▼
Modern Java Framework
```

Potential targets:

- Spring Boot
- Quarkus
- Micronaut
- Jakarta EE
- REST APIs
- microservices
- event-driven systems

---

# Architecture

## High-Level Architecture

```text
                       ┌─────────────────────┐
                       │     Developer       │
                       │    / Architect      │
                       └──────────┬──────────┘
                                  │
                                  ▼
                       ┌─────────────────────┐
                       │ Modernization UI    │
                       │ CLI / Web / IDE     │
                       └──────────┬──────────┘
                                  │
                                  ▼
                       ┌─────────────────────┐
                       │ Modernization API   │
                       └──────────┬──────────┘
                                  │
                                  ▼
                 ┌────────────────────────────────┐
                 │      AI Agent Orchestrator     │
                 │                                │
                 │ LangGraph / AutoGen / AOP      │
                 └───────────────┬────────────────┘
                                 │
          ┌──────────────────────┼──────────────────────┐
          │                      │                      │
          ▼                      ▼                      ▼
 ┌────────────────┐     ┌────────────────┐     ┌────────────────┐
 │ Code Analysis  │     │ Architecture   │     │ Transformation │
 │ Agent          │     │ Agent          │     │ Agent          │
 └───────┬────────┘     └───────┬────────┘     └───────┬────────┘
         │                      │                      │
         └──────────────────────┼──────────────────────┘
                                │
                                ▼
                    ┌─────────────────────────┐
                    │ Knowledge / Vector DB   │
                    │ PostgreSQL / Qdrant     │
                    └────────────┬────────────┘
                                 │
                                 ▼
                    ┌─────────────────────────┐
                    │ Legacy Source Repository │
                    └────────────┬────────────┘
                                 │
                                 ▼
                    ┌─────────────────────────┐
                    │ Modernized Source Code   │
                    └─────────────────────────┘
```

---

# AI Agent Platform

The modernization engine should use multiple specialized agents rather than one monolithic AI agent.

## Agent Roles

### Repository Discovery Agent

Responsibilities:

- inspect repository
- identify programming languages
- identify build tools
- detect frameworks
- identify configuration files
- identify databases
- identify external APIs

### Code Analysis Agent

Responsibilities:

- AST analysis
- dependency analysis
- complexity analysis
- code smell detection
- architectural pattern detection

### Architecture Recovery Agent

Responsibilities:

- generate component diagrams
- generate dependency graphs
- identify architectural layers
- detect monolith boundaries
- identify candidate services

### Business Rule Agent

Responsibilities:

- infer business rules
- identify domain entities
- identify workflows
- identify validations
- identify business constraints

### Modernization Planner Agent

Produces:

```text
Current State
     │
     ▼
Modernization Gap
     │
     ▼
Target Architecture
     │
     ▼
Migration Strategy
     │
     ▼
Migration Tasks
```

### Code Transformation Agent

Responsible for:

- code translation
- API migration
- framework migration
- dependency replacement
- refactoring

### Test Generation Agent

Generates:

- unit tests
- integration tests
- regression tests
- characterization tests
- contract tests

### Validation Agent

Compares:

```text
Legacy Behavior
       │
       ▼
Test Oracle
       │
       ▼
Modern Behavior
       │
       ▼
Semantic Comparison
```

---

# Legacy Modernization Pipeline

```text
┌─────────────────────┐
│ Legacy Repository   │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ Repository Discovery│
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ Static Analysis     │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ Architecture Mining │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ Business Analysis   │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ Modernization Plan  │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ Code Transformation │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ Test Generation     │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ Validation          │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ Modernized System   │
└─────────────────────┘
```

---

# Software Analysis

## Static Analysis

The platform should analyze:

- source files
- AST
- imports
- dependencies
- inheritance
- interfaces
- annotations
- configuration
- build files
- deployment descriptors

## Metrics

Recommended metrics:

| Metric | Purpose |
|---|---|
| Cyclomatic Complexity | Complexity |
| Coupling | Architecture |
| Cohesion | Modularity |
| LOC | Size |
| Duplication | Technical debt |
| Dependency Count | Maintainability |
| Code Smells | Quality |
| Test Coverage | Safety |
| API Usage | Migration complexity |

---

# Architecture Recovery

The platform should reconstruct an architecture model from source code.

Example:

```text
Legacy Monolith
│
├── Presentation
│
├── Business Logic
│
├── Persistence
│
├── Integration
│
└── Shared Utilities
```

AI can then propose:

```text
Modern Architecture
│
├── API Gateway
│
├── Customer Service
│
├── Order Service
│
├── Payment Service
│
├── Notification Service
│
└── Data Services
```

The architecture proposal must remain subject to human architectural approval.

---

# Code Transformation

## Transformation Strategies

### 1. Syntax Transformation

```text
Legacy Syntax
      ↓
AST
      ↓
Modern Syntax
```

### 2. API Transformation

```text
Legacy API
    ↓
Mapping Rules
    ↓
Modern API
```

### 3. Framework Transformation

```text
Legacy Framework
       ↓
Framework Knowledge Base
       ↓
Modern Framework
```

### 4. Architectural Transformation

```text
Monolith
   ↓
Domain Analysis
   ↓
Bounded Contexts
   ↓
Services
```

---

# Intermediate Representation

A key architectural capability should be an intermediate software representation.

```text
Source Code
     │
     ▼
Language Parser
     │
     ▼
AST
     │
     ▼
Semantic Model
     │
     ▼
Architecture Model
     │
     ▼
Target Code
```

The intermediate model enables multiple source-to-target transformations.

For example:

```text
Java Legacy
      │
      ▼
Intermediate Model
      │
      ├──► Spring Boot
      │
      ├──► Quarkus
      │
      ├──► Micronaut
      │
      └──► Jakarta EE
```

---

# Software Dependency Compendium

The following compendium organizes the technologies referenced by JFXLEGACY2MODERN into functional categories.

The reference template specifically recommends documenting libraries, frameworks, databases, external resources, licenses and tested versions, together with build/runtime requirements and testing procedures.

---

## 1. AI Agent Frameworks

| Technology | Function | Classification |
|---|---|---|
| LangGraph | Stateful agent orchestration | Core |
| AutoGen | Multi-agent applications | Core/Optional |
| OpenHands | Autonomous coding agent | Optional |
| OpenRoom | AI interaction with applications | Research |
| Dify | LLM application platform | Optional |
| Haystack | AI/RAG orchestration | Optional |
| Agent Zero | Autonomous agent framework | Research |
| Uni-Agent | General agent framework | Research |
| SRE | Production AI agent runtime/SDK | Research |

The current repository explicitly references LangGraph, AutoGen, OpenHands, Dify, Haystack, Agent Zero, Uni-Agent and other agent-oriented systems.

---

# 2. AI Coding Agents

Potential components include:

- OpenHands
- OpenCode
- Codex CLI
- Kilo
- VibeCoder
- ReforgeAI
- ScreenCoder
- Warp
- Agent S

These technologies can be used as references or integration candidates for autonomous coding workflows.

---

# 3. Legacy Modernization

The modernization compendium includes:

| Tool | Purpose |
|---|---|
| Legacy2Modern | Legacy modernization |
| Going Merry | Legacy Java migration |
| Coca | Legacy refactoring |
| ReforgeAI | AI Java modernization |
| DesigniteJava | Java architecture/code quality |

These tools can be used for:

- migration analysis
- refactoring
- architectural assessment
- code quality
- modernization benchmarking

The repository explicitly references Going Merry, Coca, DesigniteJava, Legacy2Modern and ReforgeAI.

---

# 4. Source Code Analysis

Recommended technologies:

- Tree-sitter
- Eclipse JDT
- JavaParser
- Spoon
- PMD
- SpotBugs
- Checkstyle
- SonarQube / SonarCloud
- Semgrep
- CodeQL

Capabilities:

```text
Source
 ↓
Parser
 ↓
AST
 ↓
Semantic Analysis
 ↓
Dependency Graph
 ↓
Quality Metrics
```

---

# 5. Software Architecture Analysis

Recommended technologies:

- DesigniteJava
- SonarQube
- ArchUnit
- jQAssistant
- Structure101
- Graphviz
- NetworkX

Architecture models can represent:

- dependencies
- packages
- services
- modules
- interfaces
- databases
- APIs

---

# 6. Graph Analysis

Graph technologies:

- NetworkX
- Neo4j
- Graphviz
- Apache TinkerPop

Possible graph types:

```text
Dependency Graph
Call Graph
Class Graph
Package Graph
Service Graph
Data Flow Graph
Architecture Graph
```

---

# 7. LLM Infrastructure

Potential model infrastructure:

| Component | Purpose |
|---|---|
| Ollama | Local LLM execution |
| vLLM | High-performance inference |
| OpenLLM | Model serving |
| Hugging Face Transformers | Model integration |
| llama.cpp | Local inference |
| ONNX Runtime | Optimized inference |
| OpenVINO | Hardware optimization |

---

# 8. Code LLMs

Potential model families:

- Code Llama
- StarCoder
- Qwen-Coder
- DeepSeek-Coder
- Granite Code
- CodeGemma

Selection criteria:

- code generation quality
- context length
- programming-language coverage
- license
- inference requirements
- benchmark performance
- security

---

# 9. RAG and Knowledge Management

Recommended stack:

| Component | Function |
|---|---|
| Qdrant | Vector search |
| PostgreSQL | Structured metadata |
| pgvector | Relational vector search |
| Elasticsearch | Full-text search |
| OpenSearch | Search |
| FAISS | Local vector index |
| Chroma | Development vector DB |

RAG can provide agents with:

- framework documentation
- API migration guides
- legacy code patterns
- architecture standards
- coding rules
- modernization playbooks

---

# 10. Knowledge Graph

A knowledge graph can represent:

```text
Legacy Framework
      │
      ├── Version
      ├── APIs
      ├── Dependencies
      ├── Known Issues
      └── Migration Rules
```

Candidate technologies:

- Neo4j
- NetworkX
- Apache TinkerPop
- RDF
- SPARQL

---

# 11. Software Build Systems

Legacy systems frequently depend on multiple build technologies.

### Java

- Maven
- Gradle
- Ant

### JavaScript

- npm
- Yarn
- pnpm

### Python

- pip
- Poetry
- uv

### .NET

- MSBuild
- NuGet

### C/C++

- CMake
- Make
- Ninja
- Conan
- vcpkg

The modernization agent should automatically detect build systems.

---

# 12. Java Modernization

Java is a primary candidate for modernization.

Recommended tools:

- JavaParser
- Eclipse JDT
- Spoon
- OpenRewrite
- ArchUnit
- Maven
- Gradle
- JUnit
- Mockito
- Testcontainers

Potential transformations:

```text
Java EE
   ↓
Jakarta EE

Legacy Spring
   ↓
Spring Boot

Servlet Application
   ↓
REST API

Monolith
   ↓
Modular Monolith
   ↓
Microservices
```

---

# 13. OpenRewrite

OpenRewrite can serve as a deterministic transformation engine.

Recommended architecture:

```text
AI Agent
    │
    ▼
Transformation Plan
    │
    ▼
OpenRewrite Recipe
    │
    ▼
Source Transformation
    │
    ▼
Compilation
    │
    ▼
Tests
```

AI should generate or select transformations, while deterministic rewrite engines execute predictable source changes.

---

# 14. Testing Frameworks

Recommended:

- JUnit
- Mockito
- Testcontainers
- pytest
- Jest
- Playwright
- Cypress
- REST Assured

Testing strategy:

```text
Characterization Tests
        ↓
Transformation
        ↓
Regression Tests
        ↓
Integration Tests
        ↓
Behavior Comparison
```

---

# 15. Containerization

Recommended:

- Docker
- Docker Compose
- Podman
- BuildKit
- OCI

Containers provide reproducible execution environments during migration.

---

# 16. Kubernetes

Potential deployment technologies:

- Kubernetes
- Helm
- Kustomize
- Argo CD
- Flux
- Istio

Modernization workloads can execute as isolated jobs:

```text
Kubernetes
│
├── Analysis Job
├── Architecture Job
├── Transformation Job
├── Compilation Job
├── Test Job
└── Validation Job
```

---

# 17. CI/CD

Recommended:

- GitHub Actions
- GitLab CI
- Jenkins
- Tekton
- Argo CD

Example pipeline:

```text
Commit
  ↓
Build
  ↓
Static Analysis
  ↓
AI Modernization Agent
  ↓
Transformation
  ↓
Compile
  ↓
Unit Tests
  ↓
Integration Tests
  ↓
Security Scan
  ↓
Artifact
  ↓
Deployment
```

---

# 18. Security

Recommended technologies:

- Keycloak
- OAuth 2.0
- OpenID Connect
- HashiCorp Vault
- Azure Key Vault
- Trivy
- Semgrep
- CodeQL

AI modernization requires additional controls for:

- source-code confidentiality
- credentials
- secrets
- proprietary business logic
- dependency integrity
- generated-code validation

---

# 19. Observability

Recommended:

- OpenTelemetry
- Prometheus
- Grafana
- Jaeger
- Langfuse

AI-specific metrics:

```text
Agent Execution Time
Token Consumption
Model Latency
Transformation Success Rate
Compilation Success Rate
Test Success Rate
Rollback Rate
Human Approval Rate
```

---

# 20. Documentation and Architecture Modeling

Recommended:

- Mermaid
- PlantUML
- Draw.io
- Graphviz
- Structurizr
- SysML
- Arcadia
- Capella

The repository itself includes an `MBSE/CAS` structure and references Arcadia/Capella, CAD, CAM and CAS.

---

# Dependency Classification

Each dependency should receive one of these classifications:

| Type | Description |
|---|---|
| Core | Essential to the platform |
| Runtime | Required at execution time |
| Build | Required to compile |
| Development | Developer tooling |
| Test | Testing |
| AI | AI/LLM component |
| Agent | Agent orchestration |
| Analysis | Static/semantic analysis |
| Transformation | Code migration |
| Integration | External system |
| Infrastructure | Deployment |
| Security | Security |
| Observability | Monitoring |
| Research | Experimental |
| Reference | Comparative technology |
| Legacy | Compatibility |
| Deprecated | Not recommended |

---

# Dependency Specification Template

```yaml
name:
category:
dependency_type:

purpose:

repository:
official_website:

license:
license_compatibility:

programming_language:
version_tested:

installation:
runtime_requirements:
build_requirements:

api:
protocols:
data_formats:

input_formats:
output_formats:

integration:
ai_integration:
agent_integration:
rag_integration:
mbse_integration:

security_considerations:
privacy_considerations:

performance_considerations:
hardware_requirements:
operating_systems:

container_support:
kubernetes_support:

testing:
documentation:

status:
maintenance_status:
last_review:
```

---

# Dependency Matrix

| Technology | Category | Core | Main Purpose |
|---|---|---:|---|
| LangGraph | Agent | Yes | Agent orchestration |
| AutoGen | Agent | Optional | Multi-agent workflows |
| OpenHands | Coding Agent | Optional | Autonomous coding |
| Haystack | AI/RAG | Optional | AI orchestration |
| Dify | AI Platform | Optional | LLM applications |
| Legacy2Modern | Modernization | Reference | Legacy migration |
| Going Merry | Modernization | Reference | Java migration |
| Coca | Modernization | Reference | Refactoring |
| DesigniteJava | Analysis | Recommended | Architecture analysis |
| OpenRewrite | Transformation | Recommended | Deterministic refactoring |
| JavaParser | Analysis | Recommended | Java parsing |
| Eclipse JDT | Analysis | Recommended | Java AST |
| Spoon | Analysis | Optional | Java transformation |
| SonarQube | Quality | Recommended | Code quality |
| Tree-sitter | Parsing | Recommended | Multi-language parsing |
| NetworkX | Graph | Recommended | Dependency graphs |
| Neo4j | Graph | Optional | Knowledge graph |
| Qdrant | RAG | Optional | Vector search |
| PostgreSQL | Data | Recommended | Metadata/state |
| Ollama | LLM | Optional | Local inference |
| vLLM | LLM | Optional | Production inference |
| Transformers | LLM | Recommended | Model integration |
| OpenRewrite | Transformation | Recommended | Source migration |
| JUnit | Testing | Recommended | Java testing |
| Testcontainers | Testing | Recommended | Integration testing |
| Docker | Infrastructure | Recommended | Containers |
| Kubernetes | Infrastructure | Production | Orchestration |
| Helm | Infrastructure | Recommended | Packaging |
| OpenTelemetry | Observability | Recommended | Telemetry |
| Prometheus | Observability | Recommended | Metrics |
| Grafana | Observability | Recommended | Dashboards |
| Langfuse | AI Observability | Optional | LLM tracing |

---

# Recommended Technology Stack

```yaml
platform:

  interface:
    - CLI
    - Web UI
    - IDE Plugin

  backend:
    - Python
    - FastAPI

  agent_orchestration:
    - LangGraph
    - AutoGen

  code_analysis:
    - Tree-sitter
    - JavaParser
    - Eclipse JDT
    - Spoon

  architecture_analysis:
    - DesigniteJava
    - ArchUnit
    - NetworkX
    - Graphviz

  transformation:
    - OpenRewrite
    - AST transformations
    - LLM-generated transformations

  llm:
    - Ollama
    - vLLM
    - Hugging Face Transformers

  code_models:
    - Qwen-Coder
    - DeepSeek-Coder
    - StarCoder
    - Code Llama

  knowledge:
    - PostgreSQL
    - Qdrant
    - Neo4j

  testing:
    - JUnit
    - Mockito
    - Testcontainers
    - pytest

  security:
    - Keycloak
    - OAuth2
    - OpenID Connect
    - Vault

  infrastructure:
    - Docker
    - Kubernetes
    - Helm

  observability:
    - OpenTelemetry
    - Prometheus
    - Grafana
    - Langfuse
```

---

# MBSE and Software Architecture

JFXLEGACY2MODERN can extend beyond source-code transformation toward **model-based modernization**.

The current project already contains an `MBSE/CAS` structure and references Arcadia, Capella, CAD, CAM and CAS.

## Model-Based Modernization

```text
Legacy Software
       │
       ▼
Source Analysis
       │
       ▼
Architecture Model
       │
       ▼
System Model
       │
       ▼
Target Architecture
       │
       ▼
Modern Implementation
```

Potential models:

- UML
- SysML
- Arcadia
- AADL
- C4
- BPMN
- Architecture Decision Records

---

# Digital Engineering Integration

A future architecture may connect:

```text
Software Engineering
        │
        ▼
JFXLEGACY2MODERN
        │
 ┌──────┼────────┐
 │      │        │
 ▼      ▼        ▼
MBSE   CAD      CAS
 │      │        │
 ▼      ▼        ▼
System Engineering
```

This allows modernization decisions to consider not only source code but also system-level engineering constraints.

---

# User Guide

## Step 1 — Select a Legacy Repository

```bash
git clone <legacy-repository>
```

## Step 2 — Analyze the Repository

Run the discovery process:

```bash
legacy2modern analyze ./legacy-system
```

The system should identify:

- language
- framework
- build system
- dependencies
- architecture
- tests
- databases
- APIs

## Step 3 — Generate Architecture Report

```bash
legacy2modern architecture ./legacy-system
```

Expected output:

```text
architecture/
├── components.md
├── dependencies.graphml
├── call-graph.graphml
├── architecture.drawio
└── architecture-report.md
```

## Step 4 — Generate Modernization Plan

```bash
legacy2modern plan \
  --source legacy-java \
  --target spring-boot
```

## Step 5 — Generate Transformation

```bash
legacy2modern migrate \
  --source ./legacy \
  --target ./modern
```

## Step 6 — Execute Tests

```bash
legacy2modern validate ./modern
```

---

# Installation Guide

## Requirements

Recommended development environment:

```text
Operating System:
  Linux
  macOS
  Windows + WSL2

Version Control:
  Git

Languages:
  Python 3.x
  Java 17+

Build:
  Maven
  Gradle

Containers:
  Docker
  Docker Compose

Optional:
  Kubernetes
  NVIDIA GPU
```

Exact versions used for a release should be recorded in the dependency matrix before declaring a build reproducible.

---

# Installation

Clone the repository:

```bash
git clone https://github.com/robotics-intelligent-systems/jfxlegacy2modern.git
cd jfxlegacy2modern
```

Create the development environment:

```bash
python -m venv .venv
source .venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the application:

```bash
python -m jfxlegacy2modern
```

If a Docker environment is provided:

```bash
docker compose up -d
```

---

# Docker Architecture

```text
jfxlegacy2modern/
│
├── frontend/
│
├── api/
│
├── agents/
│   ├── discovery/
│   ├── analysis/
│   ├── architecture/
│   ├── modernization/
│   ├── transformation/
│   ├── testing/
│   └── validation/
│
├── analyzers/
│
├── transformers/
│
├── knowledge/
│
├── models/
│
├── tests/
│
├── docker/
│
└── kubernetes/
```

---

# Kubernetes Deployment

A production deployment can execute modernization jobs independently.

```text
Kubernetes Cluster
│
├── API Gateway
│
├── Agent Orchestrator
│
├── Analysis Workers
│
├── Transformation Workers
│
├── Test Workers
│
├── Validation Workers
│
├── LLM Gateway
│
├── Vector Database
│
├── PostgreSQL
│
└── Observability
```

## Job-Based Modernization

Each modernization request becomes a workflow:

```text
Modernization Request
        │
        ▼
Kubernetes Job
        │
        ├── Analysis
        ├── Architecture
        ├── Planning
        ├── Transformation
        ├── Compilation
        ├── Testing
        └── Validation
```

This approach allows multiple modernization projects to run independently.

---

# Security

Legacy source code can contain highly sensitive information.

Security controls should include:

- source isolation
- private model deployment
- encryption
- access control
- audit logs
- secrets management
- network isolation
- container scanning
- dependency scanning
- generated-code review

## Source Code Privacy

For confidential systems:

```text
Enterprise Repository
        │
        ▼
Private AI Infrastructure
        │
        ├── Local LLM
        ├── Private Vector DB
        └── Private Agent Runtime
```

External AI providers should only receive source code when explicitly authorized.

---

# AI Safety

AI-generated modernization must not be treated as automatically correct.

Every transformation should pass through:

```text
AI Proposal
     │
     ▼
Deterministic Transformation
     │
     ▼
Compilation
     │
     ▼
Automated Tests
     │
     ▼
Static Analysis
     │
     ▼
Human Review
     │
     ▼
Approval
```

---

# Testing and Validation

## Characterization Testing

Before migration:

```text
Legacy Application
       │
       ▼
Characterization Tests
       │
       ▼
Behavior Baseline
```

The baseline becomes the reference for the modern implementation.

## Regression Testing

```text
Legacy
  │
  ├── Test A
  ├── Test B
  └── Test C
          │
          ▼
Modern
  │
  ├── Test A
  ├── Test B
  └── Test C
```

## Semantic Validation

The system should compare:

- outputs
- exceptions
- database effects
- API responses
- state changes
- performance

---

# Modernization Quality Metrics

| Metric | Objective |
|---|---|
| Compilation Success | Build reliability |
| Test Pass Rate | Functional correctness |
| Code Coverage | Test quality |
| Complexity Reduction | Maintainability |
| Dependency Reduction | Technical debt |
| Vulnerability Reduction | Security |
| Duplication Reduction | Quality |
| Architecture Compliance | Target architecture |
| Transformation Success | Automation quality |
| Human Approval Rate | Trust |

---

# CI/CD

Recommended pipeline:

```text
Git Push
   │
   ▼
Static Analysis
   │
   ▼
Dependency Scan
   │
   ▼
AI Analysis
   │
   ▼
Modernization Plan
   │
   ▼
Transformation
   │
   ▼
Build
   │
   ▼
Unit Tests
   │
   ▼
Integration Tests
   │
   ▼
Security Tests
   │
   ▼
Architecture Validation
   │
   ▼
Human Approval
   │
   ▼
Release
```

---

# Repository Structure

Recommended structure:

```text
jfxlegacy2modern/
│
├── README.md
├── LICENSE
├── CONTRIBUTING.md
├── CODE-OF-CONDUCT.md
│
├── docs/
│   ├── architecture/
│   │   ├── adr/
│   │   ├── diagrams/
│   │   └── modernization/
│   │
│   ├── dependencies/
│   │   ├── software-compendium.md
│   │   └── dependency-matrix.csv
│   │
│   ├── agents/
│   ├── security/
│   └── testing/
│
├── src/
│   ├── api/
│   ├── agents/
│   │   ├── discovery/
│   │   ├── analysis/
│   │   ├── architecture/
│   │   ├── planning/
│   │   ├── transformation/
│   │   ├── testing/
│   │   └── validation/
│   │
│   ├── parsers/
│   ├── analyzers/
│   ├── transformers/
│   ├── models/
│   ├── knowledge/
│   └── security/
│
├── tests/
│   ├── unit/
│   ├── integration/
│   ├── characterization/
│   ├── transformation/
│   └── validation/
│
├── examples/
│   ├── java/
│   ├── spring/
│   ├── legacy/
│   └── modernization/
│
├── docker/
├── kubernetes/
└── helm/
```

---

# Architecture Decision Records

Modernization decisions should be documented.

Example:

```text
docs/architecture/adr/
├── ADR-001-agent-orchestration.md
├── ADR-002-intermediate-representation.md
├── ADR-003-code-transformation-engine.md
├── ADR-004-llm-provider.md
├── ADR-005-vector-database.md
├── ADR-006-modernization-testing.md
└── ADR-007-human-approval.md
```

Each ADR should include:

- Context
- Problem
- Decision
- Alternatives
- Consequences
- Security
- Operational impact

---

# Contribution

Contributions are welcome.

Typical contribution areas:

- source parsers
- language adapters
- framework migration recipes
- AI agents
- transformation engines
- test generation
- architecture analysis
- visualization
- MBSE integration
- documentation
- security

Recommended workflow:

```bash
git checkout -b feature/my-modernization-feature
```

Run tests:

```bash
pytest
```

Run static analysis:

```bash
ruff check .
```

Commit:

```bash
git commit -m "feat: add modernization analyzer"
```

Push:

```bash
git push origin feature/my-modernization-feature
```

Open a Pull Request.

---

# Code of Conduct

Contributors should:

- communicate respectfully
- provide constructive feedback
- protect confidential source code
- respect third-party licenses
- document AI-generated changes
- provide reproducible tests
- avoid introducing malicious transformations

The repository should maintain a `CODE-OF-CONDUCT.md` file.

---

# Authors

**Robotics Intelligent Systems**

Organization:

```text
https://github.com/robotics-intelligent-systems
```

Project:

```text
https://github.com/robotics-intelligent-systems/jfxlegacy2modern
```

Reference repository template:

```text
https://github.com/sdk2035/Plantilla-de-repositorio
```

---

# Additional Information

## Related Projects

JFXLEGACY2MODERN fits naturally into the broader Robotics Intelligent Systems software ecosystem.

```text
                         AI SOFTWARE ECOSYSTEM
                                  │
             ┌────────────────────┼────────────────────┐
             │                    │                    │
             ▼                    ▼                    ▼
        JFXAI4ARCH            JFXAI4NLP        JFXLEGACY2MODERN
        AI Platform           Language AI       Modernization AI
             │                    │                    │
             └────────────────────┼────────────────────┘
                                  │
                                  ▼
                         AI Engineering Platform
```

### JFXAI4ARCH

Provides:

- AI agents
- RAG
- MCP
- model infrastructure
- cloud-native architecture

### JFXAI4NLP

Provides:

- NLP
- LLM
- natural-language programming
- language intelligence

### JFXLEGACY2MODERN

Provides:

- legacy analysis
- code modernization
- architecture recovery
- AI-assisted migration
- software transformation

---

# Strategic Architecture

The projects can converge toward an integrated architecture:

```text
                     Enterprise Systems
                            │
                            ▼
                   ┌─────────────────┐
                   │ JFXAI4ARCH      │
                   │ AI Platform     │
                   └────────┬────────┘
                            │
          ┌─────────────────┼─────────────────┐
          │                 │                 │
          ▼                 ▼                 ▼
       NLP/LLM          Agents/MCP       Modernization
          │                 │                 │
          ▼                 ▼                 ▼
    JFXAI4NLP         AI Orchestration   JFXLEGACY2MODERN
                                              │
                                              ▼
                                       Legacy Systems
```

---

# Modernization Maturity Model

JFXLEGACY2MODERN can implement five maturity levels.

## Level 1 — Discovery

```text
Repository Inventory
```

## Level 2 — Analysis

```text
Code + Dependency + Architecture Analysis
```

## Level 3 — Assisted Modernization

```text
AI Suggestions + Human Review
```

## Level 4 — Automated Modernization

```text
AI Agents + Deterministic Transformations
```

## Level 5 — Autonomous Engineering

```text
Discovery
   ↓
Planning
   ↓
Transformation
   ↓
Testing
   ↓
Validation
   ↓
Deployment
```

Human approval remains available for high-risk decisions.

---

# Legacy-to-Modern Knowledge Graph

A long-term objective should be to maintain a knowledge graph connecting:

```text
Legacy Technology
      │
      ├── Version
      ├── API
      ├── Dependency
      ├── Vulnerability
      ├── Migration Recipe
      └── Modern Equivalent
```

Example:

```text
Java EE 7
   │
   ├── javax.*
   │
   ├── Servlet
   │
   └── JPA
        │
        ▼
Jakarta EE
   │
   ├── jakarta.*
   │
   ├── Modern Servlet
   │
   └── Jakarta Persistence
```

This knowledge can become a reusable modernization asset.

---

# License

The project's actual license must be explicitly maintained in the repository's `LICENSE` file.

Third-party dependencies must be reviewed individually.

The dependency inventory should record:

- license
- version
- repository
- compatibility
- redistribution requirements
- commercial-use conditions
- model license
- documentation

The reference template specifically requires the README to identify the project's license and recommends keeping the complete license text in a root-level license file.

---

# Dependency Governance

For every production dependency, maintain:

```text
Name
Version
Purpose
License
Repository
Official Documentation
Runtime Requirements
Build Requirements
Security Status
Known Vulnerabilities
Container Support
Kubernetes Support
AI Integration
Maintenance Status
Last Review
```

Recommended files:

```text
docs/dependencies/software-compendium.md
docs/dependencies/dependency-matrix.csv
```

---

# Roadmap

## Phase 1 — Repository Intelligence

- [ ] Repository discovery
- [ ] Language detection
- [ ] Build-system detection
- [ ] Dependency analysis
- [ ] Static analysis
- [ ] Architecture recovery

## Phase 2 — AI Modernization

- [ ] AI modernization planner
- [ ] Code transformation agents
- [ ] Framework migration agents
- [ ] Business rule extraction
- [ ] Test generation

## Phase 3 — Deterministic Transformation

- [ ] OpenRewrite integration
- [ ] AST transformation engine
- [ ] Migration recipes
- [ ] Compilation validation
- [ ] Automated rollback

## Phase 4 — Enterprise Modernization

- [ ] Private LLM infrastructure
- [ ] Enterprise repositories
- [ ] IAM integration
- [ ] Audit
- [ ] Governance
- [ ] Compliance

## Phase 5 — Autonomous Software Engineering

- [ ] Multi-agent modernization
- [ ] Architecture optimization
- [ ] Continuous technical-debt detection
- [ ] Automated modernization proposals
- [ ] Self-validating transformations
- [ ] Human-in-the-loop governance

---

# Conclusion

JFXLEGACY2MODERN can evolve from an AI-powered code migration tool into a complete **AI Software Modernization Engineering Platform**.

Its central architecture is:

```text
             LEGACY SYSTEM
                   │
                   ▼
          ┌─────────────────┐
          │ AI DISCOVERY     │
          └────────┬────────┘
                   ▼
          ┌─────────────────┐
          │ CODE ANALYSIS    │
          └────────┬────────┘
                   ▼
          ┌─────────────────┐
          │ ARCHITECTURE     │
          │ RECOVERY         │
          └────────┬────────┘
                   ▼
          ┌─────────────────┐
          │ MODERNIZATION    │
          │ PLANNING         │
          └────────┬────────┘
                   ▼
          ┌─────────────────┐
          │ AI TRANSFORMATION│
          └────────┬────────┘
                   ▼
          ┌─────────────────┐
          │ BUILD + TEST     │
          └────────┬────────┘
                   ▼
          ┌─────────────────┐
          │ SEMANTIC         │
          │ VALIDATION       │
          └────────┬────────┘
                   ▼
          ┌─────────────────┐
          │ MODERN SYSTEM    │
          └─────────────────┘
```

The strategic value of the platform is therefore not limited to generating new code. Its principal objective is to create a **traceable engineering process from legacy software discovery to validated modern architecture**, combining AI agents, deterministic transformations, software analysis, testing, architecture modeling and human governance.

---

## References

- JFXLEGACY2MODERN: https://github.com/robotics-intelligent-systems/jfxlegacy2modern
- Repository documentation template: https://github.com/sdk2035/Plantilla-de-repositorio
- Robotics Intelligent Systems: https://github.com/robotics-intelligent-systems