<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=32&pause=1000&center=true&vCenter=true&width=700&lines=AI+Full+Stack+Developer;Building+Scalable+SaaS+%26+AI+Products;Automation+%7C+APIs+%7C+Dashboards" alt="Typing SVG" />
</div>

> *The last README you'll ever write by hand.*

**AI-powered README generation — for every language, framework, and developer.**

[![CI](https://img.shields.io/github/actions/workflow/status/eli64s/readme-ai/release-pipeline.yml?logo=githubactions&label=CI&logoColor=white&color=4F46E5&style=flat-square)](https://github.com/eli64s/readme-ai/actions)
[![Coverage](https://img.shields.io/codecov/c/github/eli64s/readme-ai?logo=codecov&logoColor=white&label=Coverage&color=7C3AED&style=flat-square)](https://app.codecov.io/gh/eli64s/readme-ai)
[![PyPI](https://img.shields.io/pypi/v/readmeai?logo=python&logoColor=white&label=PyPI&color=7F77DD&style=flat-square)](https://pypi.python.org/pypi/readmeai/)
[![Downloads](https://img.shields.io/pepy/dt/readmeai?logo=pypi&logoColor=white&label=Downloads&color=6D28D9&style=flat-square)](https://www.pepy.tech/projects/readmeai)
[![Stars](https://img.shields.io/github/stars/eli64s/readme-ai?logo=github&logoColor=white&label=Stars&color=4338CA&style=flat-square)](https://github.com/eli64s/readme-ai/stargazers)
[![License](https://img.shields.io/github/license/eli64s/readme-ai?logo=opensourceinitiative&logoColor=white&label=License&color=3730A3&style=flat-square)](https://opensource.org/license/mit/)

<br/>

```
❯ pip install readmeai && readmeai --api openai -r https://github.com/your/project
  ✓  README.md generated in 12.3s
```

<br/>

**[🚀 Quickstart](#-getting-started)** · **[✨ Features](#-features)** · **[⚙️ Configuration](#️-configuration)** · **[🖼 Gallery](#-example-gallery)** · **[🤝 Contributing](#-contributing)**

<img src="https://raw.githubusercontent.com/eli64s/readme-ai/eb2a0b4778c633911303f3c00f87874f398b5180/docs/docs/assets/svg/line-gradient.svg" width="100%" alt="divider"/>

</div>

## 🧠 What is ReadmeAI?

**ReadmeAI** scans your entire codebase — local directory or remote URL — and generates a beautifully structured, production-quality `README.md` in seconds, powered by state-of-the-art language models.

No blank-page paralysis. No boilerplate copy-paste. No documentation debt.

| What you do | What ReadmeAI does |
|-------------|-------------------|
| Point at a repo | Analyzes all source files, configs, and dependencies |
| Choose an LLM | Generates project intro, features, architecture, setup guides |
| Run one command | Outputs a fully formatted, customized README.md |

> 🎯 **Designed for simplicity, customization, and developer productivity.**

<img src="https://raw.githubusercontent.com/eli64s/readme-ai/eb2a0b4778c633911303f3c00f87874f398b5180/docs/docs/assets/svg/line-gradient.svg" width="100%" alt="divider"/>

## ✨ Features

### 🎨 Stunning Visual Customization

Every element of your README is yours to control — headers, badge colors and styles, logos, emoji packs, and navigation layouts. Ship docs that match your project's personality.

| Style | Preview | CLI Flag |
|-------|---------|----------|
| **Classic** | ![Classic](https://github.com/eli64s/readme-ai/raw/main/docs/docs/assets/img/documentation/headers/variations/custom-dragon.png?raw=true) | `--header-style classic` |
| **Modern** | ![Modern](https://github.com/eli64s/readme-ai/raw/main/docs/docs/assets/img/documentation/headers/variations/modern-for-the-badge.png?raw=true) | `--header-style modern` |
| **Compact** | ![Compact](https://github.com/eli64s/readme-ai/raw/main/docs/docs/examples/styling/headers/compact.png?raw=true) | `--header-style compact` |
| **Console** | ![Console](https://github.com/eli64s/readme-ai/raw/main/docs/docs/examples/styling/headers/console.png?raw=true) | `--header-style console` |
| **SVG Banner** | ![Banner](https://github.com/eli64s/readme-ai/raw/main/docs/docs/examples/styling/headers/svg-banner.png?raw=true) | `--header-style banner` |

---

### 🤖 Model Agnostic — Your AI, Your Rules

Switch between the world's leading LLMs with a single flag. Or run entirely offline.

| Provider | Flag | Best For | Cost |
|----------|------|----------|------|
| **OpenAI** | `--api openai` | Industry-leading general quality | Paid |
| **Anthropic Claude** | `--api anthropic` | Advanced reasoning, nuanced docs | Paid |
| **Google Gemini** | `--api gemini` | Multimodal, cutting-edge | Paid |
| **Ollama** | `--api ollama` | 100% local, any open model | **Free** |
| **Offline Mode** | `--api offline` | Structure only, no AI | **Free** |

---

### 📄 Every Section, Auto-Generated

ReadmeAI produces complete, professional documentation sections — not templates, not stubs.

<details>
<summary><strong>▸ Click to see what gets generated</strong></summary>

| Section | Description |
|---------|-------------|
| **Project Introduction** | Value proposition, purpose, target audience — crafted by AI |
| **Feature Table** | Structured breakdown of your project's capabilities |
| **Architecture Overview** | Directory tree with module-level summaries |
| **Getting Started** | Auto-detected dependencies, install steps, environment setup |
| **Usage Examples** | Real commands and code snippets pulled from your codebase |
| **Testing Guide** | Test execution instructions, framework-specific commands |
| **Roadmap** | Suggested milestones and future enhancements |
| **Contributing** | Contribution workflow, standards, and community links |
| **License & Acknowledgments** | Auto-detected license, credits, and ecosystem attribution |

</details>

---

### 🌐 Works With Any Codebase, Anywhere

| ✅ Repository Platforms | ✅ Languages & Runtimes | ✅ Frameworks |
|------------------------|------------------------|--------------|
| GitHub | Python, Go, Java | FastAPI, Django |
| GitLab | Kotlin, Rust, C++ | React, Vue, Svelte |
| Bitbucket | TypeScript, JS | Docker, K8s, Terraform |
| Local filesystem | Ruby, Swift, PHP | Spring, Rails, Laravel |

---

### 🧹 Smart Filtering with `.readmeaiignore`

Control exactly which files ReadmeAI analyzes. Same syntax as `.gitignore` — add patterns to exclude generated files, vendor directories, or anything you don't want documented.

<img src="https://raw.githubusercontent.com/eli64s/readme-ai/eb2a0b4778c633911303f3c00f87874f398b5180/docs/docs/assets/svg/line-gradient.svg" width="100%" alt="divider"/>

## 🚀 Getting Started

### Prerequisites

| Requirement | Minimum | Notes |
|-------------|---------|-------|
| Python | 3.9+ | [python.org](https://www.python.org/) |
| LLM API key | — | OpenAI / Anthropic / Gemini — or use Ollama / offline for **free** |

---

### ⚡ Installation

Choose your install method:

```bash
# pip — recommended for most users
❯ pip install -U readmeai

# pipx — keeps readmeai isolated from other projects
❯ pipx install readmeai

# uv — fastest install available
❯ uv tool install readmeai

# Docker — zero-dependency, runs anywhere
❯ docker pull zeroxeli/readme-ai:latest
```

<details>
<summary><strong>▸ Build from source</strong></summary>

```bash
❯ git clone https://github.com/eli64s/readme-ai
❯ cd readme-ai
❯ pip install -r setup/requirements.txt

# Or with Poetry:
❯ poetry install

# Or with the setup script:
❯ bash setup/setup.sh
```

</details>

> **Note — Anthropic or Gemini users:** install the provider extras:
> ```bash
> pip install "readmeai[anthropic]"
> pip install "readmeai[google-generativeai]"
> pip install "readmeai[anthropic,google-generativeai]"
> ```

---

### 🔑 Set Your API Key

```bash
# OpenAI
❯ export OPENAI_API_KEY=<your_key>

# Anthropic
❯ export ANTHROPIC_API_KEY=<your_key>

# Google Gemini
❯ export GOOGLE_API_KEY=<your_key>

# Ollama — no key needed, just start the server
❯ export OLLAMA_HOST=127.0.0.1 && ollama serve
```

---

### 🎬 Generate Your README

**Minimal — start here:**

```bash
❯ readmeai --api openai -r https://github.com/your/project
```

**Switch providers in seconds:**

```bash
# Anthropic Claude
❯ readmeai --api anthropic -m claude-3-5-sonnet-20240620 -r https://github.com/your/project

# Google Gemini
❯ readmeai --api gemini -m gemini-1.5-flash -r https://github.com/your/project

# Local Ollama (free, private)
❯ readmeai --api ollama --model llama3.2 -r https://github.com/your/project

# Fully offline — no AI, no internet
❯ readmeai --api offline -r https://github.com/your/project
```

**Full customization — power user mode:**

```bash
❯ readmeai \
    --repository https://github.com/your/project \
    --api openai \
    --model gpt-4 \
    --output my-readme.md \
    --badge-color A931EC \
    --badge-style flat-square \
    --header-style compact \
    --navigation-style fold \
    --logo LLM \
    --emojis solar \
    --temperature 0.9 \
    --tree-depth 2
```

**Docker:**

```bash
❯ docker run -it --rm \
    -e OPENAI_API_KEY=$OPENAI_API_KEY \
    -v "$(pwd)":/app zeroxeli/readme-ai:latest \
    --repository https://github.com/your/project \
    --api openai
```

---

### 🌐 No-Install Browser Option

[![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://readme-ai.streamlit.app/)

> ⚠️ The Streamlit app may lag behind the CLI on the latest features. Use the CLI for cutting-edge functionality.

---

### 🧪 Testing

```bash
# Install dev + test dependencies
❯ uv pip install --dev --group test --all-extras

# Run the unit test suite
❯ make test

# Test across Python 3.9 / 3.10 / 3.11 / 3.12 via nox
❯ make test-nox
```

<img src="https://raw.githubusercontent.com/eli64s/readme-ai/eb2a0b4778c633911303f3c00f87874f398b5180/docs/docs/assets/svg/line-gradient.svg" width="100%" alt="divider"/>

## ⚙️ Configuration

All options are available as CLI flags. Every single one has a sensible default — customize only what you need.

| Flag | Description | Default |
|------|-------------|---------|
| `--api` | LLM provider (`openai` · `anthropic` · `gemini` · `ollama` · `offline`) | `offline` |
| `--model` / `-m` | LLM model name | `gpt-3.5-turbo` |
| `--repository` / `-r` | Repository URL or local path | *required* |
| `--output` / `-o` | Output filename | `readme-ai.md` |
| `--header-style` | Layout (`classic` · `modern` · `compact` · `console` · `banner`) | `classic` |
| `--badge-style` | Badge look (`flat` · `flat-square` · `for-the-badge` · `plastic`) | `flat` |
| `--badge-color` | Badge color (name or hex, e.g. `A931EC`) | `0080ff` |
| `--navigation-style` | TOC format (`bullet` · `number` · `roman` · `accordion` · `fold`) | `bullet` |
| `--logo` | Logo preset or `custom` for your own image | `blue` |
| `--emojis` | Emoji theme pack (e.g. `solar`, `water`, `rainbow`) | `None` |
| `--temperature` | LLM creativity, 0.0–2.0 | `0.1` |
| `--tree-max-depth` | Directory tree depth | `2` |
| `--align` | Header text alignment | `center` |

```bash
❯ readmeai --help   # full reference
```

📚 **[Full Documentation →](https://eli64s.github.io/readme-ai)**

<img src="https://raw.githubusercontent.com/eli64s/readme-ai/eb2a0b4778c633911303f3c00f87874f398b5180/docs/docs/assets/svg/line-gradient.svg" width="100%" alt="divider"/>

## 🖼 Example Gallery

ReadmeAI-generated READMEs across a wide range of real-world projects:

| Stack | Repository | Generated README | Highlight |
|-------|------------|-----------------|-----------|
| Python | [readme-ai](https://github.com/eli64s/readme-ai) | [View →](https://github.com/eli64s/readme-ai/blob/main/examples/readme-ai.md) | Core project |
| Apache Flink | [pyflink-poc](https://github.com/eli64s/pyflink-poc) | [View →](https://github.com/eli64s/readme-ai/blob/main/examples/headers/modern.md) | Modern style |
| Streamlit | [readme-ai-streamlit](https://github.com/eli64s/readme-ai-streamlit) | [View →](https://github.com/eli64s/readme-ai/blob/main/examples/banners/svg-banner.md) | SVG banner |
| Go + Docker | [docker-gs-ping](https://github.com/olliefr/docker-gs-ping) | [View →](https://github.com/eli64s/readme-ai/blob/main/examples/readme-docker-go.md) | Multi-language |
| FastAPI + Redis | [async-ml-inference](https://github.com/FerrariDG/async-ml-inference) | [View →](https://github.com/eli64s/readme-ai/blob/main/examples/readme-fastapi-redis.md) | ML stack |
| Java | [minimal-todo](https://github.com/avjinder/Minimal-Todo) | [View →](https://github.com/eli64s/readme-ai/blob/main/examples/headers/compact.md) | Compact style |
| Kotlin (Android) | [file.io-Android-Client](https://github.com/rumaan/file.io-Android-Client) | [View →](https://github.com/eli64s/readme-ai/blob/main/examples/readme-kotlin.md) | Mobile app |
| PostgreSQL + DuckDB | [buenavista](https://github.com/jwills/buenavista) | [View →](https://github.com/eli64s/readme-ai/blob/main/examples/headers/classic.md) | Data stack |
| Vercel + NPM | [github-readme-quotes](https://github.com/PiyushSuthar/github-readme-quotes) | [View →](https://github.com/eli64s/readme-ai/blob/main/examples/logos/dalle.md) | Deployment |
| Offline mode | [litellm](https://github.com/BerriAI/litellm) | [View →](https://github.com/eli64s/readme-ai/blob/main/examples/offline-mode/readme-litellm.md) | No API needed |

> 💬 **Generated something great?** Share it in [Show & Tell →](https://github.com/eli64s/readme-ai/discussions/categories/show-and-tell)

<img src="https://raw.githubusercontent.com/eli64s/readme-ai/eb2a0b4778c633911303f3c00f87874f398b5180/docs/docs/assets/svg/line-gradient.svg" width="100%" alt="divider"/>

## 🗺 Roadmap

- [ ] `readmeai v1.0.0` — stable, production-ready release with robust docs creation
- [ ] Extended templates for more project types and programming languages
- [ ] VS Code Extension — generate READMEs directly inside your editor
- [ ] GitHub Actions integration — automatically update docs on every push
- [ ] Badge packs — code coverage, CI status, version, and more

<img src="https://raw.githubusercontent.com/eli64s/readme-ai/eb2a0b4778c633911303f3c00f87874f398b5180/docs/docs/assets/svg/line-gradient.svg" width="100%" alt="divider"/>

## 🤝 Contributing

ReadmeAI is open source and community-driven. All contributions are welcome.

- 📖 **[Contributing Guide](https://github.com/eli64s/readme-ai/blob/main/CONTRIBUTING.md)** — workflow, coding standards, PR process
- 🐛 **[Report a Bug](https://github.com/eli64s/readme-ai/issues)** — something broken? let us know
- 💡 **[Start a Discussion](https://github.com/eli64s/readme-ai/discussions)** — ideas, questions, feedback

[![Contributors](https://contrib.rocks/image?repo=eli64s/readme-ai)](https://github.com/eli64s/readme-ai/graphs/contributors)

<img src="https://raw.githubusercontent.com/eli64s/readme-ai/eb2a0b4778c633911303f3c00f87874f398b5180/docs/docs/assets/svg/line-gradient.svg" width="100%" alt="divider"/>

## 🙏 Acknowledgments

Built on the shoulders of excellent open-source projects:

[![shields.io](https://avatars.githubusercontent.com/u/6254238?s=36&v=4)](https://shields.io)
[![simpleicons.org](https://avatars.githubusercontent.com/u/29872746?s=36&v=4)](https://simpleicons.org)
[![skill-icons](https://avatars.githubusercontent.com/u/28990589?s=36&v=4)](https://github.com/tandpfun/skill-icons)
[![markdown-badges](https://avatars.githubusercontent.com/u/31800695?s=36&v=4)](https://github.com/Ileriayo/markdown-badges)

<img src="https://raw.githubusercontent.com/eli64s/readme-ai/eb2a0b4778c633911303f3c00f87874f398b5180/docs/docs/assets/svg/line-gradient.svg" width="100%" alt="divider"/>

## 📄 License

Copyright © 2023–2025 [ReadmeAI](https://github.com/eli64s/readme-ai).
Released under the [MIT License](https://github.com/eli64s/readme-ai/blob/main/LICENSE).

<div align="center">

[![Back to top](https://img.shields.io/badge/↑_Back_to_top-7F77DD?style=flat-square)](https://github.com/eli64s/readme-ai#-readmeai)

</div>
