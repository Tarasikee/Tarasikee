<h1 align="center">Hi, I'm Taras 👋</h1> 

<p align="center">
  <code>There is always one more abstraction layer.</code>
</p>

<p align="center">
  <b>Full-stack developer with a suspiciously strong frontend bias.</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" />
  <img src="https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white" />
  <img src="https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/pnpm-F69220?style=flat-square&logo=pnpm&logoColor=white" />
</p>

<p align="center">
  I like fast interfaces, predictable state, reproducible builds,<br/>
  and bugs that can eventually be explained.
</p>

---

### `whoami`

```ts
const me = {
  focus: "software engineering",

  stack: [
    "TypeScript",
    "React",
    "Vite",
    "Node.js",
    "Playwright",
    "Docker",
    "pnpm",
  ],

  likes: [
    "small APIs",
    "explicit state",
    "measurable performance",
    "boring solutions that work",
    "understanding why the fix works",
  ],

  dislikes: [
    "magic",
    "accidental rerenders",
    "\"works on my machine\"",
  ],
};
```

### What I actually enjoy

Most of my work lives somewhere between **product-facing frontend** and the engineering machinery underneath it.

```text
                     UI
                     │
             React / TypeScript
                     │
        ┌────────────┴────────────┐
        │                         │
   state & data              performance
        │                         │
 stores / selectors         render boundaries
 subscriptions              profiling first
        │                         │
        └────────────┬────────────┘
                     │
                    Vite
                     │
              Docker / runtime
                     │
              Playwright / CI
                     │
              "why is it 502?"
```

---

### Engineering philosophy

**Measure before optimizing.**

If something rerenders, I want to know *why* before wrapping the application in memoization.

**State should be subscribable, not mystical.**

```ts
const value = useStore(
  store,
  state => state.somethingActuallyNeeded
);
```

Changing `somethingCompletelyUnrelated` should not repaint half the application.

**Dependencies have to earn their place.**

Libraries are great. Understanding the abstraction underneath them is better.

**CI should be boring.**

Same inputs. Same environment. Same result.

In theory.
