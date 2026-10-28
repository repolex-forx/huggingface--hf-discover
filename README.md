# Repolex Knowledge Graph of huggingface/hf-discover

RDF knowledge graph data for [huggingface/hf-discover](https://github.com/huggingface/hf-discover), parsed by [repolex](https://repolex.ai).

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
rlex download huggingface/hf-discover
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 7f17fe86620729dfb2d1430dc04fa59c07c4f696
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 7f17fe86620729dfb2d1430dc04fa59c07c4f696
│           └── chunk-001.nq.gz
├── blob
│   ├── 04e615343063f30a8c315ae73885afe26a1374c6.nq.gz
│   ├── 06055da29a154f0fa7ac9c2cee34e9433262a9ae.nq.gz
│   ├── 0eb2460768a58faf2cad14285775744c771b288f.nq.gz
│   ├── 15f7bdd7916ac5fca2274ad5d1239bafe0f0f5a2.nq.gz
│   ├── 180299408ace0d5554dcd6d529c564d73dd329a4.nq.gz
│   ├── 19c6ca3decf68d4b8173285bb7e9dedd7c680cc0.nq.gz
│   ├── 1eabddbd4b0310ec29d5a11cad68b642d6f47374.nq.gz
│   ├── 271571e3131d720631469a6ef1f25802bc537c53.nq.gz
│   ├── 325106c4611d3a87951bc84c03cc56d9a86afc2b.nq.gz
│   ├── 33b59c4ecd791e45c8056826a4f49a383f3579a3.nq.gz
│   ├── 358ebc3db7ebdef85203d4788bb23b852ef778ae.nq.gz
│   ├── 3b5f427ce4b935f8d28491792929c5513f52aa18.nq.gz
│   ├── 3e65595ad054e956cbd75c93a6130f6ac815d272.nq.gz
│   ├── 3e835465dc28b3455a004da4701b31a4f3d566f8.nq.gz
│   ├── 42da3342e9054d397729580bc0ccc5ff8fee1f62.nq.gz
│   ├── 42f5f1dbe5094c6991c38ee308eead359aa8d615.nq.gz
│   ├── 44242f3b8c9bcb3fe68067462834a0474526e085.nq.gz
│   ├── 5c5e52f55c7f50ed483164faf36eb8da1c5fdb7a.nq.gz
│   ├── 619f9bd15a2ae540b00ede27e932d3a77ef7cc1a.nq.gz
│   ├── 701945fb9abc736b23990874b1685a7102f85683.nq.gz
│   ├── 711e09f68568389b59c933efc6d7daabed0cb303.nq.gz
│   ├── 724a724f12ae88f1e7fcb882f9623cd8f6b95dee.nq.gz
│   ├── 743b1a40f5c0ee80f2acd8ee6c78318270d6e4f5.nq.gz
│   ├── 7b70396ef2457ce7545716a5302f3bcfdc84698d.nq.gz
│   ├── 8bbf0a50a18580967d3cf521ca3ec802cdcdb766.nq.gz
│   ├── 958709b37ddce76f70fb03b277988b8c8e3ed9ba.nq.gz
│   ├── 9af173238ada1a75d2b210ba8bfab45cd3d69f11.nq.gz
│   ├── a4465b2cc846592db45065d44e21339f4572d985.nq.gz
│   ├── a580078da5f3951183785f58d18764ada32fe239.nq.gz
│   ├── a59b7e1385f826d877f0fad973e9e735823b17c2.nq.gz
│   ├── b3cb5960c1c3d07c35054c8f45fca121cc8cc39f.nq.gz
│   ├── b58f81e46b98e5e272847ee8ef123e753cfc52db.nq.gz
│   ├── b8f2bd1c53220f53ccfc55c9b02fd628306c92ea.nq.gz
│   ├── c656173ba2573142ff300b6c27d190d3556f4878.nq.gz
│   ├── d009f72affa770c24c5f8b10235defe63ab6ca0a.nq.gz
│   ├── d24e38daf2bd2c5bcc865e9a40fdb76893093648.nq.gz
│   ├── d458874227f51fb7cc4569c2abc98175b9dce819.nq.gz
│   ├── e4da8e34cf698e0104f2141772909696775e8bac.nq.gz
│   ├── e5041ee93d44d6818e7ccb02099e919ffeab9dee.nq.gz
│   ├── e6a137c49150c22240436786c7b548ba5ae985d2.nq.gz
│   ├── ea4f6196808d6b2695984bd9ffe66e7c8bf7192d.nq.gz
│   ├── edfed446e5da0a30edf77ca013b7a8e958c7a376.nq.gz
│   ├── f72053faa7918a9cf6f1a7b88c22fe50565c41a0.nq.gz
│   └── fcae2eeaca6065cf4fd1fab4b5d89b2fa8f14b62.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 7f17fe86620729dfb2d1430dc04fa59c07c4f696.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 52 files
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

[huggingface/hf-discover](https://github.com/huggingface/hf-discover)

---
*Parsed on 2026-10-28 by [repolex](https://repolex.ai)*
