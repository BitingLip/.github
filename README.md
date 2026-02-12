# 🫦 Biting Lip

**Intelligent Automations Platform & Studio**

AI-powered content production workflows — from raw text to fully produced audiobooks.

## Repositories

| Repo | Stack | Description |
|------|-------|-------------|
| **core** | .NET 9 / C# | Workflow engine, actions, typed DTOs, shared enums, Swagger API |
| **studio** | React 18 / TypeScript | Production editor — document view, timeline, voice selector, playback |
| **services** | Python / FastAPI | AI microservices — TTS (NeuTTS), ASR (Whisper), LLM (OpenAI), phonemizer |
| **platform** | React + FastAPI | Public site at bitinglip.com — landing page, content hub, subscriptions |

## Quick Start

```powershell
# Start everything
./core/start.ps1       # .NET Worker API on :8081
./studio/start.ps1     # Studio frontend on :5173 + backend on :8080
./services/start.ps1   # AI services (TTS, ASR, LLM)
./platform/start.ps1   # Platform site on :3000
```

## License

[MIT](LICENSE)