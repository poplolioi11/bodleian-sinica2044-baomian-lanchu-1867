> 本文件原有的 v0.2.0 校讀與數量敘述保留為歷史；本版 v0.2.1 的局部非盲覆核、現行數量及未解狀態見 [METHODS.md](METHODS.md) 與 [TARGETED-CORRECTIONS.md](TARGETED-CORRECTIONS.md)。

# Data dictionary

book.json pages[] enumerates21 captures fNNN; methods.physical_faces records36 target fNNN-R/L faces. Units preserve stable ID, side, role/exact exported Unicode text. Core bbox null; recorded source boxes/regions in source-regions.json. Non-null boxes use fixed 3000x2250 source pixels; no precise glyph box inferred.

book.txt navigation `〔unit:ID〕` is editorial. TEI ab elements preserve identical strings, source surfaces and uncertainty notes, not full critical apparatus. uncertainties.json start/end are0-based half-open codepoint spans. Null spans anchor face/region issues without locating exact character. Known extent describes exported strings, not source glyph count. `[gaiji:ID]` and `⟦ID⟧` are editorial references, not printed brackets/restored characters; source-regions.json supplies mappings. Mark/space encoding/origin can remain unknown after reference representation complete. Earlier provisional strings privately preserved; b01 uses explicit gaiji export projection.

source-pages.json gives official image/canvas URLs, decoded sizes and SHA-256. Images, crops and private production materials excluded.

Version 0.2.0: REVISION-CHANGES.json gives accepted literal operations with fixed original/result unit codepoint spans and source-image hashes/physical-face regions. source-regions.json retains historical v0.1.0 gaiji and declarations, including records resolved by this revision; current active uncertainty declarations are in book.json/uncertainties.json. A retained registry record is not necessarily an active unresolved token. Comparison questions with null spans are face/region-anchored, not exact glyph locations.

source_marks uses codepoint spans remapped to the current v0.2.0 strings; source_marks_preexport_history retains original pre-export source-record spans. Source geometry is unchanged. Known gaiji locator spans are likewise remapped; historical raw-source indices remain historical. Face-orientation observations retain the source-specific mirrored-title uncertainty.
