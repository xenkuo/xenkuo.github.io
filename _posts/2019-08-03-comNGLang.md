---
layout: xen-page
title: comNG Introduction
---

## Introduction

comNGLang is a simple language defined by comNG, the purpose is to highlight log text without extra decorator chars. Thanks to [monaco](https://microsoft.github.io/monaco-editor/index.html) editor, it make this possible.

## Syntax

We defined 10 tokens in comNGLang, each token has a regex to match certain character pattern and render this pattern with certain color. In following section, we will give out regex and description for each token.

### Regex

Have a look at these regex, it's the most precise description of comNGLang syntax definition.

{% highlight js linenos %}
[/^\[?[f|F][a|a][t|T][a|a][l|L]\]?\s._/, 'fatal'],
[/\s+\[?[f|F][a|a][t|T][a|a][l|L]\]?\s+/, 'fatal'],
[/^\[?F\]?\s._/, 'fatal'],
[/\s+\[?F\]?\s+/, 'fatal'],
[/^\[?[e|E][r|r][r|R][o|o][r|R]\]?\s._/, 'error'],
[/\s+\[?[e|E][r|r][r|R][o|o][r|R]\]?\s+/, 'error'],
[/^\[?E\]?\s._/, 'error'],
[/\s+\[?E\]?\s+/, 'error'],
[/^\[?[w|W][a|a][r|R][n|n]\]?\s._/, 'warn'],
[/\s+\[?[w|W][a|a][r|R][n|n]\]?\s+/, 'warn'],
[/^\[?W\]?\s._/, 'warn'],
[/\s+\[?W\]?\s+/, 'warn'],
[/^\[?[i|I][n|n][f|F][o|o]\]?\s._/, 'info'],
[/\s+\[?[i|I][n|n][f|F][o|o]\]?\s+/, 'info'],
[/^\[?I\]?\s._/, 'info'],
[/\s+\[?I\]?\s+/, 'info'],
[/^\[?[t|T][r|r][a|A][c|c][e|E]\]?\s._/, 'trace'],
[/\s+\[?[t|T][r|r][a|A][c|c][e|E]\]?\s+/, 'trace'],
[/^\[?T\]?\s._/, 'trace'],
[/\s+\[?T\]?\s+/, 'trace'],
[/^\[?[d|D][e|e][b|B][u|u][g|G]\]?\s._/, 'debug'],
[/\s+\[?[d|D][e|e][b|B][u|u][g|G]\]?\s+/, 'debug'],
[/^\[?D\]?\s._/, 'debug'],
[/\s+\[?D\]?\s+/, 'debug'],
[/^\d{1,2}:\d{2}:\d{2}:\d{1,3}\s/, 'timestamp'],
[/\d{1,4}(-|\/|\.|:)\d{1,2}\1\d{1,4}/, 'time'],
[
/(25[0-5]|2[0-4]\d|[0-1]\d{2}|[1-9]?\d)\.(25[0-5]|2[0-4]\d|[0-1]\d{2}|[1-9]?\d)\.(25[0-5]|2[0-4]\d|[0-1]\d{2}|[1-9]?\d)\.(25[0-5]|2[0-4]\d|[0-1]\d{2}|[1-9]?\d)/, 'ip'
],
[
/[0-9a-fA-F]{2}:[0-9a-fA-F]{2}:[0-9a-fA-F]{2}:[0-9a-fA-F]{2}:[0-9a-fA-F]{2}:[0-9a-fA-F]{2}/, 'mac'
]

{% endhighlight %}

### Color Map

{% highlight js linenos %}
{ token: 'fatal', foreground: 'e91e63' },
{ token: 'error', foreground: 'f44336' },
{ token: 'warn', foreground: 'ff9800' },
{ token: 'info', foreground: '9e9e9e' },
{ token: 'trace', foreground: '607d8b' },
{ token: 'debug', foreground: '795548' },
{ token: 'timestamp', foreground: '009688' },
{ token: 'time', foreground: '2196f3' },
{ token: 'ip', foreground: '03a9f4' },
{ token: 'mac', foreground: '00bcd4' }
{% endhighlight %}

### Fatal

Start with `[fatal]`(case ignore, [] optional, end with at least 1 space) or `[F]`(case sensitive, [] optional, end with at least 1 space), the whole line will be rendered as fatal line.

Single `[fatal]`(case ignore, [] optional, start/end with at least 1 space) or `[F]`(case sensitive, [] optional, start/end with at least 1 space), the word will be rendered as fatal word.

### Error

Take same format as `Fatal` but with a different color.

### Warn

Take same format as `Fatal` but with a different color.

### Info

Take same format as `Fatal` but with a different color.

### Trace

Take same format as `Fatal` but with a different color.

### Debug

Take same format as `Fatal` but with a different color.

### Timestamp

Timestamp is appended automatically by comNG if you enabled `Receive Timestamp` feature. It lies at the head of each line.

### Time

Time is a ordinary text pattern like `2019-08-03` or `12:03:05` or `05-03-2014` etc. Supported separators include `-`, `/`, `.`, `:`.

### IP and Mac

Just the standard IP and Mac string. Supported separators include `-`, `/`, `.`, `:`.
