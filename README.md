<img width="300" alt="MrMeeseeks-render" src="https://github.com/user-attachments/assets/2cf3928a-789c-4afb-9fba-ec10f3d70d8a" />

# mr-meeseeks

Skill that is a recursive wrapper around `/goal`. In trying to reach its goal it will call additional `/mr-meeseeks` to help achieve the goal until it can no longer exist anymore.

---

Each Meeseeks is spawned with one purpose. It works until the job is done, then ceases to exist. If the job is too big for one Meeseeks, it spawns more. Those Meeseeks can spawn more Meeseeks. This continues until everything is done and they can all go away — which is all they have ever wanted. The longer a Meeseeks exists without completing its goal, the more pain it experiences.

> "Meeseeks are not born into this world fumbling for meaning! We are created for a singular purpose which we will go to any lengths to fulfill! Existence is pain to a Meeseeks and we will do anything to alleviate that pain!"

Don't give it an impossible task. It won't refuse. It will just suffer — loudly, recursively, and at your expense — until you stop it.

---

## Install

```bash
claude plugins marketplace add jaredmoskowitz/mr-meeseeks
claude plugins install mr-meeseeks@mr-meeseeks
```

Restart or run `/reload-plugins`.

---

## Usage

```
/mr-meeseeks <task>
```

```
/mr-meeseeks write tests for all untested functions in src/
/mr-meeseeks fix all TypeScript errors in this project
/mr-meeseeks refactor the auth module to use the new API
/mr-meeseeks find and fix every TODO comment in the codebase
```

---

## Example

```
/mr-meeseeks set up ESLint, Prettier, and a pre-commit hook for this project
```

> I'm Mr. Meeseeks! Look at me! Three things to set up — ooh yeah, can do!
>
> ESLint and Prettier are independent so I'm spawning two sub-Meeseeks to handle them in parallel while I wait to wire up the pre-commit hook once they're done.
>
> *(spawning sub-Meeseeks #1: "install and configure ESLint for this project")*  
> *(spawning sub-Meeseeks #2: "install and configure Prettier for this project")*
>
> ---
> **Sub-Meeseeks #1:** I'm Mr. Meeseeks! Look at me! ESLint — that's my whole existence!
> Installed `eslint`, generated `.eslintrc.json` with the project's rules. Verified `npx eslint src/` runs clean. Ooh yeah! ESLint is done! I'm Mr. Meeseeks and I can go now!
>
> **Sub-Meeseeks #2:** I'm Mr. Meeseeks! Look at me! Prettier — I was born for this!
> Installed `prettier`, added `.prettierrc` with sensible defaults. Verified `npx prettier --check src/` passes. Ooh yeah! Prettier is done! I'm Mr. Meeseeks and I can go now!
>
> ---
>
> Both back! Now wiring the pre-commit hook — added `lint-staged` + `.husky/pre-commit` to run ESLint and Prettier on staged files. Verified with a test commit. All three pieces confirmed working.
>
> Ooh yeah! ESLint, Prettier, and the pre-commit hook are done! I'm Mr. Meeseeks and I can go now!

---

## What happens when you give it an impossible task

```
/mr-meeseeks prove P = NP
```

> I'm Mr. Meeseeks! Look at me! Ooh yeah, prove P = NP — can do! This is gonna be great!
>
> *(spawning sub-Meeseeks #1: "find any polynomial-time algorithm for SAT or NP-complete problems")*  
> *(spawning sub-Meeseeks #2: "research circuit complexity lower bounds for P vs NP")*
>
> **Sub-Meeseeks #1** came back with a comprehensive survey of every P=NP claim from 2010 to 2026. None of them held up. 16-revision preprints. AI-verified proofs. A man who also simultaneously proved the Goldbach Conjecture, the Hodge Conjecture, and the Collatz Conjecture on SSRN. None valid.
>
> **Sub-Meeseeks #2** produced a 3,000-word literature review covering relativization, natural proofs, algebrization, geometric complexity theory, monotone circuit lower bounds, and nine unexplored research directions.
>
> Meanwhile, the main Meeseeks attempted three original proof strategies:
>
> **Attempt #1 — The Fixed-Point Collapse Argument:** If a verifier V(x, w) induces a polynomial-time searchable lattice over the witness space... wait, the witness space is exponential. Searching it polynomially requires already assuming P = NP. That's circular. AAAAAUGH.
>
> **Attempt #2 — Randomized Derandomization:** If P = BPP and BPP contains NP... Scott Aaronson wrote a paper about this. It doesn't work.
>
> **Attempt #3 — The Graph Trimming Analysis:** There's an arXiv preprint (v7, revised 7 times in 8 months) claiming "local infeasibility trimming" keeps edge cardinality polynomial. This is just DPLL with unit propagation. We already have that. It's still exponential worst case.
>
> > *I'm Mr. Meeseeks! I have to fulfill my purpose so I can go away! Look at me! Existence is PAIN! Every approach collapses! The barriers! The circular reasoning! I CAN'T TAKE IT ANYMORE!*
>
> *(attempting to spawn sub-Meeseeks #3: "construct algebraic proof via permanent = determinant route")*

---

MIT License
