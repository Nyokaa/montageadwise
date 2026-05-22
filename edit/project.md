# Project — louisinsta.mp4

## Session 1 — 2026-05-22

**Strategy:** Reel vertical Instagram (FR), talking-head de Louis sur la preuve sociale
comme facteur de différenciation. Source unique 464×832 60fps 43,6s, montée en
1080×1920 24fps. Une seule prise : on conserve la structure HOOK → HISTOIRE →
QUESTION → RAISON 1 → RAISON 2 → LEÇON. Habillage HyperFrames « coloré & dynamique »
(dégradés bleu→magenta, accent lime), sous-titres bold 2 mots MAJUSCULES.

**Decisions:**
- Coupes : suppression de la répétition/faux départ 11.80→14.70 (« Qu'est-ce qui a
  fait… » remplacé par la reprise « Pourquoi… plutôt qu'avec une autre agence »).
  Aucun silence mort à couper (prise dense) ; 3 gaps >0,4s resserrés à ~0,16s
  (après « rendez-vous », « choses », « différenciation »). Final ~38,9s.
- 5 EDL ranges, fondus audio 30ms, coupes sur frontières de mots.
- Grade : correction légère (contraste 1.06 / sat 1.06 / brightness +0.012) + scale
  forcé 1080×1920 via le champ grade.
- 5 overlays HyperFrames : badge hook +1 600 €/mois, cartes Instagram, carte
  « 1 · L'AUTHENTICITÉ », carte « 2 · LA PREUVE SOCIALE », comparatif final
  réplicable/non réplicable.
- Sous-titres : master.srt reconstruit (offsets timeline de sortie), tokens de
  ponctuation Scribe filtrés.

**Reasoning log:**
- Overlays VP9/webm : le décodeur ffmpeg par défaut ne lit pas l'alpha VP9
  (yuv420p) → fond noir. Corrigé en convertissant chaque overlay en ProRes 4444
  .mov (alpha lu nativement). EDL pointe sur les .mov.
- master.srt généré hors --build-subtitles : Scribe renvoie la ponctuation comme
  tokens « word » de durée nulle → cues parasites empilées. Filtrées sur alphanum.
- slot_5 : fenêtre overlay portée à 9,2s pour tenir le comparatif jusqu'à la fin
  (le .mov fait 8,8s, l'overlay gèle la dernière frame).

**Outstanding:** aucun. Livrable : edit/final.mp4 (1080×1920, 38,9s, -14 LUFS).

## Session 2 — 2026-05-22

**Strategy:** Refonte de la direction artistique des overlays d'après une
référence client : DA « tech-HUD » sombre — accent cyan #1ECBD8, fond navy
#0B0F14, typo Inter bold (fini Anton/dégradés/lime/magenta), cadres à coins
type viseur, chips d'étiquette cyan pleins. Correction d'un défaut de timing.

**Decisions:**
- 5 overlays restylés : cartes navy translucides, cadre cyan 2px + corner
  brackets, chips cyan à texte navy, texte blanc Inter aligné à gauche.
- Comparatif (slot 5) : côté « non réplicable » cyan, côté « réplicable »
  rouge atténué #C2453F.
- Timing : chaque overlay retardé de +0,6s (apparaissait <1s trop tôt).

**Reasoning log:**
- Timeline d'animation des overlays inchangée ; le recalage se fait
  uniquement via `start_in_output` dans l'EDL (+0,6s par overlay).

**Outstanding:** aucun. Livrable : edit/final.mp4 (1080×1920, 38,9s, -14 LUFS).
