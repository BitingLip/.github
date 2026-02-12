<div align="center">

# 🫦 Biting Lip

**Intelligent Automations Platform & Studio**

![Biting Lip Logo](214111120.png)

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](../LICENSE)
[![.NET 9](https://img.shields.io/badge/.NET-9.0-purple.svg)](https://dotnet.microsoft.com)
[![React 18](https://img.shields.io/badge/React-18-blue.svg)](https://react.dev)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.4-blue.svg)](https://typescriptlang.org)
[![Python 3.11+](https://img.shields.io/badge/python-3.11%2B-blue.svg)](https://python.org)
[![FastAPI](https://img.shields.io/badge/FastAPI-latest-green.svg)](https://fastapi.tiangolo.com)

<h3>AI-powered content production, from text to audio.</h3>

</div>

---

## What Is 🫦 Biting Lip?

Biting Lip is a modular platform for building **intelligent automation workflows** — pipelines that chain LLM analysis, speech synthesis, and audio processing into end-to-end production systems.

The first production workflow is **Audiobook Studio**: import a book, and the platform annotates every sentence with narrative metadata, assigns voices, generates speech, and delivers a fully produced audiobook.

### Architecture

```
┌─────────────────────────────────────────────────────┐
│  Studio          React + TypeScript + Zustand        │
│  ───────         Editor, Timeline, Voice Selector    │
├─────────────────────────────────────────────────────┤
│  Core            .NET 9 / C#                         │
│  ───────         Workflow Engine, Actions, DTOs       │
│                  42 shared enums · Swagger/OpenAPI    │
├─────────────────────────────────────────────────────┤
│  Services        Python / FastAPI                    │
│  ───────         TTS (NeuTTS) · ASR (Whisper)        │
│                  LLM (OpenAI) · Phonemizer           │
├─────────────────────────────────────────────────────┤
│  Platform        bitinglip.com                       │
│  ───────         Landing page & content hub          │
└─────────────────────────────────────────────────────┘
```

### Key Capabilities

- **Workflow Engine** – Declarative YAML workflows with step groups, dependency graphs, and parallel execution.
- **Studio Editor** – Interactive document view with sentence-level audio, waveform timeline, and real-time playback.
- **LLM Annotation** – Scene detection, character enrichment, dialogue tagging, shot direction — all via structured prompts.
- **Voice Assignment** – Character profiling (age, sex, voice type) with automatic voice library matching.
- **TTS Pipeline** – Multi-voice speech synthesis with ASR verification and word-level timing alignment.
- **Single Source of Truth** – 42 shared enums flow from C# → JSON (UPPER_SNAKE_CASE) → TypeScript, enforced by CI integration tests.

