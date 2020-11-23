---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
year: {{dateFormat "2006" .Date}}
month: "{{dateFormat "01" .Date}}"
aliases: [
    "{{.Name|urlize}}"
]
---

** Insert Lead Paragraph here **

## A new blog post