---
layout: xen-page
title: comNG Introduction
---

## Introduction

comNGLang is a simple language defined by comNG, the purpose is to highlight log text without extra decorator chars. Thanks to [monaco](https://microsoft.github.io/monaco-editor/index.html) editor, it make this possible.

## Syntax

We defined 10 tokens in comNGLang, each token has a regex to match certain character pattern and render this pattern with certain color. In following section, we will give out regex for each token, example and color will give out as well.

### Fatal

#### Regex

```js
/^\[?[f|F][a|A][t|T][a|A][l|L]\]?\s.*/
/\s+\[?[f|F][a|A][t|T][a|A][l|L]\]?\s+/
```
