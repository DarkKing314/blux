# 🔌 BLUX Plugins Guide

Extend BLUX’s power and creativity!  
Plugins are the heart of the BLUX ecosystem, enabling anyone to add new engines, AI models, tools, and features.

---

## What is a Plugin in BLUX?

A plugin is a modular Python file or package that adds new capabilities to the BLUX system.  
Plugins can wrap AI models, provide tools/utilities, or create custom agents for your workflows.

- **Drop-in:** Place a Python module in the plugins directory
- **Configurable:** Register your plugin in `engines.json` or your `.bluxrc` file
- **Flexible:** Supports both synchronous and asynchronous (async/await) engines

---

## How to Create a Plugin

1. **Copy the Template:**  
   Use the official plugin template below or copy `sample_plugin.py` from any BLUX repo.

2. **Implement the Engine:**  
   Write a `run(prompt)` function (sync or async) that processes the input and returns output.

3. **(Optional) Add Metadata:**  
   Set `ENGINE_DESCRIPTION` and `ENGINE_VERSION` for documentation.

4. **Register the Plugin:**  
   Add your plugin to `engines.json` or your config file.

---

## Plugin Template

"""
BLUX Hive Mind Engine Plugin Template

- Define `run(prompt)` (sync) or `async def run(prompt)` (async)
- Optionally, set `IS_ASYNC = True` for async plugins.
- Add metadata if desired.
"""

```
IS_ASYNC = False  # Set to True if run() is async

def run(prompt):
    # Your engine/model logic goes here
    return f"MyPlugin: {prompt}"

ENGINE_DESCRIPTION = "Describe your engine here."
ENGINE_VERSION = "0.1.0"
```

---

Registering Plugins

Update your engines.json (or project config):

```
[
  { "name": "MyPlugin", "plugin": "my_plugin" }
]
```

Make sure the Python file is in your plugins/ folder.


---

Plugin Security

⚠️ Plugins can run arbitrary Python code. Only use trusted plugins!
If you use third-party plugins, audit their code or run in a sandboxed environment.


---

Sharing and Discovering Plugins

Share your plugin via Pull Request to the BLUX repo

Showcase in GitHub Discussions

Document your plugin clearly for others to use



---

Best Practices

Keep plugins modular and single-purpose

Document all public functions and metadata

Use async only if your engine is async-compatible

Version your plugins!



---

> The BLUX plugin system is your portal to limitless customization—build, share, and remix to shape the future of modular AI!



---

