---
layout: distill
title: Grounding Machine Creativity in Game Design Knowledge Representations - Empirical Probing of LLM-Based Executable Synthesis of Goal Playable Patterns under Structural Constraints

description:
img: 
category:  Games
related_publications: true
featured: true

authors:
  - name: Hugh Xuechen Liu
    url: 
    affiliations:
      name: Chalmers University of Technology
  - name: Kıvanç Tatar
    url: "https://www.kivanctatar.com"
    affiliations:
      name: Chalmers University of Technology


---
## Abstract

Creatively translating complex gameplay ideas into executable artifacts (e.g., games as Unity projects and code) remains a central challenge in computational game creativity. Gameplay design patterns provide a structured representation for describing gameplay phenomena, enabling designers to decompose high-level ideas into entities, constraints, and rule-driven dynamics. Among them, goal patterns formalize common player-objective relationships. Goal Playable Concepts (GPCs) operationalize these abstractions as playable Unity engine implementations, supporting experiential exploration and compositional gameplay design. We frame scalable playable pattern realization as a problem of constrained executable creative synthesis: generated artifacts must satisfy Unity's syntactic and architectural requirements while preserving the semantic gameplay meanings encoded in goal patterns. This dual constraint limits scalability. Therefore, we investigate whether contemporary large language models (LLMs) can perform such synthesis under engine-level structural constraints and generate Unity code (as games) structured and conditioned by goal playable patterns. Using 26 goal pattern instantiations, we compare a direct generation baseline (natural language -> C# -> Unity) with pipelines conditioned on a human-authored Unity-specific intermediate representation (IR), across three IR configurations and two open-source models (DeepSeek-Coder-V2-Lite-Instruct and Qwen2.5-Coder-7B-Instruct). Compilation success is evaluated via automated Unity replay. We propose grounding and hygiene failure modes, identifying structural and project-level grounding as primary bottlenecks.

<https://arxiv.org/abs/2509.22017>
