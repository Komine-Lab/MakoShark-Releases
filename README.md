# Mako Shark

Mako Shark is a Grasshopper 2 plug-in for Rhino 9 with tools for text outlines, Google Fonts, character sequences, and dice rolling. This repository hosts compiled beta downloads and installation instructions.

## Download and install

1. Open [Releases](../../releases) and choose a beta release.
2. Under **Assets**, download `MakoShark.rhp` and save it in a folder where you plan to keep it.
3. In Rhino 9, run `GH2Plugins`, click **Install…**, and select the downloaded file.
4. Run `GH2` to open Grasshopper 2. Look for **Mako Shark** in the component toolbar.

The beta has been tested on Windows with Rhino 9 WIP build `9.1.26314.9001`. Check the release notes for compatibility and known issues for each build.

## Components

| Component | What it does |
| --- | --- |
| **Character Sequence Neo** | Generates character labels from an inclusive, zero-based range. Supports English, Hiragana, Katakana, Iroha, and Greek, with capitalization controls for English and Greek. |
| **Dice** | Rolls 1–10 six-sided dice with an on-node button. Each die animates independently, and the results are output after all dice stop. |
| **Simple Text Outline** | Converts text into curves on a plane. Supports text height, font family, weight, bold, italic, and horizontal and vertical alignment. |
| **Google Fonts Selector (GFS)** | Filters and previews Google Fonts on the node. The Font output carries the selected family and style settings for compatible components such as Simple Text Outline. Install the font locally to generate outlines. |

To turn character labels into curves, connect the **Characters** output of Character Sequence Neo to **Text** on Simple Text Outline. Connect the **Font** output of Google Fonts Selector to **Font** on Simple Text Outline. Use **Show Optional Inputs** to reveal the Font input.

## Beta feedback

When reporting a problem, include the Mako Shark version, the Rhino build, and the steps to reproduce it. For text issues, include the font family, weight, and a screenshot of the component connections if possible.

## Acknowledgements

Thanks to [Google Fonts](https://fonts.google.com/) for the typeface catalog and preview fonts, and [The Quotations Page](https://www.quotationspage.com/) for preview quotations. Third-party fonts and quotations are subject to their respective terms.
