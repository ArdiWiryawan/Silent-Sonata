# Silent Sonata — Full Game Execution Documentation v2.0



---

<!-- SOURCE: README_DOWNLOAD_INDEX.md -->

# Silent Sonata — Full Game Execution Documentation Package v2.0

## Status
**Full Game Production & Execution Candidate**

Paket ini dibuat setelah MVP *The Coma Room* dinyatakan berjalan dengan baik. Fokus baru adalah mengunci desain full game dari awal sampai akhir, termasuk fase latihan baru:

> Pemain memulihkan **3 nada inti** melalui **5 fragmen latihan**.

## Isi Paket

1. `01_Silent_Sonata_Full_Game_Production_Document_v2.0.md`  
   Dokumen master lengkap dari visi sampai eksekusi.

2. `02_Story_and_Narrative_Bible_v2.0.md`  
   Cerita lengkap, karakter, chapter, memory fragments, ending.

3. `03_Gameplay_and_Systems_Bible_v2.0.md`  
   Core loop, training 3 notes/5 fragments, mechanics, progression, fail/reward.

4. `04_Level_Design_and_Encounter_Bible_v2.0.md`  
   Struktur level dari Prologue sampai Finale, encounter template, 21 playable sequences.

5. `05_Music_and_Audio_Bible_v2.0.md`  
   Final Sonata, motif, 3-ball identity, wrong/correct feedback, adaptive audio.

6. `06_Art_and_Asset_Bible_v2.0.md`  
   Asset 3D, visual language, chapter environment, VFX, UI asset, asset manifest.

7. `07_Technical_Design_and_Implementation_Plan_v2.0.md`  
   Architecture, folder structure, managers, data schema, sprint implementation.

8. `08_UX_Accessibility_Sensitivity_QA_Plan_v2.0.md`  
   UX flow, accessibility, sensitivity, QA, playtest, acceptance gates.

9. `09_Production_Roadmap_Backlog_and_AI_Agent_Prompts_v2.0.md`  
   Roadmap produksi, backlog task, AI agent prompts, definition of done.

10. `Silent_Sonata_Full_Game_Execution_Documentation_v2.0.md`  
   Semua dokumen digabung menjadi satu file Markdown.

11. `data/full_game_asset_manifest_v2.0.json`  
   Asset manifest siap dipakai untuk produksi.

12. `data/level_sequence_manifest_v2.0.json`  
   Struktur chapter/level dalam format data.

## Next Step
Gunakan paket ini sebagai dasar **Phase 12 — Full Game Vertical Slice Planning & Execution**.


---

<!-- SOURCE: docs/01_Silent_Sonata_Full_Game_Production_Document_v2.0.md -->

# Silent Sonata — Full Game Production Document v2.0

## 0. Document Control
- Version: v2.0
- Date: 2026-05-14
- Status: Full Game Production & Execution Candidate
- Owner: Ardi Wiryawan / Silent Sonata Production
- Previous Foundation: v1.4 complete documentation and v1.7 sound/gameplay revision
- Current Major Update: Prologue training phase where player restores 3 notes with 5 fragments

---

# 1. Executive Summary

Silent Sonata is a minimalist fantasy psychological rhythm-reaction game for web browser. The player helps a comatose pianist rebuild the Final Sonata by learning to trust music over deceptive visuals.

The MVP has proven the core direction. The full game now starts with a stronger early training phase:

> The player restores **3 core notes** through **5 training fragments**.

These three notes become the musical alphabet of the entire game:
- Low / Blue Orb / Grounding
- Mid / Rose Crystal / Heart
- High / Gold Prism / Hope

---

# 2. Production Lock

## Core Promise
> Music tells the truth. Vision lies.

## Gameplay Promise
> Music shows the answer first. Vision lies later.

## Full Game Opening Promise
> Restore three notes. Learn to hear the world. Rebuild the Final Sonata.

---

# 3. Story & Narrative Bible


# Silent Sonata — Story & Narrative Bible v2.0

## 0. Document Control
- Version: v2.0
- Date: 2026-05-14
- Status: Full Game Narrative Candidate
- Scope: Complete story from opening to ending
- Core Narrative Rule: Story is revealed through sound, memory, object interaction, and recovery, not exposition-heavy dialogue.

---

# 1. Logline

A comatose pianist trapped in a surreal inner world must recover three lost notes, rebuild a broken sonata, and learn to trust music over deceptive visions before the final memory fades.

---

# 2. High Concept

Silent Sonata bercerita tentang seorang pianis muda yang mengalami kecelakaan setelah konser besar. Ia tidak sadar di dunia nyata, tetapi di dalam pikirannya ia berada di ruang fantasi yang dibentuk dari musik, memori, rasa bersalah, tekanan performa, dan keinginan untuk pulang.

Visual di dunia itu sering menipu. Cahaya bisa menjadi memori palsu. Applause bisa menjadi tekanan. Cermin bisa menjadi kritik diri. Headlight bisa menjadi panik. Satu-satunya hal yang masih konsisten adalah musik: piano, heartbeat, silence, echo, resonance, dan fragmen melodi.

---

# 3. Final Story Premise

## Dunia Nyata
Pianis utama baru menyelesaikan konser terpenting dalam hidupnya. Dalam perjalanan pulang, ia mengalami kecelakaan. Ia masuk koma. Orang-orang terdekatnya menunggu di ruang rumah sakit.

## Dunia Koma
Di dalam pikirannya, semua memori berubah menjadi ruang fantasi musikal. Piano rusak menjadi pusat dunia. Ia hanya bisa pulang jika Final Sonata tersusun kembali.

## Player Role
Pemain bukan “tubuh” karakter. Pemain adalah **inner listener**—bagian dari kesadaran pianis yang masih bisa membedakan musik yang benar dari visual yang menipu.

---

# 4. Main Character

## Working Name
**Liora**  
Nama ini bisa diganti, tetapi untuk production candidate dipakai sebagai placeholder final.

## Identity
- Pianis muda.
- Perfeksionis.
- Sensitif terhadap suara.
- Merasa dicintai karena performa, bukan karena dirinya.
- Terjebak antara keinginan menjadi sempurna dan keinginan untuk bebas bermain musik.

## Wound
Liora percaya bahwa jika ia gagal bermain sempurna, ia mengecewakan semua orang.

## Need
Ia harus belajar bahwa musik bukan bukti kesempurnaan, melainkan jalan pulang menuju diri sendiri.

## Arc
Perfeksionisme → Keraguan → Tekanan → Trauma → Penerimaan → Pulang.

---

# 5. Supporting Characters

## 5.1 The Mother / Family Voice
- Tidak banyak muncul secara visual.
- Hadir sebagai suara hangat, napas, atau motif sederhana.
- Melambangkan unconditional love.

## 5.2 The Mentor
- Guru piano lama Liora.
- Muncul sebagai memori lembut.
- Kalimat kunci: “Jangan mainkan nada yang benar saja. Mainkan nada yang jujur.”

## 5.3 The Audience
- Bisa menjadi dukungan atau tekanan.
- Dalam Chapter 3, applause menjadi ilusi yang harus diuji.

## 5.4 The Inner Critic
- Bukan villain literal.
- Muncul sebagai echo yang detuned, mirror reflection, dan false cue.
- Melambangkan standar sempurna yang menyakiti Liora.

---

# 6. Narrative Structure Overview

| Act | Chapter | Narrative Function | Emotional Question |
|---|---|---|---|
| Prologue | The First Three Notes | Liora belajar kembali mendengar | “Apa suara pertamaku?” |
| Act I | The Silent Room | Ia memahami aturan dunia koma | “Bisakah aku percaya musik?” |
| Act II | The Hall of False Notes | Ia menghadapi kritik diri | “Apakah semua kesalahan adalah kegagalan?” |
| Act III | The Broken Concert | Ia menghadapi tekanan publik | “Apakah aku masih bernilai tanpa tepuk tangan?” |
| Act IV | The Accident Memory | Ia menghadapi trauma kecelakaan | “Bisakah aku menerima yang terjadi?” |
| Act V | The Last Sonata | Ia menyusun pulang | “Bisakah aku memainkan lagu yang jujur?” |
| Epilogue | Awakening | Dunia nyata kembali | “Apakah aku siap hidup lagi?” |

---

# 7. Prologue — The First Three Notes

## Purpose
Fase latihan awal sekaligus pembuka cerita. Pemain memulihkan **3 nada inti** dengan mengumpulkan **5 fragmen**.

## Three Core Notes

| Note | Object | Meaning | Story Function |
|---|---|---|---|
| Low Note | Blue Orb | Grounding / breath | Liora masih hidup |
| Middle Note | Rose Crystal | Heart / memory | Liora masih punya rasa |
| High Note | Gold Prism | Hope / awakening | Liora masih bisa pulang |

## Five Training Fragments

| Fragment | Name | Gameplay | Narrative Reveal | Restored Result |
|---|---|---|---|---|
| Fragment 1 | Breath of Blue | Klik Blue Orb setelah low cue | Detak jantung masih ada | Low Note unlocked |
| Fragment 2 | Rose in Silence | Klik Rose setelah mid cue | Ada seseorang menunggu | Middle Note seed |
| Fragment 3 | Gold Through the Dark | Klik Gold setelah high cue | Ada cahaya di ujung memori | High Note seed |
| Fragment 4 | The Three Voices | Cocokkan low/mid/high acak | Ketiga suara menjadi peta | Middle + High stabilized |
| Fragment 5 | First Phrase | Mainkan pola Low → Mid → High | Piano mulai mengingat | Three-note motif restored |

## Narrative Beat
Setelah Fragment 5, piano rusak memainkan phrase pertama Final Sonata. Ruangan tidak lagi sepenuhnya gelap. Ini adalah momen pertama bahwa Liora mungkin bisa bangun.

---

# 8. Chapter 1 — The Silent Room

## Emotional Theme
Confusion, curiosity, fragile hope.

## Story
Liora berada di ruangan sunyi yang tidak ia kenali, tetapi ada piano rusak di tengah ruangan. Tiga cahaya muncul sebagai suara pertama dunia ini. Pemain belajar bahwa suara memandu, visual bisa menipu.

## Memory Reveal
Concert hall appears as a blurred image. Liora remembers being on stage, but not what happened after.

## Key Memory Fragments
1. Piano room at home.
2. First recital photo.
3. Final concert ticket.
4. Blurred audience.
5. Broken sheet music.

## Ending Beat
Pintu menuju Hall of False Notes terbuka ketika pemain dapat membedakan truth cue dan false visual cue.

---

# 9. Chapter 2 — The Hall of False Notes

## Emotional Theme
Self-doubt and perfectionism.

## Story
Liora memasuki koridor cermin. Setiap cermin memainkan kembali nada yang pernah ia mainkan salah. Inner Critic membuat echo palsu agar Liora percaya bahwa satu kesalahan menghancurkan semuanya.

## Gameplay-Narrative Link
Echo Memory mechanic: pemain mendengar motif asli, lalu echo corrupt, dan memperbaiki nada yang salah.

## Memory Reveal
Liora ingat latihan keras, kompetisi, dan perkataan orang-orang yang ia tafsirkan sebagai tuntutan.

## Ending Beat
Mentor memory appears and says through piano, “A wrong note can still lead home.”

---

# 10. Chapter 3 — The Broken Concert

## Emotional Theme
Performance anxiety, public judgment, exposure.

## Story
Dunia berubah menjadi concert hall yang retak. Audience muncul sebagai cahaya tanpa wajah. Applause kadang menjadi dukungan, kadang menjadi pressure. Liora harus membedakan applause asli dan false applause.

## Gameplay-Narrative Link
Call-and-Response mechanic: pemain menjawab motif, lalu menilai apakah dunia membalas dengan benar.

## Memory Reveal
Final concert was not a failure. Liora played beautifully, but she could not feel it because she was trapped in fear.

## Ending Beat
Concert hall collapses into road-light fragments. The accident memory begins to leak into the world.

---

# 11. Chapter 4 — The Accident Memory

## Emotional Theme
Fear, shock, acceptance.

## Story
Dunia menjadi jalan abstrak yang terbuat dari headlight, garis heartbeat, pecahan kaca simbolik, dan silence. Tidak ada gore. Tidak ada crash realistis. Semua digambarkan sebagai memori tubuh yang sulit dipahami.

## Gameplay-Narrative Link
Heartbeat Recovery mechanic: pemain menahan dan melepas input untuk menstabilkan detak jantung.

## Memory Reveal
Liora bukan gagal. Kecelakaan terjadi. Ia tidak perlu menghukum dirinya untuk sesuatu yang tidak bisa ia kendalikan.

## Sensitivity Lock
Scene ini wajib memiliki:
- content warning,
- reduced intensity setting,
- skip with summary option,
- no realistic gore,
- no alarm-like harsh sound,
- no shock jumpscare.

## Ending Beat
Heartbeat stabil. Liora menerima bahwa pulang bukan berarti menghapus trauma, tetapi membawa dirinya kembali.

---

# 12. Chapter 5 — The Last Sonata

## Emotional Theme
Closure, integration, awakening.

## Story
Semua ruang menyatu menjadi panggung putih-keemasan. Piano yang rusak mulai utuh. Pemain memainkan Final Sonata dengan motif dari seluruh game: low grounding, mid heart, high hope, silence, echo, heartbeat, applause, and acceptance.

## Gameplay-Narrative Link
Build the Final Song: semua mechanics kembali, tetapi dalam bentuk lebih elegan dan tidak terlalu menghukum.

## Final Memory Reveal
Orang-orang terdekat Liora berada di rumah sakit. Suara mereka bukan tekanan, tetapi panggilan pulang.

---

# 13. Endings

## 13.1 Clear Awakening
Condition:
- High fragment completion.
- Low or moderate corruption.
- Final Sonata mostly complete.

Ending:
Liora bangun. Ia tidak langsung berbicara. Ia mendengar suara piano phrase terakhir, lalu menggenggam tangan orang terdekat.

## 13.2 Soft Awakening
Condition:
- Enough fragments.
- Some corruption unresolved.

Ending:
Liora bangun perlahan. Beberapa memori masih kabur. Musik terdengar tidak sempurna, tetapi hangat.

## 13.3 Dreaming Coda
Condition:
- Low fragment completion.
- High corruption.

Ending:
Liora belum sepenuhnya bangun, tetapi Final Sonata tidak hilang. Player melihat satu note tetap menyala, menandakan harapan dan retry path.

## Design Rule
No ending should feel cruel. Even incomplete endings must preserve dignity and hope.

---

# 14. Narrative Asset List

## Memory Images / Symbols
- Broken sheet music.
- Concert ticket.
- Old metronome.
- Cracked mirror.
- Mentor’s red pencil.
- Empty audience seat.
- Stage spotlight.
- Road-light streak.
- Hospital curtain silhouette.
- Family hand silhouette.

## Narrative Audio
- Mother/family hum motif.
- Mentor motif.
- Audience motif.
- Inner critic detuned echo.
- Hospital room distant ambience.
- Final Sonata phrase.

---

# 15. Narrative Approval Checklist

- [ ] Story is understandable without heavy exposition.
- [ ] Coma is symbolic, not medically overclaimed.
- [ ] Trauma is handled without shock exploitation.
- [ ] Main character has agency and dignity.
- [ ] Each chapter reveals a meaningful memory.
- [ ] Final ending feels earned.


---

# 4. Gameplay & Systems Bible


# Silent Sonata — Gameplay & Systems Bible v2.0

## 0. Document Control
- Version: v2.0
- Date: 2026-05-14
- Status: Full Game Systems Candidate
- Scope: All gameplay systems from tutorial to finale

---

# 1. Gameplay North Star

Silent Sonata is about listening before reacting.

> The player does not win by seeing faster.  
> The player wins by hearing what is true.

---

# 2. Final Core Loop

## Moment-to-Moment Loop
**Listen → Identify → Wait → React → Learn**

## Emotional Loop
**Confusion → Trust → Doubt → Recovery**

## Full Game Loop
**Recover Fragment → Restore Motif → Unlock Memory → Change World → Advance Chapter**

---

# 3. Prologue Training System — 3 Notes / 5 Fragments

## Goal
The early training phase teaches the entire language of the game before real challenge begins.

## Player Objective
Recover 5 fragments to restore 3 notes:
1. Low Note
2. Middle Note
3. High Note

## Why 5 Fragments for 3 Notes?
Because the player should not only unlock the notes, but understand them.

| Fragment | Teaches | Restores |
|---|---|---|
| Fragment 1 | Left/Low identity | Low Note |
| Fragment 2 | Center/Mid identity | Middle Note seed |
| Fragment 3 | Right/High identity | High Note seed |
| Fragment 4 | Sound direction + matching | Stabilizes Mid + High |
| Fragment 5 | Low → Mid → High phrase | Completes the Three-Note Motif |

## Training Completion Reward
- The piano plays the first complete phrase.
- Fragment counter becomes “5/5”.
- Three-note motif becomes the player’s first permanent musical memory.
- The Silent Room opens into the full Chapter 1 challenge.

---

# 4. Object Identity System

| Object | Name | Sound | Visual | Gameplay Role |
|---|---|---|---|---|
| Left | Blue Orb | Low warm voice | Slow wide ring | Grounding |
| Center | Rose Crystal | Mid bell-piano | Double ring | Heart / balance |
| Right | Gold Prism | High glass chime | Sharp shimmer ring | Hope / light |

## Identity Rule
The player must be able to identify each object through:
- position,
- sound pitch,
- timbre,
- stereo or visual direction,
- ring pattern,
- tutorial label.

---

# 5. Reaction Timing System

## State Flow
1. LISTEN
2. GET READY
3. CLICK NOW
4. RESULT

## Timing Windows
| Mode | Window |
|---|---|
| Tutorial | 1.8s |
| Practice | 1.5s |
| Standard | 1.15s |
| Challenge | 0.9s |
| Assist | +0.4s to +0.7s |

## Rule
No hard punishment until the player has completed the 5-fragment training phase.

---

# 6. Fragment System

## Fragment Types

| Fragment Type | Source | Function |
|---|---|---|
| Note Fragment | Object matching | Adds melody |
| Silence Fragment | No-input challenge | Adds rests |
| Echo Fragment | Echo correction | Adds harmony |
| Pulse Fragment | Heartbeat recovery | Adds rhythm |
| Memory Fragment | Major encounter | Adds narrative clarity |

## Fragment States
- Hidden
- Heard
- Recovered
- Stabilized
- Integrated into Final Sonata

---

# 7. Corruption & Recovery System

## Corruption Sources
- Wrong object.
- Too early.
- Too late.
- Clicking during silence.
- Following a decoy.
- Failing heartbeat hold.
- Accepting false echo.

## Recovery Sources
- Correct object.
- Waiting through silence.
- Correct echo repair.
- Stable heartbeat.
- Completing a memory fragment.
- Playing a motif phrase correctly.

## Corruption Levels
| Level | Audio | Visual | Gameplay |
|---|---|---|---|
| 0–1 | Clean piano | calm blue | wide timing |
| 2–3 | light detune | tiny cracks | normal |
| 4–5 | echo noise | distortion | decoys increase |
| 6–7 | heartbeat unstable | stronger cracks | recovery needed |
| 8 | soft fail | scene dims | retry phrase |

## Soft Fail Rule
No hard game over. The world gives a recovery phrase or returns to the last stable fragment.

---

# 8. Wrong Feedback System

Wrong feedback is a teacher, not a punishment.

| Mistake | Sound | Text | Visual |
|---|---|---|---|
| Too early | soft closed key | “Tunggu CLICK NOW.” | progress pulse resets |
| Too late | fading echo | “Ring sudah menutup.” | truth ring fades |
| Wrong object | muted piano + paper flutter | “Itu visual palsu.” | correct object hint pulse |
| Silence mistake | room hush | “Diam berarti jangan klik.” | room dims gently |

---

# 9. Correct Feedback System

Correct feedback must feel like healing.

## Correct Reward Stack
1. Warm piano chord.
2. Memory chime.
3. Fragment flies to piano.
4. Piano key glows.
5. Heartbeat stabilizes.
6. Scene warms slightly.
7. Final Sonata gains one layer.

---

# 10. Mechanics

## 10.1 True Note / False Note
Choose the object that sings with the final note.

## 10.2 Silence Means Truth
Do not click when silence is the truth.

## 10.3 Echo Memory
Compare original motif and echo; repair the wrong note.

## 10.4 Call-and-Response
Repeat or judge rhythmic phrase.

## 10.5 Heartbeat Recovery
Hold/release to stabilize heartbeat.

## 10.6 Memory Weaving
Place recovered fragments into the Final Sonata timeline.

## 10.7 Final Sonata Performance
Use all learned mechanics in a final musical sequence.

---

# 11. Difficulty Progression

| Phase | Player Skill |
|---|---|
| Prologue | Identify three voices |
| Chapter 1 | Trust clean truth |
| Chapter 2 | Detect altered truth |
| Chapter 3 | Respond under pressure |
| Chapter 4 | Stay calm under panic |
| Chapter 5 | Integrate all truth |

---

# 12. Accessibility-First Gameplay Rules

- No color-only critical cue.
- Audio cue always has visual support.
- Wrong SFX can be reduced.
- Reaction Assist available.
- Replay cue available.
- Visual Timing Ring available.
- Mono Friendly Mode available.
- Content warning before Accident Memory.


---

# 5. Level Design & Encounter Bible


# Silent Sonata — Level Design & Encounter Bible v2.0

## 0. Document Control
- Version: v2.0
- Date: 2026-05-14
- Status: Full Level Design Candidate
- Structure: Prologue + 5 Chapters + Epilogue
- Playable Sequences: 21 main sequences + optional memory rooms

---

# 1. Level Design Philosophy

Every level must do four things:
1. teach or test one musical truth,
2. reveal one emotional layer,
3. change the world visually or musically,
4. move the player closer to Final Sonata.

No filler levels.

---

# 2. Full Game Level Structure

| Sequence | Name | Chapter | Main Mechanic | Narrative Reward |
|---:|---|---|---|---|
| 0 | The First Three Notes | Prologue | Sound Map / 5 Fragments | 3-note motif |
| 1 | The First Light | Silent Room | True Note | First room memory |
| 2 | The Quiet Between | Silent Room | Silence | restraint memory |
| 3 | The Beautiful Lie | Silent Room | Soft Decoy | false visual rule |
| 4 | The Door of Sound | Silent Room | Major Encounter | Chapter 1 memory |
| 5 | Clean Echo | Hall | Echo Memory intro | original motif |
| 6 | Wrong Reflection | Hall | False Echo | self-doubt memory |
| 7 | Mirror Corridor | Hall | Echo + Decoy | mentor memory |
| 8 | The Note That Wasn't Failure | Hall | Major Encounter | acceptance of wrong note |
| 9 | Stage Breath | Concert | Call-and-Response intro | backstage memory |
| 10 | False Applause | Concert | Applause judgment | audience pressure |
| 11 | Spotlight Tremor | Concert | tempo pressure | final concert memory |
| 12 | The Broken Crescendo | Concert | Major Encounter | concert truth |
| 13 | Pulse Line | Accident | Heartbeat intro | leaving hall |
| 14 | Headlight Silence | Accident | Silence + panic visual | pre-crash memory |
| 15 | Impact Pause | Accident | heartbeat recovery | accident acceptance |
| 16 | The Breath After | Accident | Major Encounter | trauma integration |
| 17 | Returning Motif | Last Sonata | all mechanics light | loved voice |
| 18 | Harmony in Doubt | Last Sonata | all mechanics medium | full memory weave |
| 19 | The False Door | Last Sonata | final decoy | reject false comfort |
| 20 | Final Awakening | Last Sonata | Final Sonata | ending |
| 21 | Coda | Epilogue | reflection | awakening state |

---

# 3. Prologue Detail — The First Three Notes

## Objective
Recover 3 notes using 5 fragments.

## Micro-Sequence

### Fragment 1 — Breath of Blue
- Object: Blue Orb.
- Sound: low warm tone.
- Task: click when Blue sings.
- Reward: Low Note restored.

### Fragment 2 — Rose in Silence
- Object: Rose Crystal.
- Sound: mid celesta.
- Task: click Rose after mid cue.
- Reward: Middle Note seed restored.

### Fragment 3 — Gold Through the Dark
- Object: Gold Prism.
- Sound: high glass chime.
- Task: click Gold after high cue.
- Reward: High Note seed restored.

### Fragment 4 — The Three Voices
- Objects: all three.
- Task: identify random sound source.
- Reward: sound map stabilized.

### Fragment 5 — First Phrase
- Pattern: Low → Mid → High.
- Task: click 3-note phrase in order.
- Reward: first phrase of Final Sonata.

## Completion Moment
Piano plays Low → Mid → High. The broken keybed glows. The UI changes from “Training” to “Chapter 1”.

---

# 4. Chapter 1 — The Silent Room

## Level 1: The First Light
Teaches true note with low stakes.

## Level 2: The Quiet Between
Introduces silence. Correct action can be no action.

## Level 3: The Beautiful Lie
Introduces fair visual decoy.

## Major Encounter: The Door of Sound
Combines three voices, truth ring, and one silence sequence. Unlocks Hall of False Notes.

---

# 5. Chapter 2 — The Hall of False Notes

## Level 5: Clean Echo
Original motif plays, then clean echo. Player learns echo vocabulary.

## Level 6: Wrong Reflection
One echo note is wrong. Player chooses the wrong moment to repair it.

## Level 7: Mirror Corridor
Visual mirrors multiply. Audio remains source of truth.

## Major Encounter: The Note That Wasn't Failure
Player must repair a longer motif while Inner Critic tries to make every note feel wrong.

---

# 6. Chapter 3 — The Broken Concert

## Level 9: Stage Breath
Player repeats simple rhythmic call.

## Level 10: False Applause
Player judges if audience response is true support or pressure illusion.

## Level 11: Spotlight Tremor
Tempo shifts subtly; player uses breathing cues.

## Major Encounter: The Broken Crescendo
Player performs under visual collapse while following clean audio.

---

# 7. Chapter 4 — The Accident Memory

## Level 13: Pulse Line
Heartbeat tutorial. Hold/release gently.

## Level 14: Headlight Silence
Visual panic appears, but silence means no input.

## Level 15: Impact Pause
Heartbeat falters. Player stabilizes without harsh alarm sounds.

## Major Encounter: The Breath After
Player accepts the accident memory through a calm recovery sequence.

---

# 8. Chapter 5 — The Last Sonata

## Level 17: Returning Motif
All three notes return.

## Level 18: Harmony in Doubt
Echo, silence, and call-response combine.

## Level 19: The False Door
A beautiful visual exit appears but is not musically true.

## Major Encounter: Final Awakening
The player performs Final Sonata and triggers ending logic.

---

# 9. Encounter Template

1. Establish emotion.
2. Play clean motif.
3. Introduce mechanic.
4. Let player practice without harsh penalty.
5. Add fair deception.
6. Reward with fragment.
7. Show memory.
8. Change world.

---

# 10. Level Acceptance Checklist

- [ ] Level teaches one clear thing.
- [ ] Audio cue is readable.
- [ ] Visual deception is fair.
- [ ] Wrong feedback is soft.
- [ ] Correct feedback is satisfying.
- [ ] Memory reward is meaningful.
- [ ] Accessibility settings work.


---

# 6. Music & Audio Bible


# Silent Sonata — Music & Audio Bible v2.0

## 0. Document Control
- Version: v2.0
- Date: 2026-05-14
- Status: Full Music & Audio Candidate

---

# 1. Music Philosophy

Music is not background. Music is truth, map, feedback, memory, and story.

---

# 2. Final Sonata Structure

| Movement | Chapter | Musical Function | Emotional Function |
|---|---|---|---|
| I. Three Notes | Prologue | Low/Mid/High motif | learning to hear |
| II. Silent Theme | Silent Room | rests and space | trust |
| III. Echo Theme | Hall | call/echo harmony | self-doubt |
| IV. Concert Theme | Broken Concert | response rhythm | pressure |
| V. Pulse Theme | Accident | heartbeat rhythm | trauma |
| VI. Awakening Theme | Last Sonata | all motifs integrated | return |

---

# 3. Three Core Notes

| Note | Object | Pitch Area | Timbre | Meaning |
|---|---|---|---|---|
| Low | Blue Orb | C3/D3 | warm felt piano | breath / grounding |
| Mid | Rose Crystal | E4/F4 | celesta / bell-piano | heart / balance |
| High | Gold Prism | G5/A5 | glass chime | hope / awakening |

---

# 4. Motif Library

## Truth Motif
Low → Mid → High.

## Silence Motif
A rest that means “do not act.”

## Echo Motif
Original phrase followed by slightly altered phrase.

## Heartbeat Motif
Pulse rhythm that can stabilize or falter.

## Recovery Motif
Warm consonant chord with memory chime.

## Corruption Motif
Soft detune and unstable echo; never painful.

## Final Sonata Motif
All core motifs layered into one playable phrase.

---

# 5. Wrong Feedback Audio

Wrong feedback is soft correction.

## Sound Palette
- Muted piano thud.
- Sheet music flutter.
- Soft reverse note.
- Low heartbeat dip.
- Gentle detune only in challenge.

## Mixing Rule
Wrong feedback must be quieter than motif and shorter than correct feedback.

---

# 6. Correct Feedback Audio

Correct feedback is healing.

## Sound Palette
- Warm piano chord.
- Memory chime.
- Room breath.
- Stabilized heartbeat.
- Piano resonance.

---

# 7. Adaptive Audio States

| State | Audio |
|---|---|
| Calm | clear piano, low ambience |
| Doubt | light echo |
| Panic | heartbeat increases, but not harsh |
| Recovery | warm chord |
| Corruption | soft detune |
| Awakening | full harmony |

---

# 8. Technical Audio Requirements

- Use Web Audio API.
- Use audio clock timing.
- Use StereoPannerNode for object panning.
- Use GainNodes for separate buses.
- Use optional PannerNode later for 3D scene depth.
- Separate sliders: music, SFX, ambience, wrong SFX, accessibility cues.

---

# 9. Audio Asset List

## MVP
- heartbeat_loop_soft
- motif_three_notes_low_mid_high
- blue_orb_low
- rose_crystal_mid
- gold_prism_high
- correct_warm_chord
- wrong_soft_muted
- sheet_flutter
- silence_hush

## Full Game
- echo_clean
- echo_corrupt
- audience_true
- audience_false
- stage_pressure_rhythm
- accident_heartbeat_unstable
- accident_recovery_pulse
- final_sonata_layer_1_low
- final_sonata_layer_2_mid
- final_sonata_layer_3_high
- final_sonata_full


---

# 7. Art & Asset Bible


# Silent Sonata — Art & Asset Bible v2.0

## 0. Document Control
- Version: v2.0
- Date: 2026-05-14
- Status: Full Art & Asset Candidate

---

# 1. Visual North Star

Silent Sonata should look like music becoming light inside a dream.

---

# 2. Visual Pillars

1. Piano as sacred object.
2. Light as memory.
3. Space as emotion.
4. Minimal but premium.
5. Readability before beauty.
6. Deception must be elegant, not noisy.
7. Trauma must be symbolic, not graphic.

---

# 3. Global Asset Categories

## Characters
- Liora silhouette / memory form.
- Mother/family silhouette.
- Mentor silhouette.
- Audience light silhouettes.
- Inner Critic mirror shadow.

## Core Props
- Broken grand piano.
- Restored grand piano.
- Piano bench.
- Sheet music fragments.
- Old metronome.
- Concert ticket.
- Mentor pencil.
- Broken mirror shard.
- Hospital curtain silhouette.

## Interactive Objects
- Blue Orb.
- Rose Crystal.
- Gold Prism.
- Truth ring.
- Decoy ring.
- Sound wave line.
- Memory fragment object.

## Environments
- Coma Room.
- Silent Room.
- Hall of False Notes.
- Broken Concert.
- Accident Memory Road.
- Last Sonata Stage.
- Epilogue hospital light.

---

# 4. Prologue Asset Set

## Required
- Broken piano with 3 inactive keys.
- Blue Orb with wide ring.
- Rose Crystal with double ring.
- Gold Prism with shimmer ring.
- 5 floating fragments.
- First phrase staff line.
- UI labels LOW / MID / HIGH.

---

# 5. Chapter Environment Direction

## Chapter 1 — Silent Room
Dark blue, empty, piano-centered, fragile lights.

## Chapter 2 — Hall of False Notes
Mirrors, long hallway, reflected pianos, purple-silver palette.

## Chapter 3 — Broken Concert
Cracked stage, floating seats, spotlight, gold-red palette.

## Chapter 4 — Accident Memory
Abstract road lines, floating glass symbols, heartbeat line, no gore.

## Chapter 5 — Last Sonata
White-gold stage, restored piano, memory particles, warm atmosphere.

---

# 6. VFX List

## Truth VFX
- clean ring,
- sound wave pulse,
- small note icon,
- gentle particle lift.

## Recovery VFX
- sheet music flies into piano,
- piano key glow,
- room warms,
- heartbeat stabilizes.

## Corruption VFX
- elegant cracks,
- soft purple distortion,
- slight bloom shift,
- no horror flashes.

---

# 7. UI Asset Direction

UI should combine sheet music and heartbeat monitor.

## UI Elements
- phase label,
- timing ring,
- fragment counter,
- corruption meter,
- sound map icons,
- replay cue,
- accessibility settings,
- chapter transition card.

---

# 8. Asset Manifest Summary

A detailed JSON manifest is included in `data/full_game_asset_manifest_v2.0.json`.


---

# 8. Technical Design & Implementation Plan


# Silent Sonata — Technical Design & Implementation Plan v2.0

## 0. Document Control
- Version: v2.0
- Date: 2026-05-14
- Status: Full Technical Candidate
- Platform: Web browser
- Stack: HTML, CSS, JavaScript, Three.js, Web Audio API

---

# 1. Architecture Goals

1. Stable browser performance.
2. Audio-first timing.
3. Modular scene system.
4. Data-driven levels.
5. Accessibility built in.
6. Easy for AI coding agents to implement.

---

# 2. Folder Structure

```txt
silent-sonata/
  index.html
  package.json
  src/
    main.js
    core/
      Game.js
      StateMachine.js
      EventBus.js
    systems/
      AudioManager.js
      RhythmManager.js
      SceneManager.js
      InputManager.js
      UIManager.js
      AccessibilityManager.js
      CorruptionManager.js
      FragmentManager.js
      SaveManager.js
      QAStatsManager.js
    scenes/
      PrologueScene.js
      SilentRoomScene.js
      HallOfFalseNotesScene.js
      BrokenConcertScene.js
      AccidentMemoryScene.js
      LastSonataScene.js
      EpilogueScene.js
    assets/
      models/
      textures/
      audio/
    data/
      levels.json
      motifs.json
      assets.json
      dialogue.json
```

---

# 3. Core Managers

| Manager | Responsibility |
|---|---|
| Game | boot, loop, global lifecycle |
| StateMachine | LISTEN/READY/CLICK/RESULT |
| AudioManager | Web Audio routing |
| RhythmManager | timing windows |
| SceneManager | load/unload chapters |
| InputManager | click/hold/tap input |
| FragmentManager | 5 fragments, notes, memories |
| CorruptionManager | corruption/recovery |
| AccessibilityManager | settings |
| UIManager | HUD/tutorial |
| QAStatsManager | metrics |

---

# 4. Audio Timing

- Use `AudioContext.currentTime`.
- Schedule notes ahead.
- Compare click timestamps to audio window.
- Log offset for QA.
- Add calibration later.

---

# 5. Rendering

- Use Three.js WebGLRenderer.
- Use `renderer.setAnimationLoop`.
- Use primitive/procedural assets for prototype.
- GLTF optional later.
- Postprocessing optional, never required for gameplay clarity.

---

# 6. Data-Driven Level Schema

```json
{
  "id": "prologue_fragment_01",
  "chapter": "prologue",
  "title": "Breath of Blue",
  "mechanic": "sound_map",
  "targetObject": "blue_orb",
  "motif": ["low"],
  "reactionWindow": 1.8,
  "decoys": [],
  "reward": "low_note",
  "memoryFragment": "heartbeat_still_present"
}
```

---

# 7. Save Data

```json
{
  "version": "2.0",
  "unlockedChapters": ["prologue"],
  "restoredNotes": ["low", "mid", "high"],
  "fragments": [],
  "corruption": 0,
  "settings": {
    "reactionAssist": true,
    "audioClarity": true,
    "reducedWrongSfx": true,
    "reducedMotion": false
  }
}
```

---

# 8. Production Build Milestones

## Build A — Prologue Complete
- 5 fragments.
- 3 notes restored.
- Sound map stable.

## Build B — Chapter 1 Vertical Slice
- Silent Room.
- True/False Note.
- Silence.

## Build C — Chapter 2 Prototype
- Echo Memory.

## Build D — Chapter 3 Prototype
- Call-and-Response.

## Build E — Chapter 4 Prototype
- Heartbeat Recovery.

## Build F — Chapter 5 Finale
- Final Sonata.

---

# 9. Performance Budget

- Target 60 FPS desktop.
- Stable audio timing.
- Lightweight particles.
- Texture sizes controlled.
- Reduced visuals available.
- No gameplay dependency on bloom/postprocessing.


---

# 9. UX, Accessibility, Sensitivity & QA Plan


# Silent Sonata — UX, Accessibility, Sensitivity & QA Plan v2.0

## 0. Document Control
- Version: v2.0
- Date: 2026-05-14
- Status: Full UX/QA/Sensitivity Candidate

---

# 1. UX Principles

1. Teach before testing.
2. Feedback must explain.
3. Wrong feedback must not shame.
4. Audio-first, not audio-only.
5. Player comfort is part of design.

---

# 2. Full UX Flow

Start Menu → Content Warning → Settings Preset → Prologue Training → Chapter Select/Continue → Gameplay → Memory Gallery → Final Sonata → Ending → Reflection Screen.

---

# 3. Settings Presets

## Standard
Balanced challenge.

## Comfort
- Reaction Assist on.
- Reduced Wrong SFX on.
- Reduced Motion on.
- Audio Clarity on.
- Visual Timing Ring on.

## Focus
- Lower ambience.
- Stronger target cue.
- Minimal particles.

## Challenge
- Standard window.
- No labels.
- Normal decoys.

---

# 4. Accessibility Features

- Separate music/SFX/ambient/wrong SFX volume.
- Reaction Assist.
- Audio Clarity.
- Stereo Boost.
- Mono Friendly Mode.
- Visual Timing Ring.
- Reduced Motion.
- Reduced Distortion.
- Replay Cue.
- Object labels in tutorial.
- Content skip for Accident Memory.
- Simple language mode.

---

# 5. Sensitivity Plan

## Must Avoid
- stigmatizing language,
- realistic crash gore,
- jumpscare trauma,
- “insanity” framing,
- coma as gimmick.

## Accident Memory Safety
- symbolic visuals,
- content warning,
- skip with summary,
- reduced intensity option,
- no alarm-like harsh audio,
- no gore.

---

# 6. QA Plan

## Main QA Areas
- Gameplay clarity.
- 3-note training completion.
- 5-fragment flow.
- Audio source clarity.
- Wrong SFX comfort.
- Decoy fairness.
- Accessibility settings.
- Performance.
- Sensitivity safety.

## Key Metrics
| Metric | Target |
|---|---|
| Prologue completion | 85% |
| Rule comprehension | 80% in 30s |
| 3-ball sound identification | 75% |
| Wrong SFX comfort | 4/5 |
| Decoy fairness | 4/5 |
| Accident Memory comfort | 4/5 with warnings/settings |

---

# 7. Playtest Script

1. Ask player to start fresh.
2. Observe Prologue without explanation.
3. Ask: “Apa aturan game ini?”
4. Record if they identify 3 notes.
5. Trigger a wrong click and ask comfort rating.
6. Test laptop speaker and headphone if possible.
7. Test Chapter 1 sequence.
8. Ask if decoys feel fair.
9. Ask if they want to continue.
10. Collect open feedback.

---

# 8. Approval Gates

## Gate 1 — Prologue Approved
- 5 fragments understandable.
- 3 notes restored.
- Wrong feedback comfortable.

## Gate 2 — Chapter 1 Approved
- True/False and Silence understood.
- Decoys fair.

## Gate 3 — Vertical Slice Approved
- Prologue + Chapter 1 + one later mechanic.

## Gate 4 — Full Game Alpha
- All chapters playable.

## Gate 5 — Release Candidate
- No critical blocker.
- Accessibility and sensitivity check passed.


---

# 10. Production Roadmap, Backlog & AI Agent Prompts


# Silent Sonata — Production Roadmap, Backlog & AI Agent Prompts v2.0

## 0. Document Control
- Version: v2.0
- Date: 2026-05-14
- Status: Execution Roadmap Candidate

---

# 1. Production Strategy

Do not build all chapters at once. Build in proof layers:

1. Prologue training loop.
2. Chapter 1 vertical slice.
3. One advanced mechanic prototype.
4. Full chapter pipeline.
5. Full game alpha.
6. Polish and release candidate.

---

# 2. Roadmap

## Phase 12 — Prologue Full Implementation
Goal: 3 notes / 5 fragments.

Deliverables:
- sound map tutorial,
- 5 fragment sequences,
- fragment UI,
- soft wrong feedback,
- memory reward.

## Phase 13 — Chapter 1 Vertical Slice
Goal: polished Silent Room.

Deliverables:
- true/false note,
- silence,
- decoy,
- major encounter,
- first chapter memory.

## Phase 14 — Advanced Mechanic Prototype
Goal: prove Echo Memory or Heartbeat Recovery.

## Phase 15 — Full Chapter Production
Goal: build Chapters 2–5.

## Phase 16 — Full Game Alpha
Goal: playable start-to-end.

## Phase 17 — Polish & QA
Goal: tune, optimize, accessibility, sensitivity.

## Phase 18 — Release Candidate
Goal: demo/pitch/release-ready build.

---

# 3. Priority Backlog

## Must-Have
- Prologue 5 fragments.
- Three-note restoration.
- Full Chapter 1.
- Save progress.
- Accessibility settings.
- Soft wrong feedback.
- Memory gallery.
- Final Sonata system.

## Should-Have
- Full 5 chapters.
- Multiple endings.
- polished art.
- adaptive soundtrack.
- analytics/QA logs.

## Could-Have
- challenge mode,
- alternate visual skins,
- gallery replay,
- soundtrack mode.

---

# 4. AI Coding Agent Prompt — Prologue

```txt
You are a senior Three.js and Web Audio game developer.
Build the Silent Sonata Prologue: The First Three Notes.
Implement 5 fragments that restore 3 notes:
Fragment 1 Blue Orb Low,
Fragment 2 Rose Crystal Mid,
Fragment 3 Gold Prism High,
Fragment 4 random sound-source matching,
Fragment 5 Low → Mid → High phrase.
Use Web Audio API currentTime for timing, StereoPannerNode for left/right identity, and Three.js for scene rendering.
Wrong feedback must be soft. No harsh sawtooth or alarm sounds.
Add settings: Reaction Assist, Audio Clarity, Reduced Wrong SFX, Mono Friendly Mode, Replay Cue.
```

---

# 5. AI Art/Asset Agent Prompt

```txt
Create polished low-poly / stylized asset direction for Silent Sonata.
Focus on a dreamlike coma room, broken grand piano, three interactive musical lights, sheet music fragments, memory particles, and elegant corruption cracks.
The style is clean, melancholic, magical, intimate, and readable.
Do not make the scene horror. Do not over-clutter. Gameplay objects must remain readable.
```

---

# 6. AI Audio Agent Prompt

```txt
Design a soft, non-frustrating Web Audio placeholder sound set for Silent Sonata.
Create three object identities:
Blue Orb = low warm felt piano,
Rose Crystal = mid celesta,
Gold Prism = high glass chime.
Wrong feedback should be muted piano + sheet flutter, not harsh.
Correct feedback should be warm piano chord + memory chime.
```

---

# 7. Definition of Done — Prologue

- [ ] 5 fragments implemented.
- [ ] 3 notes restored.
- [ ] Player can identify left/mid/right.
- [ ] Wrong SFX comfort target met.
- [ ] Correct reward feels satisfying.
- [ ] Settings work.
- [ ] QA metrics logged.
- [ ] Build playable for testing.


---

# 11. Final Approval Checklist

## Creative
- [ ] Music remains truth.
- [ ] Visual deception supports gameplay.
- [ ] Story is emotional without melodrama.
- [ ] Piano remains symbolic center.

## Gameplay
- [ ] Prologue restores 3 notes via 5 fragments.
- [ ] Player understands low/mid/high.
- [ ] Decoys are fair.
- [ ] Wrong feedback is soft.
- [ ] Correct feedback is satisfying.

## Audio
- [ ] Three objects sound distinct.
- [ ] Source direction is clear.
- [ ] Wrong SFX is comfortable.
- [ ] Final Sonata grows over game.

## Art
- [ ] Assets are readable.
- [ ] Scene is appealing, not cluttered.
- [ ] Chapter visuals are distinct.
- [ ] Accident Memory is symbolic.

## Technical
- [ ] Web build is feasible.
- [ ] Audio timing uses audio clock.
- [ ] Managers are modular.
- [ ] Data-driven levels are possible.

## Accessibility & Sensitivity
- [ ] Settings are built in.
- [ ] Content warnings exist.
- [ ] Accident Memory has skip/summary.
- [ ] No stigmatizing language.

## QA
- [ ] Prologue tested.
- [ ] Chapter 1 tested.
- [ ] Audio clarity tested.
- [ ] Full game start-to-end tested before alpha approval.

---

# 12. Final Status

**Approved as Full Game Production & Execution Candidate v2.0.**

Next recommended production phase:

# Phase 12 — Prologue Full Implementation: 3 Notes / 5 Fragments


---

<!-- SOURCE: docs/02_Story_and_Narrative_Bible_v2.0.md -->

# Silent Sonata — Story & Narrative Bible v2.0

## 0. Document Control
- Version: v2.0
- Date: 2026-05-14
- Status: Full Game Narrative Candidate
- Scope: Complete story from opening to ending
- Core Narrative Rule: Story is revealed through sound, memory, object interaction, and recovery, not exposition-heavy dialogue.

---

# 1. Logline

A comatose pianist trapped in a surreal inner world must recover three lost notes, rebuild a broken sonata, and learn to trust music over deceptive visions before the final memory fades.

---

# 2. High Concept

Silent Sonata bercerita tentang seorang pianis muda yang mengalami kecelakaan setelah konser besar. Ia tidak sadar di dunia nyata, tetapi di dalam pikirannya ia berada di ruang fantasi yang dibentuk dari musik, memori, rasa bersalah, tekanan performa, dan keinginan untuk pulang.

Visual di dunia itu sering menipu. Cahaya bisa menjadi memori palsu. Applause bisa menjadi tekanan. Cermin bisa menjadi kritik diri. Headlight bisa menjadi panik. Satu-satunya hal yang masih konsisten adalah musik: piano, heartbeat, silence, echo, resonance, dan fragmen melodi.

---

# 3. Final Story Premise

## Dunia Nyata
Pianis utama baru menyelesaikan konser terpenting dalam hidupnya. Dalam perjalanan pulang, ia mengalami kecelakaan. Ia masuk koma. Orang-orang terdekatnya menunggu di ruang rumah sakit.

## Dunia Koma
Di dalam pikirannya, semua memori berubah menjadi ruang fantasi musikal. Piano rusak menjadi pusat dunia. Ia hanya bisa pulang jika Final Sonata tersusun kembali.

## Player Role
Pemain bukan “tubuh” karakter. Pemain adalah **inner listener**—bagian dari kesadaran pianis yang masih bisa membedakan musik yang benar dari visual yang menipu.

---

# 4. Main Character

## Working Name
**Liora**  
Nama ini bisa diganti, tetapi untuk production candidate dipakai sebagai placeholder final.

## Identity
- Pianis muda.
- Perfeksionis.
- Sensitif terhadap suara.
- Merasa dicintai karena performa, bukan karena dirinya.
- Terjebak antara keinginan menjadi sempurna dan keinginan untuk bebas bermain musik.

## Wound
Liora percaya bahwa jika ia gagal bermain sempurna, ia mengecewakan semua orang.

## Need
Ia harus belajar bahwa musik bukan bukti kesempurnaan, melainkan jalan pulang menuju diri sendiri.

## Arc
Perfeksionisme → Keraguan → Tekanan → Trauma → Penerimaan → Pulang.

---

# 5. Supporting Characters

## 5.1 The Mother / Family Voice
- Tidak banyak muncul secara visual.
- Hadir sebagai suara hangat, napas, atau motif sederhana.
- Melambangkan unconditional love.

## 5.2 The Mentor
- Guru piano lama Liora.
- Muncul sebagai memori lembut.
- Kalimat kunci: “Jangan mainkan nada yang benar saja. Mainkan nada yang jujur.”

## 5.3 The Audience
- Bisa menjadi dukungan atau tekanan.
- Dalam Chapter 3, applause menjadi ilusi yang harus diuji.

## 5.4 The Inner Critic
- Bukan villain literal.
- Muncul sebagai echo yang detuned, mirror reflection, dan false cue.
- Melambangkan standar sempurna yang menyakiti Liora.

---

# 6. Narrative Structure Overview

| Act | Chapter | Narrative Function | Emotional Question |
|---|---|---|---|
| Prologue | The First Three Notes | Liora belajar kembali mendengar | “Apa suara pertamaku?” |
| Act I | The Silent Room | Ia memahami aturan dunia koma | “Bisakah aku percaya musik?” |
| Act II | The Hall of False Notes | Ia menghadapi kritik diri | “Apakah semua kesalahan adalah kegagalan?” |
| Act III | The Broken Concert | Ia menghadapi tekanan publik | “Apakah aku masih bernilai tanpa tepuk tangan?” |
| Act IV | The Accident Memory | Ia menghadapi trauma kecelakaan | “Bisakah aku menerima yang terjadi?” |
| Act V | The Last Sonata | Ia menyusun pulang | “Bisakah aku memainkan lagu yang jujur?” |
| Epilogue | Awakening | Dunia nyata kembali | “Apakah aku siap hidup lagi?” |

---

# 7. Prologue — The First Three Notes

## Purpose
Fase latihan awal sekaligus pembuka cerita. Pemain memulihkan **3 nada inti** dengan mengumpulkan **5 fragmen**.

## Three Core Notes

| Note | Object | Meaning | Story Function |
|---|---|---|---|
| Low Note | Blue Orb | Grounding / breath | Liora masih hidup |
| Middle Note | Rose Crystal | Heart / memory | Liora masih punya rasa |
| High Note | Gold Prism | Hope / awakening | Liora masih bisa pulang |

## Five Training Fragments

| Fragment | Name | Gameplay | Narrative Reveal | Restored Result |
|---|---|---|---|---|
| Fragment 1 | Breath of Blue | Klik Blue Orb setelah low cue | Detak jantung masih ada | Low Note unlocked |
| Fragment 2 | Rose in Silence | Klik Rose setelah mid cue | Ada seseorang menunggu | Middle Note seed |
| Fragment 3 | Gold Through the Dark | Klik Gold setelah high cue | Ada cahaya di ujung memori | High Note seed |
| Fragment 4 | The Three Voices | Cocokkan low/mid/high acak | Ketiga suara menjadi peta | Middle + High stabilized |
| Fragment 5 | First Phrase | Mainkan pola Low → Mid → High | Piano mulai mengingat | Three-note motif restored |

## Narrative Beat
Setelah Fragment 5, piano rusak memainkan phrase pertama Final Sonata. Ruangan tidak lagi sepenuhnya gelap. Ini adalah momen pertama bahwa Liora mungkin bisa bangun.

---

# 8. Chapter 1 — The Silent Room

## Emotional Theme
Confusion, curiosity, fragile hope.

## Story
Liora berada di ruangan sunyi yang tidak ia kenali, tetapi ada piano rusak di tengah ruangan. Tiga cahaya muncul sebagai suara pertama dunia ini. Pemain belajar bahwa suara memandu, visual bisa menipu.

## Memory Reveal
Concert hall appears as a blurred image. Liora remembers being on stage, but not what happened after.

## Key Memory Fragments
1. Piano room at home.
2. First recital photo.
3. Final concert ticket.
4. Blurred audience.
5. Broken sheet music.

## Ending Beat
Pintu menuju Hall of False Notes terbuka ketika pemain dapat membedakan truth cue dan false visual cue.

---

# 9. Chapter 2 — The Hall of False Notes

## Emotional Theme
Self-doubt and perfectionism.

## Story
Liora memasuki koridor cermin. Setiap cermin memainkan kembali nada yang pernah ia mainkan salah. Inner Critic membuat echo palsu agar Liora percaya bahwa satu kesalahan menghancurkan semuanya.

## Gameplay-Narrative Link
Echo Memory mechanic: pemain mendengar motif asli, lalu echo corrupt, dan memperbaiki nada yang salah.

## Memory Reveal
Liora ingat latihan keras, kompetisi, dan perkataan orang-orang yang ia tafsirkan sebagai tuntutan.

## Ending Beat
Mentor memory appears and says through piano, “A wrong note can still lead home.”

---

# 10. Chapter 3 — The Broken Concert

## Emotional Theme
Performance anxiety, public judgment, exposure.

## Story
Dunia berubah menjadi concert hall yang retak. Audience muncul sebagai cahaya tanpa wajah. Applause kadang menjadi dukungan, kadang menjadi pressure. Liora harus membedakan applause asli dan false applause.

## Gameplay-Narrative Link
Call-and-Response mechanic: pemain menjawab motif, lalu menilai apakah dunia membalas dengan benar.

## Memory Reveal
Final concert was not a failure. Liora played beautifully, but she could not feel it because she was trapped in fear.

## Ending Beat
Concert hall collapses into road-light fragments. The accident memory begins to leak into the world.

---

# 11. Chapter 4 — The Accident Memory

## Emotional Theme
Fear, shock, acceptance.

## Story
Dunia menjadi jalan abstrak yang terbuat dari headlight, garis heartbeat, pecahan kaca simbolik, dan silence. Tidak ada gore. Tidak ada crash realistis. Semua digambarkan sebagai memori tubuh yang sulit dipahami.

## Gameplay-Narrative Link
Heartbeat Recovery mechanic: pemain menahan dan melepas input untuk menstabilkan detak jantung.

## Memory Reveal
Liora bukan gagal. Kecelakaan terjadi. Ia tidak perlu menghukum dirinya untuk sesuatu yang tidak bisa ia kendalikan.

## Sensitivity Lock
Scene ini wajib memiliki:
- content warning,
- reduced intensity setting,
- skip with summary option,
- no realistic gore,
- no alarm-like harsh sound,
- no shock jumpscare.

## Ending Beat
Heartbeat stabil. Liora menerima bahwa pulang bukan berarti menghapus trauma, tetapi membawa dirinya kembali.

---

# 12. Chapter 5 — The Last Sonata

## Emotional Theme
Closure, integration, awakening.

## Story
Semua ruang menyatu menjadi panggung putih-keemasan. Piano yang rusak mulai utuh. Pemain memainkan Final Sonata dengan motif dari seluruh game: low grounding, mid heart, high hope, silence, echo, heartbeat, applause, and acceptance.

## Gameplay-Narrative Link
Build the Final Song: semua mechanics kembali, tetapi dalam bentuk lebih elegan dan tidak terlalu menghukum.

## Final Memory Reveal
Orang-orang terdekat Liora berada di rumah sakit. Suara mereka bukan tekanan, tetapi panggilan pulang.

---

# 13. Endings

## 13.1 Clear Awakening
Condition:
- High fragment completion.
- Low or moderate corruption.
- Final Sonata mostly complete.

Ending:
Liora bangun. Ia tidak langsung berbicara. Ia mendengar suara piano phrase terakhir, lalu menggenggam tangan orang terdekat.

## 13.2 Soft Awakening
Condition:
- Enough fragments.
- Some corruption unresolved.

Ending:
Liora bangun perlahan. Beberapa memori masih kabur. Musik terdengar tidak sempurna, tetapi hangat.

## 13.3 Dreaming Coda
Condition:
- Low fragment completion.
- High corruption.

Ending:
Liora belum sepenuhnya bangun, tetapi Final Sonata tidak hilang. Player melihat satu note tetap menyala, menandakan harapan dan retry path.

## Design Rule
No ending should feel cruel. Even incomplete endings must preserve dignity and hope.

---

# 14. Narrative Asset List

## Memory Images / Symbols
- Broken sheet music.
- Concert ticket.
- Old metronome.
- Cracked mirror.
- Mentor’s red pencil.
- Empty audience seat.
- Stage spotlight.
- Road-light streak.
- Hospital curtain silhouette.
- Family hand silhouette.

## Narrative Audio
- Mother/family hum motif.
- Mentor motif.
- Audience motif.
- Inner critic detuned echo.
- Hospital room distant ambience.
- Final Sonata phrase.

---

# 15. Narrative Approval Checklist

- [ ] Story is understandable without heavy exposition.
- [ ] Coma is symbolic, not medically overclaimed.
- [ ] Trauma is handled without shock exploitation.
- [ ] Main character has agency and dignity.
- [ ] Each chapter reveals a meaningful memory.
- [ ] Final ending feels earned.


---

<!-- SOURCE: docs/03_Gameplay_and_Systems_Bible_v2.0.md -->

# Silent Sonata — Gameplay & Systems Bible v2.0

## 0. Document Control
- Version: v2.0
- Date: 2026-05-14
- Status: Full Game Systems Candidate
- Scope: All gameplay systems from tutorial to finale

---

# 1. Gameplay North Star

Silent Sonata is about listening before reacting.

> The player does not win by seeing faster.  
> The player wins by hearing what is true.

---

# 2. Final Core Loop

## Moment-to-Moment Loop
**Listen → Identify → Wait → React → Learn**

## Emotional Loop
**Confusion → Trust → Doubt → Recovery**

## Full Game Loop
**Recover Fragment → Restore Motif → Unlock Memory → Change World → Advance Chapter**

---

# 3. Prologue Training System — 3 Notes / 5 Fragments

## Goal
The early training phase teaches the entire language of the game before real challenge begins.

## Player Objective
Recover 5 fragments to restore 3 notes:
1. Low Note
2. Middle Note
3. High Note

## Why 5 Fragments for 3 Notes?
Because the player should not only unlock the notes, but understand them.

| Fragment | Teaches | Restores |
|---|---|---|
| Fragment 1 | Left/Low identity | Low Note |
| Fragment 2 | Center/Mid identity | Middle Note seed |
| Fragment 3 | Right/High identity | High Note seed |
| Fragment 4 | Sound direction + matching | Stabilizes Mid + High |
| Fragment 5 | Low → Mid → High phrase | Completes the Three-Note Motif |

## Training Completion Reward
- The piano plays the first complete phrase.
- Fragment counter becomes “5/5”.
- Three-note motif becomes the player’s first permanent musical memory.
- The Silent Room opens into the full Chapter 1 challenge.

---

# 4. Object Identity System

| Object | Name | Sound | Visual | Gameplay Role |
|---|---|---|---|---|
| Left | Blue Orb | Low warm voice | Slow wide ring | Grounding |
| Center | Rose Crystal | Mid bell-piano | Double ring | Heart / balance |
| Right | Gold Prism | High glass chime | Sharp shimmer ring | Hope / light |

## Identity Rule
The player must be able to identify each object through:
- position,
- sound pitch,
- timbre,
- stereo or visual direction,
- ring pattern,
- tutorial label.

---

# 5. Reaction Timing System

## State Flow
1. LISTEN
2. GET READY
3. CLICK NOW
4. RESULT

## Timing Windows
| Mode | Window |
|---|---|
| Tutorial | 1.8s |
| Practice | 1.5s |
| Standard | 1.15s |
| Challenge | 0.9s |
| Assist | +0.4s to +0.7s |

## Rule
No hard punishment until the player has completed the 5-fragment training phase.

---

# 6. Fragment System

## Fragment Types

| Fragment Type | Source | Function |
|---|---|---|
| Note Fragment | Object matching | Adds melody |
| Silence Fragment | No-input challenge | Adds rests |
| Echo Fragment | Echo correction | Adds harmony |
| Pulse Fragment | Heartbeat recovery | Adds rhythm |
| Memory Fragment | Major encounter | Adds narrative clarity |

## Fragment States
- Hidden
- Heard
- Recovered
- Stabilized
- Integrated into Final Sonata

---

# 7. Corruption & Recovery System

## Corruption Sources
- Wrong object.
- Too early.
- Too late.
- Clicking during silence.
- Following a decoy.
- Failing heartbeat hold.
- Accepting false echo.

## Recovery Sources
- Correct object.
- Waiting through silence.
- Correct echo repair.
- Stable heartbeat.
- Completing a memory fragment.
- Playing a motif phrase correctly.

## Corruption Levels
| Level | Audio | Visual | Gameplay |
|---|---|---|---|
| 0–1 | Clean piano | calm blue | wide timing |
| 2–3 | light detune | tiny cracks | normal |
| 4–5 | echo noise | distortion | decoys increase |
| 6–7 | heartbeat unstable | stronger cracks | recovery needed |
| 8 | soft fail | scene dims | retry phrase |

## Soft Fail Rule
No hard game over. The world gives a recovery phrase or returns to the last stable fragment.

---

# 8. Wrong Feedback System

Wrong feedback is a teacher, not a punishment.

| Mistake | Sound | Text | Visual |
|---|---|---|---|
| Too early | soft closed key | “Tunggu CLICK NOW.” | progress pulse resets |
| Too late | fading echo | “Ring sudah menutup.” | truth ring fades |
| Wrong object | muted piano + paper flutter | “Itu visual palsu.” | correct object hint pulse |
| Silence mistake | room hush | “Diam berarti jangan klik.” | room dims gently |

---

# 9. Correct Feedback System

Correct feedback must feel like healing.

## Correct Reward Stack
1. Warm piano chord.
2. Memory chime.
3. Fragment flies to piano.
4. Piano key glows.
5. Heartbeat stabilizes.
6. Scene warms slightly.
7. Final Sonata gains one layer.

---

# 10. Mechanics

## 10.1 True Note / False Note
Choose the object that sings with the final note.

## 10.2 Silence Means Truth
Do not click when silence is the truth.

## 10.3 Echo Memory
Compare original motif and echo; repair the wrong note.

## 10.4 Call-and-Response
Repeat or judge rhythmic phrase.

## 10.5 Heartbeat Recovery
Hold/release to stabilize heartbeat.

## 10.6 Memory Weaving
Place recovered fragments into the Final Sonata timeline.

## 10.7 Final Sonata Performance
Use all learned mechanics in a final musical sequence.

---

# 11. Difficulty Progression

| Phase | Player Skill |
|---|---|
| Prologue | Identify three voices |
| Chapter 1 | Trust clean truth |
| Chapter 2 | Detect altered truth |
| Chapter 3 | Respond under pressure |
| Chapter 4 | Stay calm under panic |
| Chapter 5 | Integrate all truth |

---

# 12. Accessibility-First Gameplay Rules

- No color-only critical cue.
- Audio cue always has visual support.
- Wrong SFX can be reduced.
- Reaction Assist available.
- Replay cue available.
- Visual Timing Ring available.
- Mono Friendly Mode available.
- Content warning before Accident Memory.


---

<!-- SOURCE: docs/04_Level_Design_and_Encounter_Bible_v2.0.md -->

# Silent Sonata — Level Design & Encounter Bible v2.0

## 0. Document Control
- Version: v2.0
- Date: 2026-05-14
- Status: Full Level Design Candidate
- Structure: Prologue + 5 Chapters + Epilogue
- Playable Sequences: 21 main sequences + optional memory rooms

---

# 1. Level Design Philosophy

Every level must do four things:
1. teach or test one musical truth,
2. reveal one emotional layer,
3. change the world visually or musically,
4. move the player closer to Final Sonata.

No filler levels.

---

# 2. Full Game Level Structure

| Sequence | Name | Chapter | Main Mechanic | Narrative Reward |
|---:|---|---|---|---|
| 0 | The First Three Notes | Prologue | Sound Map / 5 Fragments | 3-note motif |
| 1 | The First Light | Silent Room | True Note | First room memory |
| 2 | The Quiet Between | Silent Room | Silence | restraint memory |
| 3 | The Beautiful Lie | Silent Room | Soft Decoy | false visual rule |
| 4 | The Door of Sound | Silent Room | Major Encounter | Chapter 1 memory |
| 5 | Clean Echo | Hall | Echo Memory intro | original motif |
| 6 | Wrong Reflection | Hall | False Echo | self-doubt memory |
| 7 | Mirror Corridor | Hall | Echo + Decoy | mentor memory |
| 8 | The Note That Wasn't Failure | Hall | Major Encounter | acceptance of wrong note |
| 9 | Stage Breath | Concert | Call-and-Response intro | backstage memory |
| 10 | False Applause | Concert | Applause judgment | audience pressure |
| 11 | Spotlight Tremor | Concert | tempo pressure | final concert memory |
| 12 | The Broken Crescendo | Concert | Major Encounter | concert truth |
| 13 | Pulse Line | Accident | Heartbeat intro | leaving hall |
| 14 | Headlight Silence | Accident | Silence + panic visual | pre-crash memory |
| 15 | Impact Pause | Accident | heartbeat recovery | accident acceptance |
| 16 | The Breath After | Accident | Major Encounter | trauma integration |
| 17 | Returning Motif | Last Sonata | all mechanics light | loved voice |
| 18 | Harmony in Doubt | Last Sonata | all mechanics medium | full memory weave |
| 19 | The False Door | Last Sonata | final decoy | reject false comfort |
| 20 | Final Awakening | Last Sonata | Final Sonata | ending |
| 21 | Coda | Epilogue | reflection | awakening state |

---

# 3. Prologue Detail — The First Three Notes

## Objective
Recover 3 notes using 5 fragments.

## Micro-Sequence

### Fragment 1 — Breath of Blue
- Object: Blue Orb.
- Sound: low warm tone.
- Task: click when Blue sings.
- Reward: Low Note restored.

### Fragment 2 — Rose in Silence
- Object: Rose Crystal.
- Sound: mid celesta.
- Task: click Rose after mid cue.
- Reward: Middle Note seed restored.

### Fragment 3 — Gold Through the Dark
- Object: Gold Prism.
- Sound: high glass chime.
- Task: click Gold after high cue.
- Reward: High Note seed restored.

### Fragment 4 — The Three Voices
- Objects: all three.
- Task: identify random sound source.
- Reward: sound map stabilized.

### Fragment 5 — First Phrase
- Pattern: Low → Mid → High.
- Task: click 3-note phrase in order.
- Reward: first phrase of Final Sonata.

## Completion Moment
Piano plays Low → Mid → High. The broken keybed glows. The UI changes from “Training” to “Chapter 1”.

---

# 4. Chapter 1 — The Silent Room

## Level 1: The First Light
Teaches true note with low stakes.

## Level 2: The Quiet Between
Introduces silence. Correct action can be no action.

## Level 3: The Beautiful Lie
Introduces fair visual decoy.

## Major Encounter: The Door of Sound
Combines three voices, truth ring, and one silence sequence. Unlocks Hall of False Notes.

---

# 5. Chapter 2 — The Hall of False Notes

## Level 5: Clean Echo
Original motif plays, then clean echo. Player learns echo vocabulary.

## Level 6: Wrong Reflection
One echo note is wrong. Player chooses the wrong moment to repair it.

## Level 7: Mirror Corridor
Visual mirrors multiply. Audio remains source of truth.

## Major Encounter: The Note That Wasn't Failure
Player must repair a longer motif while Inner Critic tries to make every note feel wrong.

---

# 6. Chapter 3 — The Broken Concert

## Level 9: Stage Breath
Player repeats simple rhythmic call.

## Level 10: False Applause
Player judges if audience response is true support or pressure illusion.

## Level 11: Spotlight Tremor
Tempo shifts subtly; player uses breathing cues.

## Major Encounter: The Broken Crescendo
Player performs under visual collapse while following clean audio.

---

# 7. Chapter 4 — The Accident Memory

## Level 13: Pulse Line
Heartbeat tutorial. Hold/release gently.

## Level 14: Headlight Silence
Visual panic appears, but silence means no input.

## Level 15: Impact Pause
Heartbeat falters. Player stabilizes without harsh alarm sounds.

## Major Encounter: The Breath After
Player accepts the accident memory through a calm recovery sequence.

---

# 8. Chapter 5 — The Last Sonata

## Level 17: Returning Motif
All three notes return.

## Level 18: Harmony in Doubt
Echo, silence, and call-response combine.

## Level 19: The False Door
A beautiful visual exit appears but is not musically true.

## Major Encounter: Final Awakening
The player performs Final Sonata and triggers ending logic.

---

# 9. Encounter Template

1. Establish emotion.
2. Play clean motif.
3. Introduce mechanic.
4. Let player practice without harsh penalty.
5. Add fair deception.
6. Reward with fragment.
7. Show memory.
8. Change world.

---

# 10. Level Acceptance Checklist

- [ ] Level teaches one clear thing.
- [ ] Audio cue is readable.
- [ ] Visual deception is fair.
- [ ] Wrong feedback is soft.
- [ ] Correct feedback is satisfying.
- [ ] Memory reward is meaningful.
- [ ] Accessibility settings work.


---

<!-- SOURCE: docs/05_Music_and_Audio_Bible_v2.0.md -->

# Silent Sonata — Music & Audio Bible v2.0

## 0. Document Control
- Version: v2.0
- Date: 2026-05-14
- Status: Full Music & Audio Candidate

---

# 1. Music Philosophy

Music is not background. Music is truth, map, feedback, memory, and story.

---

# 2. Final Sonata Structure

| Movement | Chapter | Musical Function | Emotional Function |
|---|---|---|---|
| I. Three Notes | Prologue | Low/Mid/High motif | learning to hear |
| II. Silent Theme | Silent Room | rests and space | trust |
| III. Echo Theme | Hall | call/echo harmony | self-doubt |
| IV. Concert Theme | Broken Concert | response rhythm | pressure |
| V. Pulse Theme | Accident | heartbeat rhythm | trauma |
| VI. Awakening Theme | Last Sonata | all motifs integrated | return |

---

# 3. Three Core Notes

| Note | Object | Pitch Area | Timbre | Meaning |
|---|---|---|---|---|
| Low | Blue Orb | C3/D3 | warm felt piano | breath / grounding |
| Mid | Rose Crystal | E4/F4 | celesta / bell-piano | heart / balance |
| High | Gold Prism | G5/A5 | glass chime | hope / awakening |

---

# 4. Motif Library

## Truth Motif
Low → Mid → High.

## Silence Motif
A rest that means “do not act.”

## Echo Motif
Original phrase followed by slightly altered phrase.

## Heartbeat Motif
Pulse rhythm that can stabilize or falter.

## Recovery Motif
Warm consonant chord with memory chime.

## Corruption Motif
Soft detune and unstable echo; never painful.

## Final Sonata Motif
All core motifs layered into one playable phrase.

---

# 5. Wrong Feedback Audio

Wrong feedback is soft correction.

## Sound Palette
- Muted piano thud.
- Sheet music flutter.
- Soft reverse note.
- Low heartbeat dip.
- Gentle detune only in challenge.

## Mixing Rule
Wrong feedback must be quieter than motif and shorter than correct feedback.

---

# 6. Correct Feedback Audio

Correct feedback is healing.

## Sound Palette
- Warm piano chord.
- Memory chime.
- Room breath.
- Stabilized heartbeat.
- Piano resonance.

---

# 7. Adaptive Audio States

| State | Audio |
|---|---|
| Calm | clear piano, low ambience |
| Doubt | light echo |
| Panic | heartbeat increases, but not harsh |
| Recovery | warm chord |
| Corruption | soft detune |
| Awakening | full harmony |

---

# 8. Technical Audio Requirements

- Use Web Audio API.
- Use audio clock timing.
- Use StereoPannerNode for object panning.
- Use GainNodes for separate buses.
- Use optional PannerNode later for 3D scene depth.
- Separate sliders: music, SFX, ambience, wrong SFX, accessibility cues.

---

# 9. Audio Asset List

## MVP
- heartbeat_loop_soft
- motif_three_notes_low_mid_high
- blue_orb_low
- rose_crystal_mid
- gold_prism_high
- correct_warm_chord
- wrong_soft_muted
- sheet_flutter
- silence_hush

## Full Game
- echo_clean
- echo_corrupt
- audience_true
- audience_false
- stage_pressure_rhythm
- accident_heartbeat_unstable
- accident_recovery_pulse
- final_sonata_layer_1_low
- final_sonata_layer_2_mid
- final_sonata_layer_3_high
- final_sonata_full


---

<!-- SOURCE: docs/06_Art_and_Asset_Bible_v2.0.md -->

# Silent Sonata — Art & Asset Bible v2.0

## 0. Document Control
- Version: v2.0
- Date: 2026-05-14
- Status: Full Art & Asset Candidate

---

# 1. Visual North Star

Silent Sonata should look like music becoming light inside a dream.

---

# 2. Visual Pillars

1. Piano as sacred object.
2. Light as memory.
3. Space as emotion.
4. Minimal but premium.
5. Readability before beauty.
6. Deception must be elegant, not noisy.
7. Trauma must be symbolic, not graphic.

---

# 3. Global Asset Categories

## Characters
- Liora silhouette / memory form.
- Mother/family silhouette.
- Mentor silhouette.
- Audience light silhouettes.
- Inner Critic mirror shadow.

## Core Props
- Broken grand piano.
- Restored grand piano.
- Piano bench.
- Sheet music fragments.
- Old metronome.
- Concert ticket.
- Mentor pencil.
- Broken mirror shard.
- Hospital curtain silhouette.

## Interactive Objects
- Blue Orb.
- Rose Crystal.
- Gold Prism.
- Truth ring.
- Decoy ring.
- Sound wave line.
- Memory fragment object.

## Environments
- Coma Room.
- Silent Room.
- Hall of False Notes.
- Broken Concert.
- Accident Memory Road.
- Last Sonata Stage.
- Epilogue hospital light.

---

# 4. Prologue Asset Set

## Required
- Broken piano with 3 inactive keys.
- Blue Orb with wide ring.
- Rose Crystal with double ring.
- Gold Prism with shimmer ring.
- 5 floating fragments.
- First phrase staff line.
- UI labels LOW / MID / HIGH.

---

# 5. Chapter Environment Direction

## Chapter 1 — Silent Room
Dark blue, empty, piano-centered, fragile lights.

## Chapter 2 — Hall of False Notes
Mirrors, long hallway, reflected pianos, purple-silver palette.

## Chapter 3 — Broken Concert
Cracked stage, floating seats, spotlight, gold-red palette.

## Chapter 4 — Accident Memory
Abstract road lines, floating glass symbols, heartbeat line, no gore.

## Chapter 5 — Last Sonata
White-gold stage, restored piano, memory particles, warm atmosphere.

---

# 6. VFX List

## Truth VFX
- clean ring,
- sound wave pulse,
- small note icon,
- gentle particle lift.

## Recovery VFX
- sheet music flies into piano,
- piano key glow,
- room warms,
- heartbeat stabilizes.

## Corruption VFX
- elegant cracks,
- soft purple distortion,
- slight bloom shift,
- no horror flashes.

---

# 7. UI Asset Direction

UI should combine sheet music and heartbeat monitor.

## UI Elements
- phase label,
- timing ring,
- fragment counter,
- corruption meter,
- sound map icons,
- replay cue,
- accessibility settings,
- chapter transition card.

---

# 8. Asset Manifest Summary

A detailed JSON manifest is included in `data/full_game_asset_manifest_v2.0.json`.


---

<!-- SOURCE: docs/07_Technical_Design_and_Implementation_Plan_v2.0.md -->

# Silent Sonata — Technical Design & Implementation Plan v2.0

## 0. Document Control
- Version: v2.0
- Date: 2026-05-14
- Status: Full Technical Candidate
- Platform: Web browser
- Stack: HTML, CSS, JavaScript, Three.js, Web Audio API

---

# 1. Architecture Goals

1. Stable browser performance.
2. Audio-first timing.
3. Modular scene system.
4. Data-driven levels.
5. Accessibility built in.
6. Easy for AI coding agents to implement.

---

# 2. Folder Structure

```txt
silent-sonata/
  index.html
  package.json
  src/
    main.js
    core/
      Game.js
      StateMachine.js
      EventBus.js
    systems/
      AudioManager.js
      RhythmManager.js
      SceneManager.js
      InputManager.js
      UIManager.js
      AccessibilityManager.js
      CorruptionManager.js
      FragmentManager.js
      SaveManager.js
      QAStatsManager.js
    scenes/
      PrologueScene.js
      SilentRoomScene.js
      HallOfFalseNotesScene.js
      BrokenConcertScene.js
      AccidentMemoryScene.js
      LastSonataScene.js
      EpilogueScene.js
    assets/
      models/
      textures/
      audio/
    data/
      levels.json
      motifs.json
      assets.json
      dialogue.json
```

---

# 3. Core Managers

| Manager | Responsibility |
|---|---|
| Game | boot, loop, global lifecycle |
| StateMachine | LISTEN/READY/CLICK/RESULT |
| AudioManager | Web Audio routing |
| RhythmManager | timing windows |
| SceneManager | load/unload chapters |
| InputManager | click/hold/tap input |
| FragmentManager | 5 fragments, notes, memories |
| CorruptionManager | corruption/recovery |
| AccessibilityManager | settings |
| UIManager | HUD/tutorial |
| QAStatsManager | metrics |

---

# 4. Audio Timing

- Use `AudioContext.currentTime`.
- Schedule notes ahead.
- Compare click timestamps to audio window.
- Log offset for QA.
- Add calibration later.

---

# 5. Rendering

- Use Three.js WebGLRenderer.
- Use `renderer.setAnimationLoop`.
- Use primitive/procedural assets for prototype.
- GLTF optional later.
- Postprocessing optional, never required for gameplay clarity.

---

# 6. Data-Driven Level Schema

```json
{
  "id": "prologue_fragment_01",
  "chapter": "prologue",
  "title": "Breath of Blue",
  "mechanic": "sound_map",
  "targetObject": "blue_orb",
  "motif": ["low"],
  "reactionWindow": 1.8,
  "decoys": [],
  "reward": "low_note",
  "memoryFragment": "heartbeat_still_present"
}
```

---

# 7. Save Data

```json
{
  "version": "2.0",
  "unlockedChapters": ["prologue"],
  "restoredNotes": ["low", "mid", "high"],
  "fragments": [],
  "corruption": 0,
  "settings": {
    "reactionAssist": true,
    "audioClarity": true,
    "reducedWrongSfx": true,
    "reducedMotion": false
  }
}
```

---

# 8. Production Build Milestones

## Build A — Prologue Complete
- 5 fragments.
- 3 notes restored.
- Sound map stable.

## Build B — Chapter 1 Vertical Slice
- Silent Room.
- True/False Note.
- Silence.

## Build C — Chapter 2 Prototype
- Echo Memory.

## Build D — Chapter 3 Prototype
- Call-and-Response.

## Build E — Chapter 4 Prototype
- Heartbeat Recovery.

## Build F — Chapter 5 Finale
- Final Sonata.

---

# 9. Performance Budget

- Target 60 FPS desktop.
- Stable audio timing.
- Lightweight particles.
- Texture sizes controlled.
- Reduced visuals available.
- No gameplay dependency on bloom/postprocessing.


---

<!-- SOURCE: docs/08_UX_Accessibility_Sensitivity_QA_Plan_v2.0.md -->

# Silent Sonata — UX, Accessibility, Sensitivity & QA Plan v2.0

## 0. Document Control
- Version: v2.0
- Date: 2026-05-14
- Status: Full UX/QA/Sensitivity Candidate

---

# 1. UX Principles

1. Teach before testing.
2. Feedback must explain.
3. Wrong feedback must not shame.
4. Audio-first, not audio-only.
5. Player comfort is part of design.

---

# 2. Full UX Flow

Start Menu → Content Warning → Settings Preset → Prologue Training → Chapter Select/Continue → Gameplay → Memory Gallery → Final Sonata → Ending → Reflection Screen.

---

# 3. Settings Presets

## Standard
Balanced challenge.

## Comfort
- Reaction Assist on.
- Reduced Wrong SFX on.
- Reduced Motion on.
- Audio Clarity on.
- Visual Timing Ring on.

## Focus
- Lower ambience.
- Stronger target cue.
- Minimal particles.

## Challenge
- Standard window.
- No labels.
- Normal decoys.

---

# 4. Accessibility Features

- Separate music/SFX/ambient/wrong SFX volume.
- Reaction Assist.
- Audio Clarity.
- Stereo Boost.
- Mono Friendly Mode.
- Visual Timing Ring.
- Reduced Motion.
- Reduced Distortion.
- Replay Cue.
- Object labels in tutorial.
- Content skip for Accident Memory.
- Simple language mode.

---

# 5. Sensitivity Plan

## Must Avoid
- stigmatizing language,
- realistic crash gore,
- jumpscare trauma,
- “insanity” framing,
- coma as gimmick.

## Accident Memory Safety
- symbolic visuals,
- content warning,
- skip with summary,
- reduced intensity option,
- no alarm-like harsh audio,
- no gore.

---

# 6. QA Plan

## Main QA Areas
- Gameplay clarity.
- 3-note training completion.
- 5-fragment flow.
- Audio source clarity.
- Wrong SFX comfort.
- Decoy fairness.
- Accessibility settings.
- Performance.
- Sensitivity safety.

## Key Metrics
| Metric | Target |
|---|---|
| Prologue completion | 85% |
| Rule comprehension | 80% in 30s |
| 3-ball sound identification | 75% |
| Wrong SFX comfort | 4/5 |
| Decoy fairness | 4/5 |
| Accident Memory comfort | 4/5 with warnings/settings |

---

# 7. Playtest Script

1. Ask player to start fresh.
2. Observe Prologue without explanation.
3. Ask: “Apa aturan game ini?”
4. Record if they identify 3 notes.
5. Trigger a wrong click and ask comfort rating.
6. Test laptop speaker and headphone if possible.
7. Test Chapter 1 sequence.
8. Ask if decoys feel fair.
9. Ask if they want to continue.
10. Collect open feedback.

---

# 8. Approval Gates

## Gate 1 — Prologue Approved
- 5 fragments understandable.
- 3 notes restored.
- Wrong feedback comfortable.

## Gate 2 — Chapter 1 Approved
- True/False and Silence understood.
- Decoys fair.

## Gate 3 — Vertical Slice Approved
- Prologue + Chapter 1 + one later mechanic.

## Gate 4 — Full Game Alpha
- All chapters playable.

## Gate 5 — Release Candidate
- No critical blocker.
- Accessibility and sensitivity check passed.


---

<!-- SOURCE: docs/09_Production_Roadmap_Backlog_and_AI_Agent_Prompts_v2.0.md -->

# Silent Sonata — Production Roadmap, Backlog & AI Agent Prompts v2.0

## 0. Document Control
- Version: v2.0
- Date: 2026-05-14
- Status: Execution Roadmap Candidate

---

# 1. Production Strategy

Do not build all chapters at once. Build in proof layers:

1. Prologue training loop.
2. Chapter 1 vertical slice.
3. One advanced mechanic prototype.
4. Full chapter pipeline.
5. Full game alpha.
6. Polish and release candidate.

---

# 2. Roadmap

## Phase 12 — Prologue Full Implementation
Goal: 3 notes / 5 fragments.

Deliverables:
- sound map tutorial,
- 5 fragment sequences,
- fragment UI,
- soft wrong feedback,
- memory reward.

## Phase 13 — Chapter 1 Vertical Slice
Goal: polished Silent Room.

Deliverables:
- true/false note,
- silence,
- decoy,
- major encounter,
- first chapter memory.

## Phase 14 — Advanced Mechanic Prototype
Goal: prove Echo Memory or Heartbeat Recovery.

## Phase 15 — Full Chapter Production
Goal: build Chapters 2–5.

## Phase 16 — Full Game Alpha
Goal: playable start-to-end.

## Phase 17 — Polish & QA
Goal: tune, optimize, accessibility, sensitivity.

## Phase 18 — Release Candidate
Goal: demo/pitch/release-ready build.

---

# 3. Priority Backlog

## Must-Have
- Prologue 5 fragments.
- Three-note restoration.
- Full Chapter 1.
- Save progress.
- Accessibility settings.
- Soft wrong feedback.
- Memory gallery.
- Final Sonata system.

## Should-Have
- Full 5 chapters.
- Multiple endings.
- polished art.
- adaptive soundtrack.
- analytics/QA logs.

## Could-Have
- challenge mode,
- alternate visual skins,
- gallery replay,
- soundtrack mode.

---

# 4. AI Coding Agent Prompt — Prologue

```txt
You are a senior Three.js and Web Audio game developer.
Build the Silent Sonata Prologue: The First Three Notes.
Implement 5 fragments that restore 3 notes:
Fragment 1 Blue Orb Low,
Fragment 2 Rose Crystal Mid,
Fragment 3 Gold Prism High,
Fragment 4 random sound-source matching,
Fragment 5 Low → Mid → High phrase.
Use Web Audio API currentTime for timing, StereoPannerNode for left/right identity, and Three.js for scene rendering.
Wrong feedback must be soft. No harsh sawtooth or alarm sounds.
Add settings: Reaction Assist, Audio Clarity, Reduced Wrong SFX, Mono Friendly Mode, Replay Cue.
```

---

# 5. AI Art/Asset Agent Prompt

```txt
Create polished low-poly / stylized asset direction for Silent Sonata.
Focus on a dreamlike coma room, broken grand piano, three interactive musical lights, sheet music fragments, memory particles, and elegant corruption cracks.
The style is clean, melancholic, magical, intimate, and readable.
Do not make the scene horror. Do not over-clutter. Gameplay objects must remain readable.
```

---

# 6. AI Audio Agent Prompt

```txt
Design a soft, non-frustrating Web Audio placeholder sound set for Silent Sonata.
Create three object identities:
Blue Orb = low warm felt piano,
Rose Crystal = mid celesta,
Gold Prism = high glass chime.
Wrong feedback should be muted piano + sheet flutter, not harsh.
Correct feedback should be warm piano chord + memory chime.
```

---

# 7. Definition of Done — Prologue

- [ ] 5 fragments implemented.
- [ ] 3 notes restored.
- [ ] Player can identify left/mid/right.
- [ ] Wrong SFX comfort target met.
- [ ] Correct reward feels satisfying.
- [ ] Settings work.
- [ ] QA metrics logged.
- [ ] Build playable for testing.
