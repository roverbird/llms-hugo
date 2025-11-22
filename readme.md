# Generating llms.txt with Hugo

This repository demonstrates how to generate an **llms.txt** file using the Hugo static site generator.

## What is `llms.txt`?

`llms.txt` is a Markdown-formatted text file proposed for improving the accessibility of website content to **large language models (LLMs)**. `llms.txt` contributes to generative engine optimization (GEO) of your website.

- LLMs have small context windows and cannot process entire websites easily.
- `llms.txt` provides a concise, structured summary of your website:
  - Title
  - Base URL
  - Description
  - Content index (articles, pages) with summaries
- It is both **human-readable** and **machine-parsable** (for bots or scripts).

**Reference:** 

- LLMS Standard: [https://llmstxt.org/](https://llmstxt.org/)
- LLMS repo: [https://github.com/AnswerDotAI/llms-txt](https://github.com/AnswerDotAI/llms-txt)
- LLMS Info: [https://dev.to/masutaka/added-llmstxt-and-llms-fulltxt-to-my-hugo-built-website-343i](https://dev.to/masutaka/added-llmstxt-and-llms-fulltxt-to-my-hugo-built-website-343i)
- LLMS Example: [https://kibervarnost.si/llms.txt](https://kibervarnost.si/llms.txt)

## Step 1: Configure Hugo

Add `llms` as a custom output format in `config.toml` (already included) - add that to your `config.toml`

## Step 2: Create `index.llms.txt` Template

Already included in `/layouts/index.llms.txt`.

## Step 3: Build Hugo Site

```bash
hugo
