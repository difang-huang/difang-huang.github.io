# Fonts

`NotoSerifSC-fit-400.woff2` / `NotoSerifSC-fit-500.woff2` are **subsets** of
[Noto Serif SC](https://fonts.google.com/noto/specimen/Noto+Serif+SC) (SIL Open
Font License 1.1, see `OFL.txt`), containing only the Chinese glyphs used on this
site plus common CJK punctuation.

They are referenced from `assets/css/font.css` with `size-adjust: 88%` so Chinese
characters visually match the Latin serif (Crimson Pro). Any CJK character not in
the subset falls back to the full Noto Serif SC served from Google Fonts.

To regenerate after adding new Chinese text, re-subset the full Noto Serif SC
variable font to the characters in `index.md` (weights 400 and 500) and update the
`unicode-range` in `font.css` to match the shipped glyphs.
