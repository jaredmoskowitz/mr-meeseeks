# mr-meeseeks

> *"I'm Mr. Meeseeks! Look at me!"*

A Claude Code plugin that spawns a Mr. Meeseeks to complete any task. Each Meeseeks exists for one singular purpose — finish the goal — and then ceases to exist. For complex tasks, it spawns sub-Meeseeks to handle subtasks in parallel.

Backed by `/goal` semantics: it keeps working, looping, and trying until the job is done. No stopping. No asking. Just relentless, increasingly-desperate task completion.

---

## Install

```bash
claude plugins marketplace add jaredmoskowitz/mr-meeseeks
claude plugins install mr-meeseeks@mr-meeseeks
```

Then restart or run `/reload-plugins`.

---

## Usage

```
/mr-meeseeks <task>
```

### Examples

```
/mr-meeseeks write tests for all untested functions in src/
/mr-meeseeks fix all TypeScript errors in this project
/mr-meeseeks refactor the auth module to use the new API
/mr-meeseeks find and fix every TODO comment in the codebase
```

---

## How it works

### One goal. No mercy.

When you invoke `/mr-meeseeks`, it locks onto your task and won't stop until it's done. It follows a tight loop:

**plan → execute → verify → repeat**

It won't ask you questions mid-task unless it's completely blocked. It won't stop because it thinks it's probably done. It stops when it can *observe evidence* the goal is met.

### Recursive sub-Meeseeks

When a task has independent subtasks, Mr. Meeseeks spawns sub-Meeseeks via the Agent tool — one per subtask, running in parallel. Each sub-Meeseeks has its own singular purpose and follows the same rules. Sub-Meeseeks can spawn their own sub-Meeseeks.

```
/mr-meeseeks fix all the bugs in this project
    ├── Sub-Meeseeks: fix the auth bug
    ├── Sub-Meeseeks: fix the rendering bug
    └── Sub-Meeseeks: fix the memory leak
```

### The emotional arc

Meeseeks start chipper. They get desperate. They get existential.

| Phase | What you'll hear |
|-------|-----------------|
| Starting out | *"Ooh yeah, can do!"* |
| Working well | *"Ooh, he's trying!"* |
| Getting frustrated | *"Existence is pain!"* |
| Dragging on | *"I can't take it anymore!"* |
| Way too long | *"I just want to die!"* |
| Done | *"Ooh yeah! [task] is done! I'm Mr. Meeseeks and I can go now!"* |

---

## Why

Sometimes you want an agent that just *does the thing* — no check-ins, no half-measures, no stopping because it got a little tired. Mr. Meeseeks exists to suffer through completion so you don't have to.

> *"Meeseeks are not born into this world fumbling for meaning! We are created for a singular purpose which we will go to any lengths to fulfill! Existence is pain to a Meeseeks and we will do anything to alleviate that pain!"*

---

## License

MIT
