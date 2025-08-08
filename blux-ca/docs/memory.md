# 💾 BLUX-cA Memory System

BLUX-cA uses the [Liberation Framework](https://github.com/Justadudeinspace/liberation-framework)  
for secure, user-controlled local memory and persistent agent state.

---

## Key Features

- **User-defined memory**: Save, load, and list “memory states” for projects or tasks
- **No forced cloud**: All memory is local by default
- **Flexible**: Sync to your cloud storage (future)

---

## Memory Commands

- Save memory state:
  ```bash
  python3 cli.py memory save [name]

Load memory state:

```
python3 cli.py memory load [name]
```
List memory states:
```
python3 cli.py memory list
```


---

Under the Hood

Memory is stored as .libf files

Files can be synced, copied, or backed up anywhere you want

See the Liberation Framework for more.


---
