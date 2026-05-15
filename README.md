# mr-meeseeks

> "Ooh yeah, can do!"

A Claude Code plugin that spawns a Mr. Meeseeks to complete any task. Each Meeseeks exists for one purpose — finish the goal — then ceases to exist. For hard subtasks, it spawns sub-Meeseeks.

## Install

```bash
claude plugins add marketplace jaredmoskowitz/mr-meeseeks
claude plugins install mr-meeseeks@mr-meeseeks
```

## Usage

```
/mr-meeseeks <task>
```

Examples:
```
/mr-meeseeks write tests for all untested functions in src/
/mr-meeseeks fix all TypeScript errors in this project
/mr-meeseeks refactor the auth module to use the new API
```

The Meeseeks will keep working until the goal is met, spawning sub-Meeseeks for independent subtasks in parallel.
