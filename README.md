<div align="center">

<!-- LOGO -->
<img src="https://raw.githubusercontent.com/eli64s/readme-ai/e2a5f0ab93b923a78935178dd165d5019b4a1fbc/docs/docs/assets/svg/logo.svg" width="200px" alt="ReadmeAI Logo"/>

# ✦ ReadmeAI

### *The last README you'll ever write by hand.*

**AI-powered README generation for every language, framework, and developer.**

[![CI Pipeline](https://img.shields.io/github/actions/workflow/status/eli64s/readme-ai/release-pipeline.yml?logo=githubactions&label=CI&logoColor=white&color=4169E1)](https://github.com/eli64s/readme-ai/actions)
[![Coverage](https://img.shields.io/codecov/c/github/eli64s/readme-ai?logo=codecov&logoColor=white&label=Coverage&color=5D4ED3)](https://app.codecov.io/gh/eli64s/readme-ai)
[![PyPI](https://img.shields.io/pypi/v/readmeai?logo=Python&logoColor=white&label=PyPI&color=7934C5)](https://pypi.python.org/pypi/readmeai/)
[![Downloads](https://img.shields.io/pepy/dt/readmeai?logo=PyPI&logoColor=white&label=Downloads&color=9400D3)](https://www.pepy.tech/projects/readmeai)
[![License: MIT](https://img.shields.io/github/license/eli64s/readme-ai?logo=opensourceinitiative&logoColor=white&label=License&color=8A2BE2)](https://opensource.org/license/mit/)

<br/>

[**🚀 Quickstart**](#-getting-started) · [**✨ Features**](#-features) · [**⚙️ Configuration**](#️-configuration) · [**🖼 Gallery**](#-example-gallery) · [**🤝 Contributing**](#-contributing)

<img src="https://raw.githubusercontent.com/eli64s/readme-ai/eb2a0b4778c633911303f3c00f87874f398b5180/docs/docs/assets/svg/line-gradient.svg" width="100%"/>

</div>

## 🧠 What is ReadmeAI?

**ReadmeAI** is a developer tool that scans your codebase — local or remote — and generates a beautifully structured, comprehensive `README.md` in seconds using state-of-the-art AI language models.

No more blank-page paralysis. No more copy-pasting boilerplate. Just point ReadmeAI at your repo and ship.

> 🎯 **Designed for simplicity, customization, and developer productivity.**

```bash
# It's this simple. Point. Generate. Ship.
❯ readmeai --api openai --repository https://github.com/your/project
```

<img src="https://raw.githubusercontent.com/eli64s/readme-ai/eb2a0b4778c633911303f3c00f87874f398b5180/docs/docs/assets/svg/line-gradient.svg" width="100%"/>

## ✨ Features

### 🎨 Stunning Customization

Make your README yours — choose from multiple header styles, badge themes, emoji packs, logo options, and navigation layouts.

| Style | Preview | Command |
|-------|---------|---------|
| **Classic** | ![Classic](https://github.com/eli64s/readme-ai/raw/main/docs/docs/assets/img/documentation/headers/variations/custom-dragon.png?raw=true) | `--header-style classic --badge-style flat-square` |
| **Modern** | ![Modern](https://github.com/eli64s/readme-ai/raw/main/docs/docs/assets/img/documentation/headers/variations/modern-for-the-badge.png?raw=true) | `--header-style modern --navigation-style roman` |
| **Compact** | ![Compact](https://github.com/eli64s/readme-ai/raw/main/docs/docs/examples/styling/headers/compact.png?raw=true) | `--header-style compact --navigation-style number` |
| **Console** | ![Console](https://github.com/eli64s/readme-ai/raw/main/docs/docs/examples/styling/headers/console.png?raw=true) | `--header-style console --emojis water` |
| **SVG Banner** | ![Banner](https://github.com/eli64s/readme-ai/raw/main/docs/docs/examples/styling/headers/svg-banner.png?raw=true) | `--header-style banner` |

### 🤖 Model Agnostic — Your AI, Your Choice

Switch between leading LLM providers with a single flag:

| Provider | Flag | Best For |
|----------|------|----------|
| **OpenAI** | `--api openai` | General-purpose, industry-leading quality |
| **Anthropic Claude** | `--api anthropic` | Advanced reasoning & nuanced docs |
| **Google Gemini** | `--api gemini` | Multimodal, cutting-edge AI |
| **Ollama** | `--api ollama` | 100% local, free, no API key needed |
| **Offline Mode** | `--api offline` | No internet, no AI — just structure |

### 📦 What Gets Generated

Every README includes fully AI-crafted sections:

- **Project Introduction** — Value proposition, purpose, and audience
- **Feature Table** — Structured breakdown of capabilities
- **Architecture Overview** — Visual directory tree with module summaries
- **Getting Started** — Auto-detected dependencies, install steps, usage commands
- **Testing Guide** — Ready-to-run test instructions
- **Roadmap & Contributing** — Community-ready contribution scaffolding

### 🌐 Works With Any Codebase

| ✅ Platform | ✅ Language | ✅ Framework |
|------------|------------|------------|
| GitHub, GitLab, Bitbucket | Python, Go, Java, Kotlin, JS, TS, Rust… | FastAPI, Docker, React, Streamlit, Spring… |

### 🔇 Smart Filtering

Control exactly what gets analyzed with `.readmeaiignore` patterns — keep your AI focused on what matters.

<img src="https://raw.githubusercontent.com/eli64s/readme-ai/eb2a0b4778c633911303f3c00f87874f398b5180/docs/docs/assets/svg/line-gradient.svg" width="100%"/>

## 🚀 Getting Started

### Prerequisites

| Requirement | Details |
|-------------|---------|
| Python ≥ 3.9 | [python.org](https://www.python.org/) |
| One LLM API key | OpenAI / Anthropic / Google Gemini — **or** use Ollama/offline for free |

### Installation

Choose your preferred method:

```bash
# pip — recommended
❯ pip install -U readmeai

# pipx — isolated environment
❯ pipx install readmeai

# uv — fastest install
❯ uv tool install readmeai

# Docker — zero-dependency containerized
❯ docker pull zeroxeli/readme-ai:latest
```

> 💡 **Anthropic or Gemini users:** install the extra dependencies:
> ```bash
> pip install "readmeai[anthropic]"
> pip install "readmeai[google-generativeai]"
> pip install "readmeai[anthropic,google-generativeai]"  # both
> ```

### Usage

**Step 1 — Set your API key:**

```bash
# OpenAI
❯ export OPENAI_API_KEY=<your_key>

# Anthropic
❯ export ANTHROPIC_API_KEY=<your_key>

# Google Gemini
❯ export GOOGLE_API_KEY=<your_key>

# Ollama (no key needed — just start the server)
❯ export OLLAMA_HOST=127.0.0.1 && ollama serve
```

**Step 2 — Generate your README:**

```bash
# Minimal — OpenAI
❯ readmeai --api openai -r https://github.com/your/repo

# With Anthropic Claude
❯ readmeai --api anthropic -m claude-3-5-sonnet-20240620 -r https://github.com/your/repo

# With Gemini
❯ readmeai --api gemini -m gemini-1.5-flash -r https://github.com/your/repo

# Local repo
❯ readmeai --api openai -r /path/to/local/project

# Fully offline — no AI, no internet
❯ readmeai --api offline -r https://github.com/your/repo

# Docker
❯ docker run -it --rm \
    -e OPENAI_API_KEY=$OPENAI_API_KEY \
    -v "$(pwd)":/app zeroxeli/readme-ai:latest \
    --repository https://github.com/your/repo --api openai
```

**Power user — full customization:**

```bash
❯ readmeai \
    --repository https://github.com/your/repo \
    --api openai \
    --model gpt-4 \
    --output readme.md \
    --badge-color A931EC \
    --badge-style flat-square \
    --header-style compact \
    --navigation-style fold \
    --logo LLM \
    --emojis solar \
    --temperature 0.9 \
    --tree-depth 2
```

### 🌐 No-Install Option: Try in Your Browser

[![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://readme-ai.streamlit.app/)

> ⚠️ The Streamlit app may lag behind the CLI on latest features.

<img src="https://raw.githubusercontent.com/eli64s/readme-ai/eb2a0b4778c633911303f3c00f87874f398b5180/docs/docs/assets/svg/line-gradient.svg" width="100%"/>

## ⚙️ Configuration

Full list of CLI options:

| Option | Description | Default |
|--------|-------------|---------|
| `--api` | LLM provider (`openai`, `anthropic`, `gemini`, `ollama`, `offline`) | `offline` |
| `--model` / `-m` | LLM model name | `gpt-3.5-turbo` |
| `--repository` / `-r` | Repo URL or local path | *required* |
| `--output` / `-o` | Output filename | `readme-ai.md` |
| `--header-style` | Header layout (`classic`, `modern`, `compact`, `console`, `banner`) | `classic` |
| `--badge-style` | Badge style (`flat`, `flat-square`, `for-the-badge`, `plastic`) | `flat` |
| `--badge-color` | Badge color — name or hex | `0080ff` |
| `--navigation-style` | TOC style (`bullet`, `number`, `roman`, `accordion`, `fold`) | `bullet` |
| `--logo` | Logo preset or `custom` | `blue` |
| `--emojis` | Emoji theme pack | `None` |
| `--temperature` | LLM creativity (0.0 – 2.0) | `0.1` |
| `--tree-max-depth` | Directory tree depth | `2` |
| `--align` | Header text alignment | `center` |

```bash
❯ readmeai --help  # full reference
```

📚 **[Full Documentation →](https://eli64s.github.io/readme-ai)**

<img src="https://raw.githubusercontent.com/eli64s/readme-ai/eb2a0b4778c633911303f3c00f87874f398b5180/docs/docs/assets/svg/line-gradient.svg" width="100%"/>

## 🖼 Example Gallery

Real-world READMEs generated by ReadmeAI across diverse tech stacks:

| Language / Stack | Repository | Generated README |
|-----------------|------------|-----------------|
| Python | [readme-ai](https://github.com/eli64s/readme-ai) | [View →](https://github.com/eli64s/readme-ai/blob/main/examples/readme-ai.md) |
| Apache Flink | [pyflink-poc](https://github.com/eli64s/pyflink-poc) | [View →](https://github.com/eli64s/readme-ai/blob/main/examples/headers/modern.md) |
| Streamlit | [readme-ai-streamlit](https://github.com/eli64s/readme-ai-streamlit) | [View →](https://github.com/eli64s/readme-ai/blob/main/examples/banners/svg-banner.md) |
| Go + Docker | [docker-gs-ping](https://github.com/olliefr/docker-gs-ping) | [View →](https://github.com/eli64s/readme-ai/blob/main/examples/readme-docker-go.md) |
| FastAPI + Redis | [async-ml-inference](https://github.com/FerrariDG/async-ml-inference) | [View →](https://github.com/eli64s/readme-ai/blob/main/examples/readme-fastapi-redis.md) |
| Java | [minimal-todo](https://github.com/avjinder/Minimal-Todo) | [View →](https://github.com/eli64s/readme-ai/blob/main/examples/headers/compact.md) |
| Kotlin (Android) | [file.io-Android-Client](https://github.com/rumaan/file.io-Android-Client) | [View →](https://github.com/eli64s/readme-ai/blob/main/examples/readme-kotlin.md) |
| PostgreSQL + DuckDB | [buenavista](https://github.com/jwills/buenavista) | [View →](https://github.com/eli64s/readme-ai/blob/main/examples/headers/classic.md) |
| Offline Mode | [litellm](https://github.com/BerriAI/litellm) | [View →](https://github.com/eli64s/readme-ai/blob/main/examples/offline-mode/readme-litellm.md) |

> 💬 **Share yours!** Post your generated README in [Show & Tell →](https://github.com/eli64s/readme-ai/discussions/categories/show-and-tell)

<img src="https://raw.githubusercontent.com/eli64s/readme-ai/eb2a0b4778c633911303f3c00f87874f398b5180/docs/docs/assets/svg/line-gradient.svg" width="100%"/>

## 🔬 Testing

```bash
# Install dev dependencies
❯ uv pip install --dev --group test --all-extras

# Run unit tests
❯ make test

# Test across Python 3.9, 3.10, 3.11, 3.12 via nox
❯ make test-nox
```

<img src="https://raw.githubusercontent.com/eli64s/readme-ai/eb2a0b4778c633911303f3c00f87874f398b5180/docs/docs/assets/svg/line-gradient.svg" width="100%"/>

## 🗺 Roadmap

- [ ] `readmeai 1.0.0` — stable, production-ready release
- [ ] Extended templates for more project types and languages
- [ ] VS Code Extension — generate READMEs right inside your editor
- [ ] GitHub Actions integration — auto-update docs on every push
- [ ] Badge packs — coverage, version, CI status, and more

<img src="https://raw.githubusercontent.com/eli64s/readme-ai/eb2a0b4778c633911303f3c00f87874f398b5180/docs/docs/assets/svg/line-gradient.svg" width="100%"/>

## 🤝 Contributing

ReadmeAI is open source and community-driven. All contributions are welcome!

- 📖 **[Contributing Guide](https://github.com/eli64s/readme-ai/blob/main/CONTRIBUTING.md)** — coding standards and workflow
- 🐛 **[Report a Bug](https://github.com/eli64s/readme-ai/issues)** — found something broken?
- 💡 **[Start a Discussion](https://github.com/eli64s/readme-ai/discussions)** — ideas, questions, feedback

[![Contributors](https://contrib.rocks/image?repo=eli64s/readme-ai)](https://github.com/eli64s/readme-ai/graphs/contributors)

<img src="https://raw.githubusercontent.com/eli64s/readme-ai/eb2a0b4778c633911303f3c00f87874f398b5180/docs/docs/assets/svg/line-gradient.svg" width="100%"/>

## 🙏 Acknowledgments

Built on the shoulders of giants:

[![shields.io](https://avatars.githubusercontent.com/u/6254238?s=40&v=4)](https://shields.io) 
[![simpleicons.org](https://avatars.githubusercontent.com/u/29872746?s=40&v=4)](https://simpleicons.org)
[![skill-icons](https://avatars.githubusercontent.com/u/28990589?s=40&v=4)](https://github.com/tandpfun/skill-icons)
[![markdown-badges](https://avatars.githubusercontent.com/u/31800695?s=40&v=4)](https://github.com/Ileriayo/markdown-badges)

<img src="https://raw.githubusercontent.com/eli64s/readme-ai/eb2a0b4778c633911303f3c00f87874f398b5180/docs/docs/assets/svg/line-gradient.svg" width="100%"/>

## 📄 License

Copyright © 2023–2025 [ReadmeAI](https://github.com/eli64s/readme-ai).  
Released under the [MIT License](https://github.com/eli64s/readme-ai/blob/main/LICENSE).

<div align="center">

[![Return to Top](https://img.shields.io/badge/Return_to_Top-5D4ED3?style=flat&logo=ReadMe&logoColor=white)](#-readmeai)

</div>
