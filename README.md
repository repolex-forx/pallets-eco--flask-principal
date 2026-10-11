# Repolex Knowledge Graph of pallets-eco/flask-principal

RDF knowledge graph data for [pallets-eco/flask-principal](https://github.com/pallets-eco/flask-principal), parsed by [repolex](https://repolex.ai).

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
rlex download pallets-eco/flask-principal
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── f46b75e42d9f7de240bf5f05e1936fb63703070b
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── f46b75e42d9f7de240bf5f05e1936fb63703070b
│           └── chunk-001.nq.gz
├── blob
│   ├── 075e1406de41a490cb7f6bed031ece9db4146a6d.nq.gz
│   ├── 0ec0ae6044821061a27915b64c6e8f9b65d941c1.nq.gz
│   ├── 1492811e49e8edd9dd84b212fa8c5742c4d656ea.nq.gz
│   ├── 16ee7bdbeece98aeabd4c02e189ab10cb5cc203f.nq.gz
│   ├── 1aba38f67a2211cf5b09466d7b411206cb7223bf.nq.gz
│   ├── 1f47f125e5c06e827ba4df75cffd838547a4163a.nq.gz
│   ├── 23d1773c9bce8c85ef767ff6666d42ad93ca082b.nq.gz
│   ├── 2ff985a67af35fdfd1076354b771c425867cdab4.nq.gz
│   ├── 34037aef6bb1fa7ae29333b36735fc57b1dd2274.nq.gz
│   ├── 5f8ceed76107982e5d35f30e33e8d7ee5fcb0c05.nq.gz
│   ├── 637ea0976b6969004503bf5369bf0e1713ac3680.nq.gz
│   ├── 6b79eaa1d6e754caa0986f1f206799c325b95b4c.nq.gz
│   ├── 70c9b4f0bfdf8dcb60362d2a78840e792506e7c5.nq.gz
│   ├── 841b7f9695df1852f714a28f7aeeb8be26dd8b60.nq.gz
│   ├── 8a9aae5d5385c315bf363376cfd2379cbfb94382.nq.gz
│   ├── 9fdb06d614c54fae396c62b14de63d4b565b1f36.nq.gz
│   ├── b3a3862db7e7b5b150d209c3e145f4c4c6aa5852.nq.gz
│   ├── b4fd5a25023f91378596f9061bfe8ba46ae30d48.nq.gz
│   ├── bb1a7559e1785e2d3a7aa574e4daa7445c0ec922.nq.gz
│   ├── d6c5f48c7917bae3cd89fd14a28922e380380820.nq.gz
│   ├── dbb67e35faf4686efb8c52eb25dc763f2f38e6e2.nq.gz
│   ├── e0d9d224db986c5a9fe4d0abb803ae7772aba24e.nq.gz
│   ├── e62e3a41273c8433bedd4977f7b236ddb4c643fe.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── ec9043be996ae628578902c1426cb126d7b0b394.nq.gz
│   └── fbbc1459326a11fb1f94953aa2650716f87121f8.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── f46b75e42d9f7de240bf5f05e1936fb63703070b.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 34 files
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

[pallets-eco/flask-principal](https://github.com/pallets-eco/flask-principal)

---
*Parsed on 2026-10-11 by [repolex](https://repolex.ai)*
