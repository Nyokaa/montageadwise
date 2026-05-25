# Project — videomanon.mp4

## Session 1 — 2026-05-25

**Strategy:** Reel vertical 1080×1920, ~34,5s. Skit (0–7s) → Pitch + checklist
5 items (7–26s) → CTA (28–34s). Une seule coupe : resserrer le silence
inter-scènes 6,76→7,42s à ~0,4s. DA terreuse/artisanale : vert #2F3E34,
terracotta #B86A4A, blanc pierre #D9D2C7, bois #6B4A34, police Montserrat,
formes douces arrondies (pas de tech-HUD).

**Decisions:**
- Transcription via faster-whisper local (medium, FR, word timestamps) —
  ElevenLabs Scribe bloqué en free tier depuis cette IP cloud.
- 4 overlays HyperFrames : lower-third Manon (1,0–4,0s), carte « DIAGNOSTIC
  PERSONNALISÉ » (15–17s), checklist 5 items (17–26,5s), CTA « RÉSERVE TON
  CRÉNEAU » (30,3–34,3s).
- Sous-titres Montserrat, FontSize 9, casse naturelle, ~4 mots/ligne,
  position MarginV 110, outline noir.
- Frame 0 des overlays supprimée à la conversion ProRes (poster parasite).
- master.srt construit sur durées réelles des clips ; corrections Whisper
  appliquées : « angulaire » → « ongulaire », apostrophes recollées
  (« t 'es » → « t'es »), flush sur tokens de ponctuation isolés.

**Reasoning log:**
- Source `videomanon.mp4` déjà fortement éditée par l'auteur : sous-titres
  burnt-in (police différente), cartons noirs titres pour chaque item du
  diagnostic, cuts inter-scènes outdoor→indoor déjà présents. Posé au
  client → décision « Tout garder (assumé redondant) ». Mes overlays et
  mes sous-titres se superposent donc à ce qui existe déjà.
- Whisper local ~±150ms (vs ~50ms pour Scribe) — précision suffisante
  pour les coupes et la synchro des chunks de sous-titres.

**Outstanding:** aucun. Livrable : edit_manon/final.mp4 (1080×1920, 34,5s,
-14 LUFS).
