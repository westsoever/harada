# Harada

A one-page website for filling in a Harada sheet (the "Open Window 64" grid), plus a printable worksheet that helps you work out what goes in it.

## What's here

| File | What it is |
|---|---|
| `index.html` | The website. Fill in the sheet, then print it or save it as a PDF. |
| `harada-worksheet.pdf` | An empty 23-page worksheet to print and fill in by hand. |
| `worksheet.html` | The source of the worksheet PDF. |

## The Harada method in short

Takeshi Harada, a Japanese track coach, built a 9×9 grid for planning a big goal. Shohei Ohtani made it famous with the chart he filled in at high school.

- The **main goal** goes in the centre.
- The 8 cells around it hold **8 goals** (Harada calls them pillars): the areas that have to go right to reach the main goal.
- Each of those 8 goals repeats in the centre of its own outer block, and gets **8 subgoals** (actions) around it: concrete things you do.

That makes 1 + 8 + 64 cells. The grid is only one part of Harada's method. The worksheet covers the rest: why you want the goal, what went right and wrong in the past, which 10 tasks to start with, and how to keep going.

## Using the website

Open `index.html` in a browser. Nothing to install, no account, no server.

- **9×9 grid**: click a cell and type. Enter moves to the next cell, Shift+Enter starts a new line. A goal typed in the centre block also appears in the centre of its outer block.
- **List**: the same sheet as an outline, with the main goal at the top and each goal's 8 subgoals indented under it. You can edit here too.
- **Print / PDF**: prints the tab that is open. The grid prints on one landscape A4 page and the list on portrait A4. In the print dialog, choose "Save as PDF" to keep a copy.
- **Worksheet (PDF)**: downloads the empty worksheet.

Your sheet is saved in your own browser (local storage). It is never sent anywhere, so it isn't available on another device or browser, and clearing your browser data deletes it. Print or save a PDF to keep it.

The 8 goals are numbered clockwise from the top-left, the same order as the worksheet, so you can copy your answers across in order.

## Using the worksheet

Print `harada-worksheet.pdf` and fill it in by hand, in pencil first. It asks questions and leaves the answers to you:

1. **Step 0, the goal form**: sharpen the goal, write down what it gives you and others, look at past successes and failures, pick a coach or mentor.
2. **Round 1**: collect ideas with six prompts (a pre-mortem, your easiest and worst days, and more), group them into themes and cut them to 8 goals.
3. **Round 2**: one page per goal with 8 actions each, every action with a "bad-day version" for days when it all goes wrong.
4. **Open Window 64**: an empty 9×9 grid to copy everything into. Or type it into the website instead.
5. **Step 3**: choose 10 tasks and 10 new routines to start with, not all 64.
6. **Step 4**: decide how you will keep it running (a check sheet, a diary, reviews).

## Changing the worksheet

Edit `worksheet.html`, then rebuild the PDF with Chrome:

```sh
"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" --headless --no-pdf-header-footer \
  --print-to-pdf=harada-worksheet.pdf worksheet.html
```

## Sources

- Harada & Bodek, *The Harada Method: the Spirit of Self-Reliance* (2012)
- Jethwani, Dezerv (2026)
- Robinovitz, *Score at the Top* (2025)
- Bloom, *Curiosity Chronicle*
- Newport, *Deep Questions* ep. 263 (2023)
