# FUNtasia complete-site replacement checklist

Goal: make https://funtasiaaudio.github.io/ the primary, self-contained FUNtasia website, while retiring old landing pages **only after** equivalent content and links are validated.

## Already migrated
- Unified home and major product categories
- Audio product catalog (verify completeness against old Audio before cutover)
- Records artist overview in five languages (JA, EN, DE, FR, RU)
- Records creators' rights / AI policy (Japanese and English original wording, translations in DE/FR/RU)
- Records support / Ko-fi / individual or recurring patronage inquiry
- Records collaboration and demo-submission invitation (Japanese and English original wording, translations in DE/FR/RU)
- Studio and expansion-pack microsite links
- FUNtasia Mixer official release-list link

## Still required before old-sites replacement
1. **Audio content inventory:** compare all old `funtasia-audio` sections, products, current version/download links, manuals, screenshots, wallpapers, cursors, Studio pages, and expansion pages with their destination pages. Preserve accurate release claims.
2. **Records content inventory:** confirm all original art, collaborators, music releases, support/contact/legal statements and translations are represented accurately. The original Records site has JA, EN, KO, and Traditional Chinese language behavior; add or intentionally route KO and zh-TW before retiring its original homepage. New DE/FR/RU translations need human review.
3. **Asset independence:** copy owned website images/CSS/JS/download references where appropriate and verify they resolve, rather than relying indefinitely on hotlinked old-site files.
4. **URL mapping:** prepare 1:1 redirects or stable passthrough routes for deep links, especially Studio and expansion landing pages, manuals, and any download/archive links. A root-only JavaScript redirect must not break older deep links.
5. **QA and discoverability:** check desktop/mobile, all language navigation, external URLs, live ZIP links, accessibility, metadata, sitemap, canonical links, and search indexing. Verify actual deployment after each change.
6. **Cutover approval:** keep the two original repositories unchanged until an explicit follow-up approval to modify each. Back up/tag their last known-good revisions. Deploy safe redirect changes and test; retain old assets/deep links or permanent equivalents until migrated.
7. **Rollback:** restore the original landing pages if redirect or content checks fail. Never delete existing downloads or repository files as part of cutover.

## Decision
The destination is the unified GitHub Pages user site `funtasiaaudio/funtasiaaudio.github.io`.
The original sites remain protected during migration:
- Audio: `funtasiaaudio/funtasia-audio`
- Records: `infofuntasiarecords-tech/funtasia-records`

Created 2026-11-05. Completion of HTML section updates alone does **not** mean the entire legacy sites can safely be redirected or removed.
