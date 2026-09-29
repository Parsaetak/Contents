# SHEYTAN-LA R&D DIRECTION & STRATEGIC ARCHITECTURE

### Research baseline: 29 September 2026

## 1. Strategic Objective

SHEYTAN-LA should evolve from a local software-engineering agent into a **user-owned AI platform** capable of competing at the product/system level with the capabilities users increasingly expect from ChatGPT, Claude, Gemini, and Grok.

The fundamental product is therefore no longer:

> “a local AI assistant that can code.”

It becomes:

> **“A system for creating, running, understanding, and continuously improving your own AI.”**

Every user should be able to build an AI system around their own:

* models
* hardware
* memory
* knowledge
* personality/instructions
* skills
* tools
* applications
* projects
* automations
* permissions
* evaluation criteria
* workflows
* feedback
* system-performance constraints

The model is only one component.

The long-term SHEYTAN-LA architecture should resemble an **AI operating environment**, where the user owns the intelligence stack rather than renting one fixed assistant.

---

# 2. What the Current Repository Already Gives Us

The v1.7.5 repository is a surprisingly strong foundation for this direction.

The important point is that most of the required primitives already exist.

### Runtime

SHEYTAN already has a single coherent Go runtime that wires the LLM, orchestrator, tools, memory, recall, research, repository intelligence, Coding Lab, scheduler, automation, native engine, and lifecycle management.

### Agent

The orchestrator already provides:

```text
planning
→ context resolution
→ generation
→ tool execution
→ tool results
→ iteration
→ failure handling
→ verification
→ settlement
```

It already contains bounded execution, tool policies, task classification, context tiers, telemetry, recovery, and run-control.

### Memory

The current memory architecture already distinguishes trust and provenance rather than treating every remembered statement as equally reliable.

The memory classes and recall system create the beginning of a real long-lived personal AI.

### Skills

SHEYTAN already has:

```text
JSON skills
+
SKILL.md packages
+
global/workspace/task scopes
+
progressive disclosure
+
verified-learning promotion
```

That is particularly important because reusable procedural knowledge is one of the foundations of a user-trained AI system.

### Tools

The project already supports:

```text
built-in tools
+
custom tools
+
task-scoped tools
+
tool permissions
+
bounded execution
+
MCP foundation
```

This means the future does not require another disconnected plugin architecture.

### Coding Lab

The Coding Lab already supplies:

```text
isolated execution
+
policy
+
build/test
+
verification
+
repair
+
artifacts
+
snapshots
```

This is precisely the infrastructure required for future **AI self-evaluation and self-improvement**.

### Automation

The existing scheduler has already evolved into a durable automation engine with recurring tasks, event triggers, task tools, skills, artifacts, and run history.

### Repository Intelligence

The repository index already provides:

```text
files
symbols
dependencies
test/source relationships
Git metadata
hybrid search
```

### Research

The unified research service already provides a foundation for external information gathering through the existing provider architecture.

### Native + llama.cpp

SHEYTAN already has two distinct serving paths:

```text
SHEYTAN Native Engine
llama.cpp
```

with shared backend/capability concepts and explicit fallback behavior.

### Evidence

Perhaps most importantly, the product already treats:

> model claims ≠ evidence.

That distinction should become the foundation of the future self-improvement architecture.

---

# 3. The Market Has Changed: Basic Agent Features Are Now Table Stakes

The current frontier products increasingly combine several capabilities instead of behaving as simple chatbots.

OpenAI's current ecosystem combines deep research, projects, memory, scheduled work, connected sources, files, and agentic workflows. Deep Research now supports explicit source selection, editable plans, progress tracking, interruption, and connected applications.

Anthropic has moved toward persistent workspaces, Artifacts, MCP, coding agents, and specialized research environments. Claude Science, for example, combines a coordinating agent, specialist agents, skills, connectors, auditable artifacts, code/environment provenance, and flexible compute resources.

Google's current agent direction includes computer use, long-horizon automation, Deep Research with MCP and native visualizations, and Canvas-based creation.

xAI's current direction is particularly relevant to SHEYTAN-LA: Grok 4.7 emphasizes long-running agents and extended work across coding, research, and knowledge work, while Grok Bot gives agents persistent computers, ongoing operation, memory, and the ability to return for approval only when needed.

The local ecosystem is also moving in the same direction. Open WebUI already exposes Models, Knowledge, Prompts, Skills, and Tools as composable building blocks. Jan now combines local models, projects, assistants, agents, skills, memory, and MCP; its Agent can read/edit projects, execute commands, search the web, use MCP, remember across sessions, delegate work, and pursue persistent goals.

LM Studio demonstrates another important trend: local inference itself is becoming an adaptive runtime problem, with JIT model loading, automatic unloading, tool use, MCP, and multiple API surfaces.

Therefore SHEYTAN should **not** define its competitive target as “add web search” or “add MCP” or “add agents.”

Those are necessary capabilities, but they are becoming infrastructure.

---

# 4. SHEYTAN's Differentiation

SHEYTAN should compete on a different axis:

## User-owned intelligence

The user should be able to construct an AI that is:

```text
personal
persistent
inspectable
modifiable
portable
local
model-independent
evidence-driven
resource-aware
self-improving
```

The central differentiator becomes:

> **Other products provide an AI. SHEYTAN provides the environment in which the user builds their AI.**

That creates a much larger architectural target.

---

# 5. Introduce the AI System as a First-Class Object

The most important future architectural change should be the introduction of a first-class **AI System** abstraction.

Today the product is centered around sessions, models, tools, skills, and tasks.

Future SHEYTAN should be centered around:

```text
AI SYSTEM
│
├── Identity
├── Instructions / behavior
├── Model policy
├── Model routing
├── Memory
├── Knowledge
├── Skills
├── Tools
├── Connectors
├── Permissions
├── Context policy
├── Runtime policy
├── Automations
├── Evaluation suite
├── Feedback
├── Performance profile
├── Improvement history
└── Version
```

An AI System should be exportable, versionable, clonable, inspectable, and rollback-capable.

A user could therefore have:

```text
Personal Assistant
Coding Architect
Research Analyst
Business Agent
Trading Research System
Creative Writer
Private Company Assistant
Game Development Agent
```

without SHEYTAN requiring a separate application for every identity.

---

# 6. SHEYTAN Must Have a Self-Model

This directly addresses the requirement that SHEYTAN should understand its own system and operate it near its practical peak.

The AI should have access to a controlled, machine-generated **self-model** describing the system's current reality.

Conceptually:

```text
SELF MODEL
│
├── Hardware
│   ├── CPU
│   ├── RAM
│   ├── GPU
│   ├── VRAM
│   └── NPU
│
├── Runtime
│   ├── active engine
│   ├── active model
│   ├── loaded resources
│   ├── current processes
│   └── current system pressure
│
├── Capabilities
│   ├── vision
│   ├── tools
│   ├── browser
│   ├── research
│   ├── coding
│   └── connectors
│
├── Constraints
│   ├── memory budget
│   ├── CPU pressure
│   ├── context budget
│   ├── permissions
│   └── network policy
│
├── Health
│   ├── engine state
│   ├── tool health
│   ├── storage health
│   └── recent failures
│
└── Learned state
    ├── successful strategies
    ├── failed strategies
    ├── user preferences
    └── verified improvements
```

The self-model must be **evidence-backed**.

It must never say:

> “I have a powerful GPU.”

when the only evidence is that Windows reported a GPU.

The existing SHEYTAN evidence philosophy should remain intact.

---

# 7. The Runtime Governor Is a Major New Core Subsystem

This should become one of the highest-priority R&D areas.

The system should continuously answer:

> **What is the best way for SHEYTAN to perform the current workload on this machine right now?**

Not merely:

> “How much RAM does the computer have?”

And not:

> “How much CPU can I consume?”

The objective should be:

> **maximize useful AI work subject to responsiveness, safety, thermal/power, memory, and user-defined constraints.**

## Runtime Governor

Proposed architecture:

```text
Telemetry
   ↓
Resource State
   ↓
Pressure Model
   ↓
Resource Envelope
   ↓
Runtime Decision
   ↓
Engine / Context / Tool / Scheduler actions
   ↓
Measure outcome
   ↓
Update model
```

The Governor should own policy, while existing subsystems remain the execution authorities.

It must not create a second engine manager or second scheduler.

---

# 8. Resource State Should Be Continuous, Not Binary

Instead of:

```text
RAM okay / RAM bad
CPU okay / CPU bad
```

SHEYTAN should maintain a continuously updated state.

For example:

```text
GREEN
YELLOW
ORANGE
RED
EMERGENCY
```

The exact thresholds should be **measured and hysteresis-protected**, not arbitrary constants.

### Green

Normal operation:

```text
full context
background indexing
prewarm allowed
calibration allowed
normal automation
normal parallelism
```

### Yellow

Some pressure:

```text
reduce background work
reduce indexing frequency
avoid unnecessary model loads
reduce speculative work
preserve user responsiveness
```

### Orange

Meaningful pressure:

```text
pause nonessential background jobs
trim caches
reduce retrieval breadth
reduce parallel tool work
lower optional context
avoid loading a second model
```

### Red

Critical pressure:

```text
stop admitting new heavyweight tasks
evict nonessential memory
stop calibration
reduce background processes
protect active run
```

### Emergency

The system's first priority becomes survival and state preservation:

```text
persist state
settle/abort unsafe work
unload heavy resources where safe
protect the UI
recover gracefully
```

The existing `preflight.LiveMonitor` and memory manager are excellent foundations for this.

The next step is to transform them from isolated protection mechanisms into a **closed-loop resource controller**.

---

# 9. CPU Adaptation

CPU adaptation should distinguish between:

```text
interactive workload
agent workload
background workload
maintenance workload
```

A laptop at 90% CPU for 500 ms is not equivalent to sustained 90% utilization for ten minutes.

The Governor should therefore use:

```text
instantaneous samples
+
rolling averages
+
pressure duration
+
hysteresis
```

The system can adapt:

```text
generation threads
prefill threads
tool parallelism
repository indexing
memory maintenance
automation concurrency
research concurrency
calibration
background summarization
```

Some engine parameters require restart, so SHEYTAN should distinguish:

```text
LIVE ADJUSTMENT
vs
NEXT-RUN ADJUSTMENT
vs
RELOAD REQUIRED
```

This avoids constant engine restarts.

---

# 10. RAM Adaptation Should Be More Intelligent Than “Use X%”

SHEYTAN already knows model-card facts and computes memory plans.

The next level is to combine:

```text
physical RAM
+
currently available RAM
+
SHEYTAN process RSS
+
engine RSS
+
model memory plan
+
context/KV requirements
+
background workload
+
observed pressure
```

A model should not be considered safe simply because:

```text
model file size < RAM
```

Nor should mapped memory automatically be treated as fully resident.

The Governor should maintain a **resident-memory budget** and an **admission-control decision** for new workloads.

This can determine:

```text
which model to load
whether to keep a draft model resident
whether to retain caches
how large the logical context may safely become
whether background indexing may run
whether multiple tasks may coexist
```

---

# 11. Model Routing Becomes Essential

Today SHEYTAN largely chooses a model/backend configuration.

The future needs to choose among multiple possible models.

Conceptually:

```text
Task
 ↓
Capability requirements
 ↓
Resource envelope
 ↓
Model candidates
 ↓
Measured cost/quality history
 ↓
Policy
 ↓
Selected model
```

A small model could handle:

```text
classification
simple lookup
summaries
routine transformations
lightweight automation
```

A larger model could handle:

```text
architecture
difficult debugging
complex research
high-risk decisions
long reasoning
```

A vision model can handle:

```text
screenshots
PDF/image interpretation
visual UI tasks
```

A coding-specialized model can handle:

```text
large repository changes
refactoring
debugging
test repair
```

The routing system should consider:

```text
capability
+
measured quality
+
latency
+
memory
+
CPU/GPU load
+
user preferences
+
privacy
+
cost
+
task risk
```

This becomes one of the largest differences between “local model runner” and “local AI platform.”

---

# 12. The Improvement Loop

The phrase **self-improving AI** needs an engineering definition.

SHEYTAN should initially improve its *system*, not casually rewrite its model weights.

The first improvement loop should be:

```text
OBSERVE
   ↓
DIAGNOSE
   ↓
FORM HYPOTHESIS
   ↓
CREATE CANDIDATE
   ↓
RUN CONTROLLED EXPERIMENT
   ↓
EVALUATE
   ↓
COMPARE AGAINST BASELINE
   ↓
PROMOTE OR ROLLBACK
   ↓
STORE VERIFIED LESSON
```

This is strongly compatible with the existing repository.

The Coding Lab supplies execution.

Artifacts supply provenance.

Scheduler supplies recurring experiments.

Memory supplies long-term state.

Skills supply reusable procedures.

Verification supplies objective evidence.

The missing component is the **improvement/evaluation controller** connecting them.

---

# 13. What SHEYTAN Should Be Allowed to Improve

Initially:

### Behavior

```text
system instructions
response policies
reasoning procedures
task decomposition
tool-selection strategy
```

### Memory

```text
what should be remembered
what should be forgotten
retrieval strategy
memory organization
```

### Skills

```text
new skills
skill refinement
trigger refinement
failure boundaries
procedural improvements
```

### Tools

```text
new tools
tool schemas
tool selection
tool workflows
```

### Context

```text
retrieval strategy
context allocation
summarization
history selection
tool-result compression
```

### Runtime

```text
threads
batching
context sizes
model choice
backend choice
caching
background scheduling
```

### Routing

```text
which model handles which class of work
```

Only later should SHEYTAN move into heavier mechanisms such as:

```text
LoRA
adapters
fine-tuning
distillation
specialized local training
```

Those should be experimental capabilities, not prerequisites for self-improvement.

---

# 14. Every Improvement Needs an Evaluation Harness

A self-modifying AI without evaluation becomes self-reinforcing configuration drift.

SHEYTAN therefore needs a first-class:

## Evaluation Suite

An evaluation suite should contain real tasks such as:

```text
coding task
research task
reasoning task
memory task
tool-use task
file-edit task
vision task
conversation task
```

Each can have measurable criteria:

```text
correctness
tests passing
citation quality
tool efficiency
latency
RAM peak
CPU pressure
token usage
failure rate
user feedback
```

A system change should never be promoted merely because the model claims it is better.

The existing verification architecture gives SHEYTAN a natural place to build this.

---

# 15. System Versions Become Important

An AI System should be versioned like software.

Example:

```text
Personal Assistant v12
```

contains:

```text
model policy v4
memory policy v3
skills v17
tools v8
instructions v9
evaluation suite v6
runtime policy v5
```

A new candidate becomes:

```text
Personal Assistant v13-candidate
```

SHEYTAN evaluates it.

If it performs better according to the user's evaluation policy:

```text
PROMOTE
```

Otherwise:

```text
ROLLBACK
```

This turns "my AI learned something" into a reproducible engineering event.

---

# 16. User Feedback Must Become a Learning Signal

The current memory/recall feedback mechanism is a useful starting point.

The future system should separate:

```text
explicit user feedback
objective test evidence
automatic telemetry
model self-assessment
```

These are not equivalent.

For example:

```text
User liked answer
```

is useful evidence.

But:

```text
build passed
```

is stronger evidence for a coding change.

And:

```text
benchmark suite improved
```

is evidence for a system-policy change.

SHEYTAN should preserve these evidence classes separately.

---

# 17. Long-Running Agents Need Durable Identity

The project has already implemented pause/edit/resume, recovery, durable automation, checkpoints, artifacts, and persistent memory.

The next architectural step is to treat an agent task as something that can exist for:

```text
minutes
hours
days
weeks
```

without requiring one giant context window.

The system should maintain:

```text
Task identity
Mission
Current state
Known facts
Decisions
Open questions
Completed work
Pending work
Artifacts
Memory
Skills
Evaluation state
Resource state
Current system version
```

Recent research strongly supports this general direction: long-running agents require explicit mechanisms for bridging context windows, and newer research is exploring self-optimizing memory and evolving skill memory rather than relying solely on larger prompts.

SHEYTAN already has many of the required persistence primitives.

---

# 18. The Future UI Should Become an AI Laboratory

The current UI is still organized primarily around:

```text
Chat
Agent
Workspace/Lab
System
Settings
```

The future should add a first-class concept of:

## My AI Systems

A user should see:

```text
My AI Systems
│
├── SHEYTAN Assistant
├── Coding Engineer
├── Research Analyst
├── Private Business AI
└── Experimental AI
```

Opening one should expose:

```text
Chat
Knowledge
Memory
Skills
Tools
Models
Automations
Experiments
Evaluations
Artifacts
Permissions
Performance
History
Versions
```

This is much closer to what your stated product vision actually requires.

---

# 19. Computer Use Is a Major Capability Gap

Current frontier products increasingly operate computers rather than only text APIs. Google has integrated computer use into Gemini models; Anthropic exposes computer-use tooling; OpenAI's agentic systems have used browsers, terminals, APIs, and graphical interaction; Grok Bot provides persistent computers for agents.

SHEYTAN therefore eventually needs a controlled:

```text
Computer Interaction Layer
```

with:

```text
screen capture
mouse
keyboard
window discovery
application discovery
browser
clipboard
file dialogs
process interaction
```

But this must go through the existing permission architecture.

The system should never give an agent unrestricted desktop control merely because the model requested it.

---

# 20. Multimodality Should Become Model-Agnostic

SHEYTAN already has a vision foundation.

The future should make multimodality a capability layer rather than a hardcoded model feature.

The system should be able to reason:

```text
text
+
images
+
screenshots
+
PDFs
+
audio
+
video
+
structured data
+
code
```

and route each input/output modality to whatever local or remote backend actually supports it.

---

# 21. MCP Should Become an Interoperability Layer, Not the Product Architecture

MCP is clearly becoming a major ecosystem standard. Anthropic, Google, Jan, LM Studio and others are all integrating it.

SHEYTAN should support MCP strongly.

But the architecture must remain:

```text
SHEYTAN capability model
        ↓
permission/trust layer
        ↓
MCP adapter
```

rather than:

```text
MCP becomes the entire internal architecture
```

SHEYTAN's own lifecycle, security, evidence, memory, resource governor and task model must remain authoritative.

---

# 22. The Competitive Architecture

The long-term architecture should look approximately like this:

```text
                         SHEYTAN-LA
                              │
             ┌────────────────┼────────────────┐
             │                │                │
          AI SYSTEM        USER/WORK        SYSTEM
             │                │                │
     ┌───────┼────────┐       │         ┌──────┼───────┐
     │       │        │       │         │      │       │
   Models  Memory   Skills   Projects  CPU    RAM    GPU/NPU
     │       │        │       │         │      │       │
     └───────┼────────┴───────┘         └──────┼───────┘
             │                                  │
        Agent Runtime ←──────── Resource Governor
             │
     ┌───────┼──────────────────────────────┐
     │       │        │        │             │
   Tools   Research  Browser  Coding Lab  Computer
     │       │        │        │             │
     └───────┼────────┴────────┴─────────────┘
             │
       Context / Memory Engine
             │
       Evaluation / Evidence
             │
       Improvement Engine
             │
       Version / Promotion / Rollback
             │
       Local + Optional Remote Models
```

This is the architecture I would now use as the strategic north star.

---

# 23. What Should NOT Be Done

Several tempting directions would weaken the product.

### Do not become another wrapper

SHEYTAN should not become:

```text
UI → Ollama
UI → LM Studio
UI → arbitrary API
```

with a few cosmetic features.

Existing engine ownership should remain a core strength.

### Do not make model size the architecture

A bigger local model does not automatically make the system better.

SHEYTAN's advantage should come from:

```text
model
+
context
+
memory
+
tools
+
skills
+
routing
+
verification
+
runtime optimization
```

### Do not confuse self-improvement with arbitrary self-modification

A self-improving system needs:

```text
candidate
baseline
experiment
measurement
promotion
rollback
```

### Do not maximize CPU/RAM usage blindly

“Peak hardware utilization” is not the objective.

A laptop that becomes unusable is a failed optimization.

The objective is:

> **maximum useful AI capability while maintaining a healthy, responsive system.**

### Do not create duplicate authorities

The current architecture's one-registry/one-session/one-scheduler/one-lifecycle pattern should remain sacred.

---

# 24. Recommended New Roadmap

The existing ROADMAP.md should be rewritten because it is now centered on an older v1.7.2 planning state while the repository has reached v1.7.5.

The new roadmap should be capability-driven.

## v1.8 — Adaptive Runtime Intelligence

Primary objective:

> SHEYTAN understands its machine continuously and adapts its execution strategy.

Deliver:

```text
Runtime Governor
resource-state model
CPU/RAM pressure model
resource envelopes
dynamic admission control
adaptive background work
adaptive context budgets
adaptive tool concurrency
model memory admission
runtime self-inspection
system-health dashboard
```

Exit condition:

> SHEYTAN can operate for long periods without unnecessarily degrading the host and can explain why it changed its runtime strategy.

---

## v1.9 — AI System Builder

Primary objective:

> Users can create their own complete AI systems.

Deliver:

```text
AI System object
system profiles
instructions
model policy
memory policy
knowledge sources
skills
tools
permissions
automations
runtime policy
versioning
clone/export/import
system-level UI
```

Exit condition:

> A user can create a named AI system, configure its personality/capabilities/resources/tools/knowledge, and use it independently.

---

## v1.10 — Universal Agent

Primary objective:

> SHEYTAN handles general computer-based work, not only engineering.

Deliver:

```text
computer-use layer
browser automation
desktop interaction
advanced document workflows
multimodal task execution
voice/input/output foundation
richer artifact generation
application connectors
```

Exit condition:

> An AI System can complete meaningful multi-application real-world workflows under explicit permissions.

---

## v1.11 — AI Learning & Evaluation

Primary objective:

> Users can systematically improve their AI systems.

Deliver:

```text
evaluation suites
baselines
experiments
A/B system variants
automatic diagnostics
feedback learning
skill evolution
memory optimization
routing optimization
context optimization
promotion/rollback
improvement history
```

Exit condition:

> SHEYTAN can demonstrate that a proposed system change actually improved defined evaluation outcomes.

---

## v1.12 — Advanced Model Intelligence

Primary objective:

> SHEYTAN dynamically combines different models and engines.

Deliver:

```text
multi-model routing
capability discovery
task-specialist models
vision routing
reasoning routing
draft/speculative models
dynamic loading/unloading
model pools
cross-model fallback
resource-aware model selection
```

Current llama.cpp already provides increasingly sophisticated options such as adaptive fitting, multiple GPU-layer strategies, continuous batching and several speculative-decoding mechanisms, making this a practical future runtime direction rather than a purely theoretical feature.

---

# v2.0 — SHEYTAN Local AI Platform

The v2.0 definition should change from:

> “complete local engineering environment”

to:

> **“complete user-owned local AI platform.”**

The v2.0 acceptance test should be something like:

> “Create an AI system for me. Understand my goals, inspect my machine, choose an appropriate model and runtime, connect the required knowledge and tools, remember what matters, perform the task, evaluate the result, improve the system when evidence supports the change, and keep the resulting AI system versioned and reproducible.”

That is a much more ambitious and much more differentiated target.

---

# 25. The Long-Term Product Model

The central architecture becomes:

```text
                    USER
                      │
                      ▼
                MY AI SYSTEM
                      │
        ┌─────────────┼─────────────┐
        ▼             ▼             ▼
     KNOWLEDGE      MEMORY        SKILLS
        │             │             │
        └─────────────┼─────────────┘
                      ▼
                 AGENT CORE
                      │
          ┌───────────┼───────────┐
          ▼           ▼           ▼
        TOOLS      RESEARCH    COMPUTER
          │           │           │
          └───────────┼───────────┘
                      ▼
                 MODEL ROUTER
                      │
        ┌─────────────┼─────────────┐
        ▼             ▼             ▼
      LOCAL          NATIVE       REMOTE
      MODELS         ENGINE       MODELS
        │             │             │
        └─────────────┼─────────────┘
                      ▼
               RUNTIME GOVERNOR
                      │
             CPU / RAM / GPU / NPU
                      │
                      ▼
               SYSTEM FEEDBACK
                      │
                      ▼
             EVALUATION ENGINE
                      │
                      ▼
             IMPROVEMENT ENGINE
                      │
             ┌────────┴────────┐
             ▼                 ▼
          PROMOTE            ROLLBACK
```

---

# 26. Final R&D Conclusion

SHEYTAN-LA should not attempt to win by building another chatbot.

The strongest path is to build the infrastructure for **personal AI ownership**.

The critical conceptual transition is:

```text
CURRENT

User
 ↓
SHEYTAN
 ↓
Model
```

becoming:

```text
FUTURE

User
 ↓
AI System
 ↓
SHEYTAN Runtime
 ├── Models
 ├── Memory
 ├── Knowledge
 ├── Skills
 ├── Tools
 ├── Research
 ├── Computer
 ├── Automation
 ├── Evaluation
 ├── Improvement
 └── Runtime Governor
```

That distinction matters enormously.

The model should become replaceable.

The AI System should become durable.

The user's knowledge, skills, memory, tools, experiments, evaluation history, and preferences should survive model changes.

The runtime should continuously adapt to the machine.

The system should know what it actually has available.

It should know what is currently constrained.

It should choose what to load, what to unload, what to run, what to postpone, and which model should handle each task.

And when the user wants a better AI, SHEYTAN should provide an engineering loop for creating one:

```text
observe
→ learn
→ experiment
→ evaluate
→ improve
→ version
→ preserve
```

This is where the current v1.7.5 architecture becomes strategically valuable: the repository already contains many of the difficult foundational pieces—durable execution, memory, skills, tools, automation, repository intelligence, Coding Lab, artifacts, verification, multiple inference backends, recovery, and resource protection.

The next generation of SHEYTAN-LA should therefore focus less on accumulating isolated features and more on **connecting those existing authorities into one coherent AI-system lifecycle**.

## Core product statement

> **SHEYTAN-LA is a local-first platform for creating, running, understanding, and continuously improving user-owned AI systems.**

## Core engineering principle

> **The model provides intelligence. SHEYTAN provides the system that makes that intelligence useful, persistent, adaptive, verifiable, and user-owned.**

## Core runtime principle

> **SHEYTAN should maximize useful AI capability within the real constraints of the user's machine—not merely maximize resource utilization.**

## Core learning principle

> **No system change becomes an improvement until evidence demonstrates that it improved the user's defined objective.**

## Core competitive strategy

> **Do not try to clone ChatGPT, Claude, Gemini, or Grok internally. Build the local platform in which users can construct AI systems with the same broad class of capabilities, while retaining ownership of their models, memory, tools, knowledge, behavior, experiments, and runtime.**

This is the direction I recommend treating as the new R&D north star for SHEYTAN-LA.
