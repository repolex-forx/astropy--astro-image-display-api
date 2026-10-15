# Repolex Knowledge Graph of astropy/astro-image-display-api

RDF knowledge graph data for [astropy/astro-image-display-api](https://github.com/astropy/astro-image-display-api), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download astropy/astro-image-display-api
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 8f18e54e6eaaebb3643fa0a2ae8b40ee96828040
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 8f18e54e6eaaebb3643fa0a2ae8b40ee96828040
│           └── chunk-001.nq.gz
├── blob
│   ├── 15e27b2bf5762225c41fe9f97589dd5b2d6788f6.nq.gz
│   ├── 16af41b8ab93798ae64637f8c2426d3ea35cafc6.nq.gz
│   ├── 1f1bb2430900e1fbb8d8a56e45d26a4eb43d0765.nq.gz
│   ├── 23c9122aafbaa508040cf6c27ff325d5faa05cd7.nq.gz
│   ├── 2518862bcef84a807fd1220984e2da66cd0e538d.nq.gz
│   ├── 30083e098be6cfb89bc20605cf21a3553f62f450.nq.gz
│   ├── 32bb24529f92346af26219baed295b7488b77534.nq.gz
│   ├── 4173532dc4be2b611600e0cf8cc1ff100b426fdc.nq.gz
│   ├── 500f0115ce34a9446a8d67c8ea22406b76b7d38a.nq.gz
│   ├── 5aab9215ac1022e2f29ee2fef274354c9356c79d.nq.gz
│   ├── 642a9dc257bb053a26fa2dc565207f53d754c983.nq.gz
│   ├── 6eaf4569d40f8a2622474a8f92cf756a9e2869ca.nq.gz
│   ├── 94024237c27e7095899995f30f13a79bf02234ec.nq.gz
│   ├── 95c6a1f1a10fc1b4c69cdf1982d11830a1c416c7.nq.gz
│   ├── 9bf7271e5104a9e074c4416bade449475b399d7b.nq.gz
│   ├── a39c37697d292862a64aa651c1648eae5364a868.nq.gz
│   ├── ad35932dc3b05318c722347cb73a326be49e154b.nq.gz
│   ├── bbbae89637ab5526369b000676afe3746356157b.nq.gz
│   ├── be09c3cce8bc9c6e686d5d13ecc9edf032431e1d.nq.gz
│   ├── bf0af0a9b9f37d18154f167de71c6f5c942601eb.nq.gz
│   ├── cd74dea70248e913ba807755ee15ccd723ad10d2.nq.gz
│   ├── ce7fd633756112a97a70174e833f1bd4eac24ef8.nq.gz
│   ├── d4bb2cbb9eddb1bb1b4f366623044af8e4830919.nq.gz
│   ├── d4c256cd36e01c161d3b89db45c51ac03053479e.nq.gz
│   ├── dc0f75443d394fadc82bcc30467edac485a3ad44.nq.gz
│   ├── ee3a3be1a005610ba43f3f05fb7788ec67ecbaaa.nq.gz
│   ├── ee45bd3c3df3b263cb289b99e546943be6e27631.nq.gz
│   ├── ee72b35d9a89450a6bfd3a54eb7c94d2c152ad2e.nq.gz
│   ├── f0d5d22afe98f38a3030785c27e709153afa6618.nq.gz
│   └── f7d0d0cb9bf392ba999f5793cb06291cbca4502c.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 8f18e54e6eaaebb3643fa0a2ae8b40ee96828040.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 38 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[astropy/astro-image-display-api](https://github.com/astropy/astro-image-display-api)

---
*Parsed on 2026-10-15 by [repolex](https://repolex.ai)*
