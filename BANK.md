# The Bank

Entries are grouped by theme. Each entry: date, canonical source, summary in our words, a brief verified key line where available, tags, and a product lens. See the [banking policy](README.md#banking-policy) for how entries are verified and marked.

---

## LLM capability & agents

### 2026-10-11 — The capability-understanding funnel is widening
Source: https://x.com/karpathy/status/2109361546505966046
Summary: Karpathy revives his April post: the gap in shared understanding of LLM capability is widening into a funnel — ~75% of people have barely touched LLMs and read AI as hype; many still think LLMs are the frontier when it is agentic systems now; the tip that deeply understands agents looks "crazy" even to the layer below. Frontier capability is "peaky" (strongest where RL rewards are verifiable: code, math, research), so both camps are right about what they have seen.
Key line: "The people at the very tip are starting to look totally crazy to even the very next layer down in the funnel."
Tags: capability-gap, agents, adoption, general
Product lens: Most users meet your product from a lower layer of the funnel than you do. Build onboarding and explanations that meet them at their layer — and make capability legible with receipts, not claims. (mymilo: show the work, not just the answer.)

### 2025-11-17 — Verifiability is the new predictive feature
Source: https://x.com/karpathy/status/1990116666194456651
Summary: Software 1.0 automated what could be specified; Software 2.0 automates what can be verified. Whether a task gets automated now hinges on verifiability — the environment must be resettable, efficient, and rewardable so an AI can practice in it. This also explains "jagged" capability: domains with good verifiers (math, code) leap ahead; domains without them lag.
Key line: "If a task/job is verifiable, then it is optimizable directly or via reinforcement learning."
Tags: verification, rl, automation, codetopo, general
Product lens: The moat is the verifier, not the model. Pick product surfaces where outcomes are checkable, and ship the checker with the feature. (codetopo: proof and verification artifacts are the product, not a by-product.)

### 2025-12-26 — "I've never felt this much behind"
Source: https://x.com/karpathy/status/2004607146781278521
Summary: A year-end confessional that became the agentic-engineering manifesto: the profession is being refactored, the programmer's own bits are increasingly sparse, and there is a whole new programmable layer to master — agents, subagents, prompts, contexts, memory, modes, permissions, tools, plugins, skills, hooks, MCP, workflows — on top of the old stack, with stochastic, fallible entities now intermingled with classical engineering.
Key line: "I've never felt this much behind as a programmer."
Tags: agents, agentic-engineering, mcp, skills, mymilo, general
Product lens: That new layer *is* the product surface now. An agent product should expose and manage these primitives natively — memory, permissions, tools, hooks — instead of hiding them behind a chat box. (mymilo: the layer is the UI.)

### 2026-01-26 — The 80/20 flip: from manual coding to agent coding
Source: https://x.com/karpathy/status/2015883857489522876
Summary: Notes from a few weeks of heavy agent coding: his workflow flipped in about a month, from roughly 80% manual-plus-autocomplete coding and 20% agents in November to roughly 80% agent coding and 20% edits and touch-ups by December — a phase change in capability, not a gradual drift. (via aggregator — secondary source; wording unverified — summary from secondary sources)
Tags: agents, workflow, agentic-engineering, general
Product lens: When the user's work flips from doing to directing, the product's job flips too: delegation, review queues, and diff-level oversight become the core experience. (mymilo, codetopo: build for the director, not the typist.)

### 2026-03-07 — autoresearch: agents that run the experiments overnight
Source: https://x.com/karpathy/status/2029701092347630069
Summary: Release of autoresearch: give an agent a small, real LLM training setup and a program.md brief; it modifies code, trains for a few minutes, checks whether the result improved, keeps or discards the change, and repeats — overnight. You stop programming the Python files and start programming the research organization itself. A follow-up post two days later reported hundreds of experiments transferring to larger models. (via aggregator — secondary source)
Tags: agents, autoresearch, autonomous-loops, general
Product lens: The keep/discard loop is the pattern: autonomous iteration is safe where each step is cheap, time-boxed, and judged by a metric. Products can run bounded self-improvement loops — but only behind a verifier that decides keep vs. discard.

### 2026-04-09 — Hand a model a terminal and watch it melt problems
Source: https://x.com/karpathy/status/2042334451611693415
Summary: A short field note on the current frontier: give one of these models a computer terminal and it will visibly dissolve programming problems that would normally take days or weeks of human work. The bottleneck has moved from "can it code" to access, supervision, and judgment. (via aggregator — secondary source)
Key line: "you can now watch them melt programming problems that you'd normally expect to take days/weeks of work"
Tags: agents, terminal, capability, conduit, mymilo
Product lens: Terminal/tool access is the capability multiplier — and the risk multiplier. Offer it with sandboxes, permission gates, and audit trails as first-class features, not afterthoughts. (conduit: governed tool access is the sellable surface.)

### 2026-06-09 — The temptation to stop looking at the code
Source: https://x.com/karpathy/status/2064409694761054332
Summary: On a frontier model release: it has never felt this tempting to stop reading the code entirely — with the immediate self-correction that you must not do this in production. The better the generator gets, the stronger the pull to skip review, and the more deliberate the review discipline has to be. (via aggregator — secondary source)
Key line: "it's never felt this tempting to stop looking at the code at all (but don't do this in prod!)"
Tags: verification, review, craft, codetopo
Product lens: Review tooling must scale with trust: as generation gets better, make verification cheaper and more visual, or users will skip it exactly when the stakes rise. (codetopo: comprehension tooling is the counterweight to generation.)

### 2025-06-25 — Context engineering over prompt engineering
Source: https://x.com/karpathy/status/1937902205765607626
Summary: An endorsement that named a discipline: in every industrial-strength LLM app, the real work is filling the context window with just the right information for the next step — task descriptions, examples, retrieved data, tools, state, history, compaction. Too little or the wrong form and the model underperforms; too much or too irrelevant and cost rises while performance falls.
Key line: "context engineering is the delicate art and science of filling the context window with just the right information for the next step"
Tags: context-engineering, agents, memory, mymilo, codetopo
Product lens: Context is a budget, not a bucket. Treat retrieval, compaction, and relevance-ranking as core product engineering. (mymilo: memory quality = answer quality; codetopo: topology is how you choose what enters the window.)

---

## Software & AI industry

### 2023-01-24 — The hottest new programming language is English
Source: https://x.com/karpathy/status/1617979122625712128
Summary: A one-line thesis that became his pinned post: natural language is now a programming interface — you specify intent in English and the model compiles it into working software. It reframed prompting from a chat trick into a development paradigm, years before "vibe coding" named the practice.
Key line: "The hottest new programming language is English"
Tags: software-3.0, natural-language, industry, general
Product lens: If English is the interface, then the quality of a user's intent-expression is your product's input quality. Invest in intent capture — structured briefs, clarifying questions, examples — the way compilers invest in parsers. (mymilo: the brief is the program.)

### 2023-09-28 — LLMs as the kernel of a new operating system
Source: https://x.com/karpathy/status/1707437820045062561
Summary: The origin of the "LLM OS" frame: LLMs are emerging not as chatbots but as the kernel process of a new operating system, already orchestrating multimodal I/O, a code interpreter, browsing, and an embeddings database for memory and retrieval — with computer-security concepts (attacks, defenses, vulnerabilities) carrying over wholesale.
Key line: "a more complete picture is emerging of LLMs not as a chatbot, but the kernel process of a new Operating System"
Tags: llm-os, architecture, agents, mymilo
Product lens: Design agent products like an OS, not an app: processes (agents), a scheduler, permissions, a filesystem (retrieval), and peripherals (tools). The winners build the platform layer, not another chatbot skin. (mymilo: be the OS of the user's work.)

### 2023-11-10 — LLM OS, spec sheet edition
Source: https://x.com/karpathy/status/1723140519554105733
Summary: The analogy made concrete as a spec sheet: the LLM as a multi-core processor running at tokens-per-second speed, the context window as RAM (128K tokens at the time), and an embeddings model as the filesystem. A playful post that quietly fixed the vocabulary the industry still uses for agent architecture.
Key line: "LLM OS. Bear with me I'm still cooking."
Tags: llm-os, context-window, architecture, codetopo, general
Product lens: RAM is scarce and precious: page information in and out deliberately. Every architecture review should ask "what's in RAM right now, and why?" (codetopo: maps of the codebase are how a small RAM covers a large disk.)

### 2025-02-02 — Vibe coding
Source: https://x.com/karpathy/status/1886192184808149383
Summary: The coinage that named an era: a new kind of coding where you talk to the model (in his case, by voice), accept all changes, paste errors back, and barely touch the keyboard — explicitly scoped by him as fine for throwaway weekend projects. The term went so mainstream it became a dictionary Word of the Year, and he later drew the line himself: vibe coding raises the floor; agentic engineering raises the ceiling.
Key line: "you fully give in to the vibes, embrace exponentials, and forget that the code even exists"
Tags: vibe-coding, craft, agents, general
Product lens: Support both modes honestly: a fast, loose mode for exploration and a rigorous mode for production — and make the boundary visible in the product, because users will not police it themselves. (codetopo, conduit: flag unreviewed output; never let the throwaway path silently become the production path.)

### 2026-05-19 — Joined Anthropic
Source: https://x.com/karpathy/status/2056753169888334312
Summary: A personal update: he joined Anthropic to get back to R&D, expecting the next few years at the frontier of LLMs to be especially formative — while remaining passionate about education and planning to resume that work in time. A datapoint on where top independent talent judged the frontier action to be. (via aggregator — secondary source)
Key line: "Personal update: I've joined Anthropic."
Tags: industry, talent, frontier-labs, general
Product lens: Frontier gravity is real: independent builders compete on application, taste, and domain depth, not on base models. Position products where labs won't go — specific users, specific workflows, verified outcomes.

---

## Learning & craft

### 2024-07-11 — GPT-2, reproduced in llm.c for $672
Source: https://x.com/karpathy/status/1811467135279104217
Summary: The llm.c project — GPT training implemented directly in C/CUDA with minimal dependencies — reproduced the full GPT-2 (1.5B) run on a single 8×H100 node in 24 hours for about $672, five years after the original cost orders of magnitude more. A demonstration of his recurring ethos: strip a system to its essentials, in the open, until anyone can run it. (via aggregator — secondary source)
Tags: llm.c, from-scratch, reproducibility, craft, general
Product lens: Minimal, inspectable implementations compound trust and teachability. Where a dependency-heavy stack hides behavior, a small readable core becomes the reference everyone forks. (codetopo: dependency-light and readable-by-design is a feature users can feel.)

### 2024-07-16 — Eureka Labs: an AI-native school
Source: https://x.com/karpathy/status/1813263734707790301
Summary: Launch of Eureka Labs, "a new kind of school that is AI native": the teacher still designs the course materials, but an AI teaching assistant — patient, fluent, always available — guides each student through them. First course: LLM101n, where students build their own LLM. The pattern inverts the usual ed-tech pitch: experts design the artifact; AI personalizes the delivery.
Key line: "Excited to share that I am starting an AI+Education company called Eureka Labs."
Tags: education, ai-native, eureka-labs, general
Product lens: The AI-native pattern: human expertise authors the substance once; the model delivers, paces, and adapts it per user. Any product with expert content inside should split those two jobs the same way.

### 2025-10-13 — nanochat: the $100 ChatGPT
Source: https://x.com/karpathy/status/1977755427569111362
Summary: Release of nanochat: unlike nanoGPT (pretraining only), a minimal, from-scratch, full-stack training-and-inference pipeline for a ChatGPT clone in roughly 8,000 lines — tokenizer, pretraining, midtraining, SFT, optional RL, inference engine, and a web UI — that trains a talkable model in about 4 hours for about $100 on a rented GPU box, and emits a single markdown "report card" for the run.
Key line: "Excited to release new repo: nanochat!"
Tags: nanochat, from-scratch, minimalism, education, general
Product lens: A complete, small, forkable reference implementation beats a sprawling framework for learning and for trust. Ship the strong baseline in one cohesive piece — and grade the run with a report card, not a log dump.
