# Data dictionary

book.json pages[] enumerates21 captures fNNN; methods.physical_faces records36 target fNNN-R/L faces. Units preserve stable ID, side, role/exact exported Unicode text. Core bbox null; recorded source boxes/regions in source-regions.json. Non-null boxes use fixed3000x2250 source pixels; no precise glyph box inferred.

book.txt navigation `〔unit:ID〕` is editorial. TEI ab elements preserve identical strings, source surfaces and uncertainty notes, not full critical apparatus. uncertainties.json start/end are0-based half-open codepoint spans. Null spans anchor face/region issues without locating exact character. Known extent describes exported strings, not source glyph count. `[gaiji:ID]` and `⟦ID⟧` are editorial references, not printed brackets/restored characters; source-regions.json supplies mappings. Mark/space encoding/origin can remain unknown after reference representation complete. Earlier provisional strings privately preserved; b01 uses explicit gaiji export projection.

source-pages.json gives official image/canvas URLs, decoded sizes and SHA-256. Images, crops and private production materials excluded.
