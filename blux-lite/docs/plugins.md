# 🔌 Plugins in BLUX-Lite

**BLUX-Lite** supports Python plugins to add new models, engines, and features.

---

## How Plugins Work

- Place `.py` files in the `plugins/` directory.
- Register each plugin in `engines.json`.
- Each plugin should implement a `run(prompt)` function and optional metadata.

---

## Plugin Template

```python
IS_ASYNC = False  # Set to True for async plugins

def run(prompt):
    # Add your logic here
    return f"BLUX-Lite Plugin: {prompt}"

ENGINE_DESCRIPTION = "Describe your plugin."
ENGINE_VERSION = "0.1.0"
```

---

Registering Plugins

Edit engines.json:
```
[
  { "name": "LitePlugin", "plugin": "lite_plugin" }
]
```

---

Security

⚠️ Only use trusted plugins. Always audit code you add or download.


---

Share Your Plugins

Contribute via PR or share in BLUX Discussions.



---

> BLUX-Lite: Lightweight, extendable AI for everyone.



---
