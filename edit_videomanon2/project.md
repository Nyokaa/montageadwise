# Project — videomanon2.mp4

## Session 1 — 2026-05-28

**Strategy:** Vertical 1080×1920, ~73s. Multi-take cleanup d'un brut 2:37 :
HOOK (intro Manon + santé naturelle) → ESTHÉTIQUE + SANTÉ → 3 PILIERS
RESPECTÉS (plaque / habitudes / sensibilités) + punchline → DIAGNOSTIC
personnalisé → OBJECTIF (mains belles aujourd'hui + saines long terme) →
CTA (formulaire en dessous). DA terreuse Montserrat identique à
instamanon (vert/terracotta/pierre/bois).

**Decisions:**
- Source 220 MB récupérée via Google Drive (lien public temporaire),
  gitignorée au repo root car > 100 MB GitHub.
- Transcription faster-whisper local (272 mots, 99s).
- 8 ranges EDL : skip director cues (« c'est good ? ok », « il est
  arrivé », « là je vais tourner pour qu'on voit le paysage »,
  « je te dirais juste de refaire »), skip faux départs (« beaucoup
  de femmes... esthéti... », « une prestation qui va... »,
  « chaque cliente diagnostic personnalisé » version courte, premier
  CTA take 1), garde les bonnes prises.
- Tightening des pauses speaker mid-phrase : « Mon objectif, ce n
  [3s] 'est pas » → 0,3s ; « approche respectueuse, [3s] vous
  pouvez » → 0,3s.
- 6 overlays : 5 cartes transparentes compactes en haut (lower-third
  Manon, spécialité, esthétique+santé, 3 piliers checklist, diagnostic)
  + slot 6 full-page forest-green pour le CTA final.
- Sous-titres Montserrat FontSize 10, casse naturelle, ~4 mots, box
  noir semi-opaque, MarginV 110. Corrections Whisper : « angulaire »
  → « ongulaire », apostrophes recollées.
- Re-encode final libx264 slow CRF 21 pour passer sous 100 MB GitHub.

**Outstanding:** aucun. Livrable : edit_videomanon2/final.mp4
(1080×1920, 73,2s, -14 LUFS, 78 MB).
