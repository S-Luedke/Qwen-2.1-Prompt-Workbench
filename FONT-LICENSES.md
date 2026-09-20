# Fonts

The three typefaces used by `index.html` are embedded directly in the page as base64 woff2,
so the page makes **no request to Google Fonts or any other external host**. Nothing about a
visitor reaches a third party.

All three are licensed under the **SIL Open Font License, Version 1.1**, which permits
embedding and redistribution. The full licence text is in [`OFL.txt`](OFL.txt).

| Typeface | Used for | Upstream |
|---|---|---|
| Cormorant Garamond | masthead, section headings | https://github.com/google/fonts/tree/main/ofl/cormorantgaramond |
| Archivo | interface and body text | https://github.com/google/fonts/tree/main/ofl/archivo |
| JetBrains Mono | prompts and code | https://github.com/JetBrains/JetBrainsMono |

Only the latin subsets are embedded, at the weights the page actually uses: Cormorant Garamond
600, Archivo 400/500/600, JetBrains Mono 400/500. That is 187 KB of font data.

Copyright in each typeface remains with its respective authors, as stated in the upstream
repositories linked above.
