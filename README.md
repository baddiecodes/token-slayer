# 🚨 token-slayer

Stop wasting 70–80% of your Claude/GPT context window.

If you’re building in crypto, writing Solidity, auditing protocols, or grinding monorepos — you’re probably burning most of your tokens before your model even does useful work.

This repo is a collection of **real-world patterns + tools** to reduce hidden token waste in AI-assisted development.

---

## 🧠 The Problem

Most token waste doesn’t come from prompts.

It comes from invisible layers:

- Claude.md bloat
- history re-reads
- plugin injection
- tool schema overhead
- unnecessary context loading
- logs and terminal noise
- over-generation loops

Result:

👉 73–80% of tokens are spent before actual reasoning begins.

---

## ⚖️ Reality Check

Claude is powerful for large context (200k–1M tokens),  
but uses more tokens per prompt (~2× vs GPT in many cases).

So efficiency = everything.

---

## 🛠️ Tools (Real Workflow Stack)

This repo documents + organizes tools that reduce token waste:

### Output reduction
- caveman claude — reduces verbose outputs (~75%)

### Terminal / logs filtering
- rtk (rust token killer) — filters terminal output (~60–90%)

### Code-level efficiency
- code review graph — focuses only on relevant code (~49× reduction)

### Context isolation
- context mode — stores output externally (sqlite), avoids context pollution (~98%)

### Prompt optimization
- claude token optimizer — reduces full-project prompt cost (~90%)

### Hidden waste detection
- token optimizer — finds invisible token leakage

### MCP optimization
- token optimizer mcp — caching + compression (~95%+)

### Codebase search efficiency
- claude context — vector search across repo (~40% reduction)

### Strict formatting control
- claude token efficient — enforces minimal context usage

### Navigation optimization
- token savior — symbol-based navigation (~97% reduction)

---

## 🧠 Suggested Stack (by use case)

- Large monorepos → code review graph + token savior  
- Heavy logs → rtk  
- MCP-heavy workflows → context mode  
- Fast wins → caveman + token efficient  

---

## ⚡ Real Impact Example

A 50k-line Solidity monorepo audit:

- before: context exhausted before useful output  
- after: ~49× reduction using structured context filtering  

Large logs:

- 300k tokens → <10k after filtering

---

## 🎯 Goal

Not to “use AI more”

But to:
- use fewer tokens
- get faster outputs
- reduce API cost
- increase signal-to-noise ratio

---

## 📉 Summary

Most devs are not limited by AI quality.

They are limited by **context inefficiency**.

Fix that → everything improves.

---

## 🍒 Contact
https://x.com/withmewtwo 

---

## 💎 License

MIT
