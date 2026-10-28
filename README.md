# Repolex Knowledge Graph of spatialaudio/sfa-numpy

RDF knowledge graph data for [spatialaudio/sfa-numpy](https://github.com/spatialaudio/sfa-numpy), parsed by [repolex](https://repolex.ai).

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
rlex download spatialaudio/sfa-numpy
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── ea94d6af6171cde9de605fd8ef1fd2ecee837f31
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── ea94d6af6171cde9de605fd8ef1fd2ecee837f31
│           └── chunk-001.nq.gz
├── blob
│   ├── 036e6a3abfbe823aa30ffd658141dd242d280db2.nq.gz
│   ├── 03d06047eb5ca15212296c9565813fe3e69431d4.nq.gz
│   ├── 04cde0a016fc230f737deb9db16ae69192c57b2a.nq.gz
│   ├── 08eb60bb3291a815e642af0a8e18b0c0a27ea099.nq.gz
│   ├── 0bba10d71afbfa280ded7453adb4062addface27.nq.gz
│   ├── 11151f801ea6420c39a1c9fdae93719e4281f82c.nq.gz
│   ├── 1873a892ddd782e721892eec7a80603312fa5993.nq.gz
│   ├── 1ec40555dc4d1043253152de9634d462bf0ca3af.nq.gz
│   ├── 2a88a77462d4e96a18a991ab5958409e8624a4da.nq.gz
│   ├── 46d85b0e54e3465961f7287c5a5a4a242bbcfa21.nq.gz
│   ├── 49c1e3d2b35fdff69e6c4e1a9335eaa47eb1acf6.nq.gz
│   ├── 4f799c5745b7835d9780f88aab18547b7691b307.nq.gz
│   ├── 5a6668bb330a9dc04bc12a44c8e291b7351b478e.nq.gz
│   ├── 6205530a54469bb7d3b3f3bbc3f0e5aec5e44b57.nq.gz
│   ├── 649d5b4f7a27e24320ee54088a8bc7fff14ca461.nq.gz
│   ├── 7d8ec4c06c3690db01c256f99d3479baaca2fa6c.nq.gz
│   ├── 7eae0e9b63f2e4dea0eccc8d513f320f9007c2fd.nq.gz
│   ├── 80c872426646d830eba75ce55204b97625353ed6.nq.gz
│   ├── 91078bfaa96df7f0e1ea0f22a68cf56aff9a28f3.nq.gz
│   ├── a2ad9987b76554ae15699bf9963b83b930ba3369.nq.gz
│   ├── aa7726f8eda80e972954469626866c9ecf2d0a5d.nq.gz
│   ├── b002368e70bcf4233dd8d09491d2c609396ef550.nq.gz
│   ├── bb79ada2165ce408f1f1fbe8147d716ac1c5f470.nq.gz
│   ├── cb6945e70f07b321efd9c5a5439c4c5dd8171e00.nq.gz
│   ├── cc2b2ef344c76830911368ccc27a84212b671fac.nq.gz
│   ├── e539e2b17cd2072dd50bf4ca52768ccc93668960.nq.gz
│   ├── e6bae1799aa1a4551ae7e1da2bf996795257459a.nq.gz
│   ├── eeff17955e43da8ead76fd9f8142c9bdbab0765b.nq.gz
│   ├── f7036ad171f84f32479e698abddcec505adae5dc.nq.gz
│   ├── f8ef38938ee09c5109ad4b4b977d05cb56c27d58.nq.gz
│   └── fcbcabc526d593055598a9df0ab960b6be0a0ce5.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── ea94d6af6171cde9de605fd8ef1fd2ecee837f31.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 39 files
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

[spatialaudio/sfa-numpy](https://github.com/spatialaudio/sfa-numpy)

---
*Parsed on 2026-10-28 by [repolex](https://repolex.ai)*
