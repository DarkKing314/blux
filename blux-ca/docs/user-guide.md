# 📘 BLUX-cA User Guide

Welcome to BLUX-cA—the modular, privacy-first coding agent.

---

## Basic Usage

- Launch with:
  ```bash
  python3 cli.py q "Your prompt here"

Use other CLI commands as described in the README and docs/config.md



---

Commands

```
q [prompt] — Query the Hive Mind (main engine group)

memory save [name] — Save current memory state

memory load [name] — Load saved memory state

cs u — Upload state to cloud (future/optional)

cs d — Download state from cloud (future/optional)
```

See docs/config.md for customizing commands and configuration.


---

Examples

```
python3 cli.py q "Refactor this function for readability."
python3 cli.py memory save project_1
python3 cli.py --models
```

---
