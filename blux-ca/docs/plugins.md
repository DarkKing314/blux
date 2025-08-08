# 🔌 Plugins in BLUX-cA

**BLUX-cA** supports plugins to extend its coding, chat, and creative abilities.  
Plugins let you add new AI engines, tools, or integrations—without modifying the core agent.

---

## What Is a Plugin?

A plugin is a Python module placed in the `plugins/` folder.  
Each plugin implements a `run(prompt)` function (sync or async) and optional metadata.

- **Drop-in:** Add your `.py` file to `plugins/`
- **Configurable:** Register it in `engines.json`
- **Flexible:** Supports sync and async logic

---

## Creating a Plugin

1. **Copy this template:**

   
   """
   BLUX-cA Plugin Template

   - Define `run(prompt)` (sync) or `async def run(prompt)` (async)
   - Set `IS_ASYNC = True` if your plugin is async.
   - Add metadata if you like.
   """
```
   IS_ASYNC = False  # Set to True if run() is async

   def run(prompt):
       # Your engine/model logic goes here
       return f"MyPlugin: {prompt}"

   ENGINE_DESCRIPTION = "Describe your engine here."
   ENGINE_VERSION = "0.1.0"
```
2. Save the file in plugins/ (e.g., my_plugin.py).


3. Register your plugin in engines.json:

```
[
  { "name": "MyPlugin", "plugin": "my_plugin" }
]
```



---

Plugin Security

> ⚠️ Security note: Plugins run Python code—use only trusted plugins!
Audit third-party code or sandbox plugins as needed.




---

Best Practices

Single responsibility: Each plugin should focus on one task or engine.

Document all metadata and functions.

Async support: Use IS_ASYNC = True and async def run(prompt) for async engines.

Version: Always update ENGINE_VERSION with changes.



---

Sharing and Discovering Plugins

Share plugins via PRs to BLUX-cA, or in BLUX Discussions.

Clearly document your plugin so others can use it!



---

> BLUX-cA plugins: modular and built for creative coding AI.



---
