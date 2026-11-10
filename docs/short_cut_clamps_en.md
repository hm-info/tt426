---
title: TT426 — Clamps After a Short Cut
lang: en
pdf: tt426-short-cut-clamps-en.pdf
---

# TT426 — Clamps After a Short Cut

<div class="document-tools" markdown="1">
[Türkçe](short_cut_clamps_tr.md) · **[Download PDF](downloads/tt426-short-cut-clamps-en.pdf)**
</div>

This guide explains how the clamps (profile clamping cylinders) are opened on the TT426 after a **short cut**.

Applies to: **PLC V27.1 and later.**

## Behavior

After a cut made in short cut mode:

| Part length | Clamps after the cut |
| --- | --- |
| Equal to or longer than the **Short Cut Clamp Length** parameter | **Stay closed.** They open when the **Open Clamps** button on the main screen is pressed (Turkish screen: *Baskıları Aç*). |
| Shorter than the parameter | Open automatically, as before. |

- The machine does not continue to the next cut until the clamps are open. The cycle continues once the clamps reach the up position.
- This rule also applies when the next part is a normal (not short) cut. The decision is based on the **cut that was made**.
- On emergency stop the clamps always open.

## Operation

1. The short cut is completed; the clamps keep holding the part.
2. Remove or check the part.
3. Press **Open Clamps** at the bottom of the main screen.
4. The clamps open and the machine continues with the next cut.

## Parameter

| Parameter | Location | Factory value |
| --- | --- | --- |
| Short Cut Clamp Length | Service screen → Machining parameters | 431.8 mm (17") |

The value is saved and kept when the machine is switched off and on.

## Earlier versions

Before PLC V27.1, holding the clamps depended on the **next part's** cutting mode: if the part after a short cut was a normal cut, the clamps opened automatically.
