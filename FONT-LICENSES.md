# Fonts

The three typefaces used by `index.html` are embedded in the page as base64 woff2, so the page
makes **no request to Google Fonts or any other external host**. Nothing about a visitor reaches
a third party.

All three are licensed under the **SIL Open Font License, Version 1.1**, which permits embedding
and redistribution. The full licence text for each, including its copyright notice, is in
`fonts/`.

| Typeface | Used for | Copyright | Licence |
|---|---|---|---|
| Cormorant Garamond | masthead, section headings | 2015 the Cormorant Project Authors | [OFL](fonts/OFL-cormorantgaramond.txt) |
| Archivo | interface and body text | 2020 The Archivo Project Authors | [OFL](fonts/OFL-archivo.txt) |
| JetBrains Mono | prompts and code | 2020 The JetBrains Mono Project Authors | [OFL](fonts/OFL-jetbrainsmono.txt) |

None of the three declares a Reserved Font Name, so the embedded latin subsets keep their
original family names, as distributed upstream.

Only the latin subsets are embedded, at the weights the page actually uses: Cormorant Garamond
600, Archivo 400/500/600, JetBrains Mono 400/500. That is 187 KB of font data.

## Preview image

`social-preview.png` is drawn programmatically from these fonts. It contains no generated
imagery, so no model licence applies to it.
