# 🔌 Plugins in BLUX-Quantum

BLUX-Quantum is built for extensibility.  
Plugins let you add, remove, and combine new AI engines, commands, and automations.

---

## How Plugins Work

- Drop `.py` plugin files into the `plugins/` folder
- Register them in `engines.json` or `.bluxrc`
- Each plugin should implement a `run(prompt)` or CLI command

---

## Plugin Template

```python
IS_ASYNC = False  # True for async plugins

def run(prompt):
    # Plugin logic goes here
    return f"QuantumPlugin: {prompt}"

ENGINE_DESCRIPTION = "Describe your plugin."
ENGINE_VERSION = "0.1.0"
```

---

Registering Plugins

In engines.json:
```
[
  { "name": "QuantumPlugin", "plugin": "quantum_plugin" }
]
```

---

Security

⚠️ Use only plugins from trusted sources.
Audit third-party code before running.


---

> Customize Quantum for any workflow with plugins!



---
