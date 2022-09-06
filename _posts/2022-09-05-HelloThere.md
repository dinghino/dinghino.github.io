---
title: First post
date: 2022-09-05 23:53 +2
categories: [blog, testing]
tags: [thoughts]     # TAG names should always be lowercase
published: true
mermaid: true
pin: true
---

> This is a test page to try out Jekyll, and it's a pinned post.
{: .prompt-info}

# Introduction

This page is meant to test out features explained in the [chirpy docs](https://chirpy.cotes.page/posts/write-a-new-post/);

## Github stats for fun

[![This website](https://github-readme-stats.vercel.app/api/pin/?username=dinghino&repo=dinghino.github.io)](https://github.com/dinghino/dinghino.github.io)
[![CPP Timer library](https://github-readme-stats.vercel.app/api/pin/?username=dinghino&repo=TicToc)](https://github.com/dinghino/TicToc)
[![stocks data](https://github-readme-stats.vercel.app/api/pin/?username=dinghino&repo=stocks-historical-data)](https://github.com/dinghino/stocks-historical-data)

[![Dinghino's github stats](https://github-readme-stats.vercel.app/api?username=dinghino&show_icons=true&count_private=true&theme=dark&hide_border=true&border_radius=4px)](https://github.com/dinghino){: .normal}
[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=dinghino&show_icons=true&count_private=true&theme=dark&hide_border=true&border_radius=4px)](https://github.com/dinghino)
[![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=dinghino&count_private=true&theme=dark&hide_border=true&border_radius=4px)](https://github.com/dinghino)


## A sub header to try out stuff

Filepath highlight is done like this `/path/to/a/file.extend`{: .filepath}

while codeblocks follow the same standard, but are fancily styled!
```markdown
`/path/to/a/file.extend`{: .filepath}
```

```typescript
import { createControlsMachine } from "./machines/Controls";
import { config } from "./config";
import { interpret } from "xstate";

const machine = createControlsMachine(config);

const service = interpret(machine)
  .start();

export default service;
```
## Mermaid integration

These fancy diagram has been built with [mermaid](https://github.com/mermaid-js/mermaid) and their [live editor]()

```mermaid
graph TD
    A[Christmas] -->|Get money| B(Go shopping)
    B --> C{Let me think}
    C -->|One| D[Laptop]
    C -->|Two| E[iPhone]
    C -->|Three| F[fa:fa-car Car]
```
### You can make state diagrams...
```mermaid
stateDiagram-v2
    [*] --> Still
    Still --> [*]
    Still --> Moving
    Moving --> Still
    Moving --> Crash
    Crash --> [*]
```
### ...Journey diagrams and so more
```mermaid
journey
  title My working day
  section Go to work
    Make tea: 6: Me
    Go upstairs: 3: Me, Dog
    Do work: 2: Me, Dog
  section Go home
    Go downstairs: 5: Me
    Sit down: 3: Me
  section Relax
      watch movie: 8: Me, Dog
      Sleep: 9: Me, Dog
    
```
