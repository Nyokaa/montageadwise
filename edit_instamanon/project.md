# Project — instamanon.mp4

## Session 1 — 2026-05-25

**Strategy:** Reel vertical 1080×1920, ~42,2s. Manifeste : HOOK (proverbe
« il faut souffrir pour être belle » réfuté) → AVANT vs AUJOURD'HUI →
3 SYMPTÔMES anormaux → CITATION (« la beauté ne devrait jamais se faire
dans la douleur ») → CTA QUESTION (« et toi, c'était NORMAL ? »). Une seule
coupe : resserrer le silence inter-actes 5,80→6,36s à ~0,35s. DA terreuse
identique à videomanon : vert #2F3E34, terracotta #B86A4A, blanc pierre
#D9D2C7, bois #6B4A34, Montserrat.

**Decisions:**
- Transcription via faster-whisper (medium, FR, word timestamps). Scribe
  toujours bloqué en free tier depuis cette IP.
- 4 overlays HyperFrames :
  1. Hook proverbe barré + tampon « ANNÉES 1800 » (0,8–5,5s)
  2. Split « AVANT · douleur banalisée » vs « AUJOURD'HUI · pas de douleur »
     (6,0–12,5s)
  3. Checklist 3 symptômes ✗ + tampon « PAS NORMAL » (13,0–22,0s)
  4. Carte citation Phase 1 → question Phase 2 + CTA commentaire (32,5–42,0s)
- Sous-titres Montserrat FontSize 10, casse naturelle, ~4 mots, MarginV 110,
  outline noir.
- Frame 0 des overlays supprimée à la conversion ProRes (poster parasite).
- master.srt construit sur durées réelles ; corrections Whisper appliquées :
  `ombre/s` → `ongle/s`, `pause/s` → `pose/s`, apostrophes recollées.

**Reasoning log:**
- Source brute (pas de subs incrustés cette fois, contrairement à
  videomanon.mp4) — overlays et subs propres, sans superposition.
- Phase 1→2 du slot 4 fait en crossfade dans la même carte (au lieu de deux
  overlays séparés) — plus fluide visuellement.

**Outstanding:** aucun. Livrable : edit_instamanon/final.mp4 (1080×1920,
42,3s, -14 LUFS).

## Session 2 — 2026-05-25

**Strategy:** Refonte des overlays en **full-screen opaque** pour couvrir
entièrement le visage du début à la fin (demande utilisateur : « qu'on ne
voit plus du tout »). Plus dynamique : slams, screen-shakes, kinetic
typography. Ajout d'un 5e slot pour la section « principe » qui n'était
pas couverte.

**Decisions:**
- 5 overlays sans transparence, couverture 100% du timing :
  1. HOOK proverbe + strike + tampon (0–5,95s) — fond pierre
  2. AVANT/AUJOURD'HUI split vertical (5,95–13,0s) — bois/pierre
  3. 3 SYMPTÔMES + tampon « PAS NORMAL » (13,0–22,0s) — fond pierre
  4. PRINCIPE kinetic typography « CONFORT / juste / BIEN »
     (22,0–32,5s) — fond vert
  5. CITATION + CTA « NORMAL ? » (32,5–42,2s) — fond vert
- Animations énergiques : back-eases, scale-slams, parallax, glow blooms,
  letter-stagger types, motion-blur strikes.
- Sous-titres Montserrat repositionnés MarginV 50 (très bas, sous les
  overlays) + box noir semi-opaque (BorderStyle 3, BackColour 80000000)
  pour rester lisibles sur les fonds clairs (slots 1/2/3).

**Reasoning log:**
- Subs à MarginV 110 entraient en collision avec le texte du slot 4
  (principe). Descendus à MarginV 50 → zone claire en bas.
- Slot 5 « NORMAL ? » à 170px de typo : le mot déborde légèrement le
  cadre 1080px — accepté en tant qu'effet d'impact.
- Aucune piste alpha nécessaire (overlays opaques) ; conversion ProRes
  conservée pour le drop frame 0 (sécurité poster-frame).

**Outstanding:** option à proposer si demandé — réduire la taille de
« NORMAL ? » dans le slot 5 pour qu'il ne déborde pas.
