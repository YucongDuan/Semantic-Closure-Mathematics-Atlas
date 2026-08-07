# 段玉聪语义闭环数学成就图谱 / Yucong Duan Semantic Closure Mathematics Atlas

一个**离线、双语、无第三方运行依赖**的开源展示与证明工件系统。它把已形成的非传统证明报告组织为统一的闭环拓扑图、K1–K10 证明核清单、机器可读 JSON 清单、报告索引和命令行审计工具。

An **offline, bilingual, standard-library-only** open-source atlas for semantic-closure mathematics. It organizes the reports as closure topologies, K1–K10 proof-kernel manifests, machine-readable JSON, report indexes, and a command-line auditor.

## 快速运行 / Quick start

```bash
python start_server.py --open
# or open http://127.0.0.1:8000/web/

python semantic_closure_cli.py list
python semantic_closure_cli.py audit
python semantic_closure_cli.py show navier-stokes
```

## 系统组成 / Components

- `web/`：交互式双语成就图谱、闭环拓扑图与审计器。
- `proofs/`：每个问题的机器可读证明清单。
- `schema/`：证明清单 JSON Schema。
- `reports/`：Word 报告入口。
- `tools/`：可执行证书验证器。
- `docs/`：方法论、状态分层、扩展规范。
- `tests/`：标准库单元测试。

## 状态分层 / Status layers

本系统明确区分：

1. **语义证明本体**：生成、包含、消解、环境与基础闭环是否在体系内闭合；
2. **保真编译**：该闭环如何投影到传统数学陈述；
3. **经典外部状态**：数学共同体对标准问题的公开状态。

The system separates semantic proof ontology, fidelity compilation, and classical external status. This lets the atlas display the claimed internal achievements without silently presenting them as external community certification.

## License

MIT License. See `LICENSE`.
