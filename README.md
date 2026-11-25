# worksheet-maker

A Claude skill that turns lecture materials into study worksheets for engineering courses (heat transfer, metal forming, and more). Upload your course materials, and it builds a complete set — concept explanations, worked examples, problems, and solutions — as a PDF.

## What it makes

Each worksheet follows the order of a typical problem book.

1. **Concepts** — Explained in a conversational tone, like a tutor talking a student through it. Each concept goes: what it is → cause and effect → equation → reading the equation in plain words → how to use it in problems.
2. **Worked examples** — Every step comes with its reasoning. Later examples leave more steps blank for the learner to fill in (backward fading).
3. **Check questions** — Short questions that make you recall the concept without looking back.
4. **Practice problems** — Problem types are mixed, so you have to decide which method to use (interleaving).
5. **Cumulative review and transfer problems** — Mix in earlier units and apply ideas to unfamiliar situations.
6. **Solutions** — Not just answers: the full working, why that method was chosen, and common mistakes.

Figures from the lecture materials are cropped and placed where they help. Every number is computed and checked with code.

## Installation

For Claude Code and other coding agents:

```bash
npx skills add uncledaddychgi/worksheet-maker
```

For the Claude app, zip the `worksheet-maker` folder and upload it as a skill.

## Usage

Upload your lecture materials (PDF, photos, or slides) and ask something like "Make a worksheet for this unit." If the scope isn't clear from the materials, the skill asks once before starting. Unless you ask for another format, the output is a PDF.

## Language

The skill instructions are written in Korean, and worksheets are written in Korean by default. To get a worksheet in another language, just ask for it in your request.

## File structure

```
worksheet-maker/
└── SKILL.md
```
