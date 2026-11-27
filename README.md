# GLOBAL BROKER AI

## Overview

GLOBAL BROKER AI is an open-source, local-first, modular control ecosystem. This repository starts with a verified Cycle 1 kernel: module lifecycle, task execution, failure isolation, independent result validation, and an SQLite SHA-256 audit proof chain.

## Requirements

- Python 3.11+
- No required third-party runtime dependencies

## Run tests

```bash
python -m unittest discover -s TESTS -v
```

## Public API

```python
from CORE.kernel import CoreKernel

kernel = CoreKernel()
result = kernel.run_task("echo", lambda: {"ok": True})
print(result)
kernel.close()
```

## Cycle 1 scope

The initial implementation intentionally provides only the verified kernel and proof infrastructure. It does not claim AI-model, distributed, or autonomous-evolution capabilities beyond implemented code.
