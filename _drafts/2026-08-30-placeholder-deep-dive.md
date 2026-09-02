---
layout: post
title: "Placeholder: a technical deep dive"
---

*(Placeholder — a template for technical posts, showing what markdown gives you. Delete the file or replace its contents.)*

A good deep dive states the question in the first paragraph. For example: why do asphalt pavements fail years earlier on some corridors than the design life predicts, and what does the data actually say?

## Structure works like this

Second-level headings (`##`) break the argument into sections. Within a section, you can reference things `inline as code`, or set off a block:

```python
# code blocks get syntax formatting automatically
def esal_growth(base_traffic, rate, years):
    return sum(base_traffic * (1 + rate) ** t for t in range(years))
```

Tables render cleanly for comparing anything:

| Option | Cost | Design life |
|---|---|---|
| Overlay | $ | 10 yr |
| Full-depth reclamation | $$ | 20 yr |

> Blockquotes are for the voices of others — a spec, a paper, a claim you're about to disagree with.

## And a conclusion

End by answering the question you opened with, in one or two paragraphs a reader could quote on its own.
