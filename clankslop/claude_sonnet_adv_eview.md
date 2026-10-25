# Point-and-Click Adventure Games: Design Principles, the Canon, and Why the Best Succeeded

*Research write-up, compiled October 2026 from web sources (see [Sources](#sources)). Claims are marked **[sourced]** when taken from a cited page, and **[synthesis]** when they are my own interpretation. Sales figures from the 1990s are patchy and sometimes contradictory; treat them as orders of magnitude.*

## Contents

1. [Short version](#1-short-version)
2. [General game design principles, and how they map onto adventure games](#2-general-game-design-principles-and-how-they-map-onto-adventure-games)
3. [Principles that are special to (or much stronger in) point-and-click adventures](#3-principles-that-are-special-to-or-much-stronger-in-point-and-click-adventures)
4. [The canon: consistently top-rated classic and classic-retro games](#4-the-canon-consistently-top-rated-classic-and-classic-retro-games)
5. [What made the most successful games successful](#5-what-made-the-most-successful-games-successful)
6. [Does the success analysis agree with the theory?](#6-does-the-success-analysis-agree-with-the-theory)
7. [Practical checklist](#7-practical-checklist)
8. [Sources](#sources)

---

## 1. Short version

- Most general design theory (flow, clear goals, feedback, "interesting decisions", MDA) still applies to adventures. Several parts are **inverted or switched off**: challenge by execution skill, balancing, mastery curves, replayability and emergent dynamics.
- Adventure games are **authored-content games**. Their "mechanics" are thin (click, combine, talk). The fun comes from *aesthetics* in MDA terms: **narrative, discovery, humour, fantasy and expression**. The design problem is therefore less "make the loop engaging" and more "keep the player in the fiction while they think."
- The central adventure-specific ideas are:
  - **fairness of puzzle logic** (no moon logic, no dead ends, no forced death);
  - **clear goals and sub-goals**;
  - **non-linear puzzle structure** (Gilbert's dependency charts, "cages vs. options");
  - **hotspot and verb economy**;
  - **writing, character and voice as the primary content**;
  - **pacing and length**.
- Across the canon, the games rated best and remembered longest combine **a strong, distinctive world and voice** with **puzzles that are fair enough not to break immersion**. Puzzle cleverness alone does not do it.
- **Critical acclaim and commercial success are different stories.**
  - Myst, a game that deliberately breaks the "adventure game rules", sold the most by a wide margin.
  - Sierra's harsher games outsold LucasArts' fairer ones for years.
  - Grim Fandango topped the critics' list and is widely described as a commercial disappointment.
  - Timing, platform and audience reach matter as much as design quality.

---

## 2. General game design principles, and how they map onto adventure games

### 2.1 Gathered principles (generic)

| # | Principle | One-line meaning |
|---|-----------|------------------|
| G1 | **Core loop** | Repeatable cycle of act → feedback → reward → new goal. |
| G2 | **Flow / challenge-skill balance** (Csikszentmihalyi) | Clear goals, immediate feedback, challenge matched to ability. |
| G3 | **Interesting decisions** (Sid Meier) | A game is a series of meaningful choices. |
| G4 | **Player agency** | Actions visibly matter. |
| G5 | **Feedback and legibility** | The game communicates cause and effect. |
| G6 | **MDA** (Mechanics → Dynamics → Aesthetics) | Designers write mechanics, but players experience aesthetics. |
| G7 | **Lenses / playtest-driven iteration** (Schell) | Look at the design from many angles. Playtest. |
| G8 | **Onboarding and learning curve** | Teach in isolation, then combine. |
| G9 | **Pacing / tension and release** | Rhythm of intensity and rest. |
| G10 | **Reward schedule and progress visibility** | Players need to feel they are advancing. |
| G11 | **Replayability, emergence, systemic depth** | Rules that generate varied play. |
| G12 | **Balance and fairness** | Difficulty is the player's to overcome, not the game's to inflict arbitrarily. |

Sources for G1–G7: the Game Developer / Medium / MDA summaries listed below. G8–G12 are common textbook material and are not tied to one source.

### 2.2 What carries over, what is weakened, what doesn't apply

| Principle | Applies to point-and-click? | Notes |
|-----------|-----------------------------|-------|
| **G1 Core loop** | **Applies, but reshaped.** | The loop is *observe → hypothesise → try → get a (funny or revealing) response → new information/location*. There is no "grind" loop. The *response text/animation* is the reward. |
| **G2 Flow** | **Applies, in a different form.** | Flow comes from *thinking*, not reflexes. It breaks when the player is stuck with no leads. Gilbert's essay frames suspension of disbelief as the thing to protect, and each reload or head-bang breaks it. |
| **G3 Interesting decisions** | **Weak.** | Most "decisions" are *what to try*, not *what to choose*. Choice appears in dialogue, in order of attack, and in multi-solution games such as Fate of Atlantis (Team/Wits/Fists paths) and Maniac Mansion (character choice). Choice-heavy modern narrative games bring more of G3 in. |
| **G4 Agency** | **Applies, but is mostly agency over discovery/pace.** | The player rarely changes the plot. They change *when and in what order* the story is revealed. Gilbert: "the player doesn't always do what the designer intended." |
| **G5 Feedback** | **Applies strongly.** | Every hotspot should answer. Default "I can't do that" lines are where LucasArts-style games put humour and personality. |
| **G6 MDA** | **Applies, and highlights a difference.** | Mechanics are minimal. Dynamics are small (inventory combinatorics). The aesthetics that matter are *narrative, fantasy, discovery, humour, expression*, not challenge or competition. |
| **G7 Playtesting** | **Applies strongly, and is the key defence against designer blindness.** | Gilbert: "It's very easy when designing to become blind to what the player doesn't know about your story." |
| **G8 Onboarding** | **Applies.** | Gilbert's "first sub-goal must be obvious" rule is onboarding. Chapter structure and bottlenecks act as learning gates. |
| **G9 Pacing** | **Applies, but the "tension" instrument is different.** | Pacing is set by puzzle dependency shape, location reveals and story beats, not by combat intensity. Real-time pressure is mostly disliked here (see 3.5). |
| **G10 Progress visibility** | **Applies strongly.** | Gilbert's "incremental reward": a new area, character or plot beat should arrive regularly. |
| **G11 Replayability / emergence** | **Mostly does not apply.** | Content is authored and consumed once. Replay value is in rediscovering jokes, alternate paths (Fate of Atlantis) or different solutions (Maniac Mansion). This is why price per hour and game length become design issues (see 3.9). |
| **G12 Balance / fairness** | **Applies, but "balance" becomes "fairness of logic".** | There are no numbers to balance, only *clue quality* and *dependency structure*. Difficulty is information difficulty, not execution difficulty. |
| Execution skill, twitch, build/tuning, economy design, multiplayer | **Do not apply** (mostly). | Action sequences have been repeatedly criticised in adventure games. Gilbert argues the player should be rewarded for "thinking and figuring, rather than quick reflexes". |

**[synthesis]** The reason so much theory applies "weakly" is that adventures are **content-driven**. Their quality is concentrated in writing, art, audio, character, puzzle ideas and the *information architecture* around them, not in systems that generate depth by themselves.

---

## 3. Principles that are special to (or much stronger in) point-and-click adventures

### 3.1 Gilbert's rules of thumb (the founding document)

Ron Gilbert wrote "Why Adventure Games Suck (And What We Can Do About It)" in 1989 while designing *Monkey Island*. In a later preface he says he no longer agrees with everything in it. The rules, paraphrased **[sourced: Grumpy Gamer]**:

1. **End objective must be clear** (it may change mid-game, but the player should know what they are doing at the start).
2. **Sub-goals must be obvious**, at least the first one. Gilbert cites Ben Kenobi laying out Luke's journey in the first twenty minutes of *Star Wars*.
3. **Live and learn**: a careful and observant player should be able to finish without dying or relying on saves. Danger is fine if it is survivable by being clever.
4. **No backwards puzzles**: the *problem* should be found before the *solution* (see the crevice before the rope).
5. **"I forgot to pick it up"**: never make an unrecoverable, seemingly insignificant item mandatory. Either give it an earlier use that guarantees pickup, or hint at it.
6. **Puzzles should advance the story** and be clearly connected to the immediate goal.
7. **Real time is bad drama**: use "Hollywood time". Wait until the hat is grabbed, then slam the door.
8. **Incremental reward**: the player must feel they are achieving something.
9. **No arbitrary puzzles**: they don't have to be obvious, just make sense. The target reaction is "Of course, why didn't I think of that?" and the failure reaction is "I never would have gotten that!"
10. **Reward intent**: if the player is clearly trying to do the thing the game wants, let it work. Avoid "second guess the parser" meta-games, and be generous with proximity and synonyms.
11. **No unconnected events**: when something unlocks a new area, there must be a reason it does.
12. **Give the player options (uncage the game)**: avoid sequences of small cages, each with the only key. Let the player choose from many puzzles, so being stuck on one doesn't stop the game.
13. **Meta**: Gilbert wishes games had no save-game dependency, and shorter, denser games (about four to five hours) at lower prices, with no padding puzzles.

### 3.2 Puzzle Dependency Charts: non-linearity as a design tool

**[sourced: Grumpy Gamer]** Gilbert's other major contribution is the *Puzzle Dependency Chart* (PDC), used for every aspect of puzzle design on *Monkey Island*.

- A PDC is a graph of puzzles and puzzle steps, where each node points to what must be done before it. It is *not* a flowchart. Flowcharts are for solving a game, PDCs are for designing one.
- Design **backwards from the end of puzzle chains**, e.g. "player needs to get into the basement", not "where do I hide a key?".
- A healthy chart shows **diamond-shaped expansion and contraction**. Solving one puzzle opens two or three, which later collapse to a single bottleneck.
- Too linear is bad ("nothing worse"), and too unwieldy with choice is also bad.
- Design in **acts** with bottlenecks between them. This gives the player a sense of completion and lets you cull inventory.
- Gilbert admits *Maniac Mansion* had no PDCs and "it really shows": dead-end puzzles, uneven flow, bottlenecks.

### 3.3 Fairness of logic: moon logic, designer logic and clue quality

- **Moon logic** is a puzzle whose solution only makes sense by guessing the designer's mind. The classic counter-example is Gabriel Knight 3's "cat hair mustache" sequence, famously used by Jonathan Blow in his *Design Reboot* talk **[sourced via search summaries; I did not watch the talk]**.
- Blow's critique of the genre, as summarised by the sources, is that good puzzles communicate intent clearly, respect the player's intelligence, and give a payoff proportional to effort. Several sources add that logic should arise from consistent systems or world rules, not arbitrary associations.
- **Inventory puzzles** are lock-and-key puzzles. Done badly they degrade into "use every item on every hotspot until something happens". Done well, items hint at their use through the fiction.
- **[synthesis]** *Cartoon logic* (Monkey Island, Day of the Tentacle) is usually accepted because the *tone* tells the player the rules are loose, and the writing foreshadows the gag. It still needs to be **clued**. The test is whether the solution feels like a delighted "of course" after the fact.

### 3.4 No dead ends, no unfair death, and the Sierra/LucasArts split

- Sierra's games historically let the player die and/or become unwinnable ("walking dead") by missing an item. LucasArts removed those fail states after *Maniac Mansion*, on Gilbert's argument that reloading breaks immersion.
- Both approaches sold. In Gilbert's own words, *Monkey Island 1 and 2* "sold well, but Sierra Online and King's Quest were still kicking our ass completely" **[sourced: Wikipedia quoting Gilbert]**. The King's Quest series had sold 2.5M copies by 1994 and 7M by 1997 **[sourced: Wikipedia]**.
- **[synthesis]** "No dead ends" is a *quality-of-life* and *reputation* principle, not a sales guarantee.

### 3.5 Time pressure and "Hollywood time"

- Reaction-based sequences generally damage the adventure contract: they test a skill the player did not sign up for. Gilbert's alternative: cinematic time that keys off the player's intent, with roughly 10% of players finishing early, 10% failing, and 80% making it "just in time".
- Modern examples keep this rule by making action or timing optional or non-punishing.

### 3.6 Verbs, interface and hotspots

- Point-and-click replaced the text parser. Gilbert disliked parser guessing, so he built a verb-based point-and-click interface for *Maniac Mansion* (and the SCUMM engine) **[sourced: Wikipedia, Maniac Mansion]**.
- Core issues for the genre: **pixel hunting**, verb count, "second-guess the interface" problems, and hotspot visibility.
- **[synthesis]** The interface is the "mechanics". Cutting friction here (clear hotspots, fast walking, skippable dialogue, double-click to exit) has more effect than any "balance" work.

### 3.7 Writing, characters, humour and voice as the primary content

- Gilbert opens his essay with: "The element that brings adventure games to life for me is the stories around which they are woven."
- He is also explicit that story games are **not interactive movies**. Take what's useful from film, but find the medium's own methods. The main difference is **interaction**, and the player "doesn't always do what the designer intended."
- Several of the most-loved games are loved for tone: Monkey Island's humour, Grim Fandango's noir-in-the-land-of-the-dead, Day of the Tentacle's cartoon time travel, Full Throttle's biker mythology (well-received voice acting and soundtrack, many reviewers felt it was too short **[sourced: Wikipedia]**).

### 3.8 Information design: the "problem of amnesia", mystery structure and plot holes

- Adventure stories lean on mystery because the player starts without the protagonist's knowledge. Ernest Adams calls this the "Problem of Amnesia" **[sourced: Wikipedia, Adventure game]**.
- Gilbert's plot-hole test: **retell one complete path as a normal story**. If the character uses information they could not have learned, the plot has a hole.
- Because of this, the genre's information structure (who knows what, and when) matters as much as the puzzles.

### 3.9 Length, price, padding and hint systems

- Gilbert argues high prices push developers to pad with the worst puzzles. He wanted four-to-five-hour games.
- **[sourced: Polygon/IGN via search]** For *Return to Monkey Island* (2022), Gilbert has said that obscure puzzles were tolerable in the pre-internet era because getting stuck was expected. Now players look things up, so the game ships an in-world **hint system** and a **casual mode** (an idea already seen in *Thimbleweed Park*).
- **[synthesis]** In the walkthrough era, a puzzle's real difficulty is "how long before the player gives up and googles". Hint systems and difficulty modes address that.

### 3.10 Sub-genre differences matter

- **LucasArts-style** (inventory, dialogue, comedy, no death).
- **Sierra-style** (fail states, parser or early point-and-click, more fairy-tale/RPG hybrids such as *Quest for Glory*).
- **Puzzle-adventure / Myst-style** (first-person, little or no inventory or NPCs, environmental logic puzzles, atmosphere). These games "lack the type of inventory puzzles that typical point-and-click adventure games have" **[sourced: Wikipedia]**.
- **Narrative / Telltale-style** (choices, quick-time events, light puzzles).

Principles above need to be read per sub-genre. The inventory-puzzle fairness rules are central to LucasArts-style games and largely irrelevant to Myst-style games, where the equivalent is *environmental clue legibility*.

---

## 4. The canon: consistently top-rated classic and classic-retro games

### 4.1 How I built the list

I looked for **overlap** between: Adventure Gamers' long-standing "Top 100 All-time Adventure Games" (updated 2011, the community's best-known institutional ranking), aggregator scores, the point-and-click "best of" lists that came up in searches (TechPlayGuide, The Daily Juice, ENEBA, TheGamer, etc.), and available Wikipedia reception and sales data. Anything that appears in most lists, plus a high aggregate score or an "all-time great" label, is placed in a tier.

**Adventure Gamers' Top 20 (2011)** **[sourced: Thimbleweed Park forum post reproducing the list]**:

1. Grim Fandango
2. The Longest Journey
3. Gabriel Knight: The Beast Within
4. Broken Sword: The Shadow of the Templars
5. Riven
6. Day of the Tentacle
7. The Last Express
8. Monkey Island 2: LeChuck's Revenge
9. Tex Murphy: The Pandora Directive
10. Portal 2
11. Indiana Jones and the Fate of Atlantis
12. Zork Grand Inquisitor
13. King's Quest VI: Heir Today, Gone Tomorrow
14. The Secret of Monkey Island
15. Syberia
16. Gabriel Knight: Sins of the Fathers
17. Machinarium
18. Myst
19. Beneath a Steel Sky
20. Still Life

Note the difference between **expert/community ranking** (AG puts Monkey Island 1 at 14 and Grim Fandango at 1) and **popular memory** (Monkey Island 1 is nearly always the first game named).

### 4.2 Consensus tiers

**Tier 1: appears on nearly every list; widely called "best ever" or "genre-defining"**

| Game | Year | Studio | Notes |
|------|------|--------|-------|
| The Secret of Monkey Island | 1990 | Lucasfilm Games | The popular "gold standard". Humour, insult sword-fighting, no-death design. AG rank 14. |
| Monkey Island 2: LeChuck's Revenge | 1991 | LucasArts | Critics' favourite of the first two (e.g. 95–96% from magazines **[sourced: Wikipedia]**). AG rank 8. |
| Day of the Tentacle | 1993 | LucasArts | Three-timeline puzzle structure. AG rank 6. Remastered scored 87 on Metacritic **[sourced: Wikipedia]**. |
| Grim Fandango | 1998 | LucasArts | AG rank 1. Metacritic 94 **[sourced: Wikipedia]**. |
| Indiana Jones and the Fate of Atlantis | 1992 | LucasArts | Three paths (Team/Wits/Fists). Over 1M units, LucasArts' best-selling adventure by 2009. 30% female audience (Falstein) **[sourced: Wikipedia]**. AG rank 11. |
| Broken Sword: Shadow of the Templars | 1996 | Revolution | AG rank 4. 825k copies by 2000 **[sourced: Wikipedia]**. |
| Myst | 1993 | Cyan | Best-selling PC game for nearly a decade, 6M+ copies **[sourced: Wikipedia]**. AG rank 18. |

**Tier 2: very frequently listed; strong critical standing**

| Game | Year | Studio | Notes |
|------|------|--------|-------|
| Sam & Max Hit the Road | 1993 | LucasArts | ~84% GameRankings **[sourced: Wikipedia]**. Offbeat-humour fan favourite. |
| Full Throttle | 1995 | LucasArts | Over 1M units, the first LucasArts adventure past that mark **[sourced: Wikipedia]**. Often called short. |
| Gabriel Knight: Sins of the Fathers / The Beast Within | 1993 / 1995 | Sierra | AG ranks 16 and 3. Mature storytelling. (GK3 gave the genre the "cat hair mustache".) |
| King's Quest VI | 1992 | Sierra | AG rank 13. Often named Sierra's peak. |
| Beneath a Steel Sky | 1994 | Revolution | AG rank 19. |
| The Longest Journey | 1999 | Funcom | AG rank 2. |
| Maniac Mansion | 1987 | Lucasfilm Games | The founding "SCUMM" point-and-click. Flawed (dead ends), foundational. |
| Riven | 1997 | Cyan | AG rank 5. |
| The Last Express | 1997 | Smoking Car | AG rank 7. |

**Tier 3: frequently mentioned honourable mentions**

Loom, The Curse of Monkey Island (1997), Zork Grand Inquisitor, Syberia, Machinarium, Tex Murphy: The Pandora Directive, Still Life, and Quest for Glory (the adventure/RPG hybrid).

**Modern "classic-retro" entries that belong in the conversation**

- *Thimbleweed Park* (Gilbert/Winnick, 2017), a deliberate retro-style return with a casual mode.
- *Return to Monkey Island* (2022): "generally favorable" on Metacritic **[sourced]**. About ~100k units and ~$3M in its first month on Steam, per one secondary report (GameSensor via Wikipedia) **[sourced, low confidence]**.
- *Machinarium* (2009), already in AG's top 20.

### 4.3 Caveats on the data

- The search summaries I used for the popular lists are AI-generated digests of third-party pages. I only trusted facts that I could also confirm in a primary-ish source (Gilbert's essay, Wikipedia, the AG list).
- Aggregator scores for 1990s games are often retrospective and sparse (Metacritic did not exist for most of them).
- Sales numbers conflict between sources. For example, Edge reports Day of the Tentacle at roughly 80,000 copies by 2009 **[sourced: Wikipedia]**, which looks low and probably reflects an incomplete count. For Grim Fandango I found figures from ~100k to ~500k in various places and a confirmed *debut at #6 on PC Data's charts, then absent the next week* **[sourced: Wikipedia]**, so I describe it only as "widely considered a commercial disappointment".
- Nostalgia and survivorship bias are strong. Games that were poorly designed but are less remembered don't appear on any list.

---

## 5. What made the most successful games successful

I separate **critical/enduring success** (what appears on the lists above) from **commercial success** (what sold). They overlap only partly.

### 5.1 Case notes

**The Secret of Monkey Island / Monkey Island 2**
- Distinctive comic voice and a lovable, underdog protagonist.
- Insult sword-fighting is a genre-appropriate *non-twitch* "combat", turning a danger scene into a wits puzzle.
- No death and no dead ends, with a design built on PDCs, so the player can pursue several leads at once.
- Clear opening goal (become a pirate) and clear sub-goals.
- Commercial note: sold well, but did not beat Sierra at the time **[sourced]**. The reputation grew over years.

**Day of the Tentacle**
- A single high-concept structure: three characters in three time periods whose puzzles interlock (changes in the past appear in the future). **[synthesis from common knowledge]**
- Strong cartoon art direction and voice.
- Parallel puzzle strands naturally "uncage" the player (Gilbert's rule 12).
- Commercial note: acclaimed, moderate sales **[sourced]**.

**Grim Fandango**
- Unique setting and art direction (Mexican Day of the Dead plus film noir) praised especially by critics **[sourced]**.
- It ranks #1 in the AG list and had Metacritic 94 **[sourced]**.
- Commercially disappointing in 1998. Context: the genre was in decline as first-person shooters rose to dominate the market **[sourced: Wikipedia, Adventure game]** and LucasArts' later adventure output dwindled.
- **[synthesis]** Shows that quality of writing and art can sustain a game's legacy for decades, but cannot change a market shift by itself.

**Indiana Jones and the Fate of Atlantis**
- A beloved licence, three selectable routes (Team, Wits, Fists) for replay value, and a broader audience (30% female per Falstein) **[sourced]**.
- Over 1M units, LucasArts' best-selling adventure for years.
- **[synthesis]** Licence plus an accessible, *genuinely multiple-path* design is a rare combination of market reach and design generosity.

**Full Throttle**
- Over 1M units, versus a typical LucasArts adventure target of ~100k at the time **[sourced]**. Strong voice acting, music and animation, with a strong stylistic identity. Often criticised as short.

**Broken Sword: Shadow of the Templars**
- Cinematic thriller/mystery with a global-conspiracy story, historic detail and a strong character duo. 825k copies by 2000, with a notably strong PlayStation performance **[sourced]**. Evidence that a serious tone and a console port can expand the audience.

**Myst**
- Broke the "adventure-game rules" on purpose: no inventory, no death, no NPCs, no dialogue trees. Slow, solitary exploration.
- Sold 6M+ and was the best-selling PC game for nearly a decade **[sourced]**. Retailers reportedly sold CD-ROM drives on the back of it **[sourced via search, treat as anecdotal]**.
- It attracted a non-gamer audience. Its design principles (no fail state, wonder, atmosphere) are similar to Gilbert's immersion argument, but its *means* are different.

**King's Quest series (Sierra)**
- 2.5M copies by 1994 and 7M by 1997 **[sourced]**. Fairy-tale breadth, wide marketing and an enormous catalogue. Sierra's harsher fail states did not stop the series from selling.

**Return to Monkey Island / Thimbleweed Park**
- Show a *modernised* version of the same contract: a hint system, casual mode, and fewer opaque puzzle chains, with the original comic voice intact **[sourced: Polygon/IGN via search]**.

### 5.2 Recurring success factors (cross-game)

| Factor | Games where it's evident | Evidence level |
|--------|--------------------------|----------------|
| **Distinctive world and tone** (a single strong aesthetic idea) | Monkey Island, Grim Fandango, DOTT, Full Throttle, Myst | Strong (critical consensus) |
| **Writing, humour and character voice** | LucasArts catalogue, Broken Sword | Strong |
| **Puzzles that are fair enough** (no forced death, few dead ends, clear goals) | LucasArts catalogue (by design), Myst (by omission) | Moderate. Fair play is widely praised but not a *sales* predictor. |
| **Non-linear puzzle structure** (parallel leads) | Monkey Island, DOTT, Fate of Atlantis | Moderate (Gilbert's own account) |
| **Audio-visual showcase for the platform of the day** | Myst (CD-ROM), Grim Fandango (3D), Full Throttle (voice acting) | Strong for sales |
| **Broader audience reach** (non-gamers, women, console ports, licences) | Myst, Fate of Atlantis, Broken Sword (PlayStation) | Strong for sales |
| **Right place in the market cycle** | Pre-1998 releases vs. Grim Fandango | Strong for sales |
| **Incremental reward and obvious goals** | Gilbert's rules; seen in all the best | Moderate |
| **Replay hooks** (alternate paths) | Fate of Atlantis, Maniac Mansion | Weak-to-moderate |

### 5.3 Where the successful games are *not* alike

- **Death/dead ends**: LucasArts avoids them, Sierra includes them, Myst removes the idea. All three have fans.
- **Puzzle style**: inventory combos (LucasArts), environmental logic puzzles (Myst/Riven), mixed (Broken Sword).
- **Tone**: comedy (Monkey Island, DOTT), noir (Grim Fandango, Broken Sword), mythic exploration (Myst).
- **Perspective and interface**: third-person verb UI vs. first-person click navigation.

So a single "recipe" does not exist. What is shared is **a strong identity** plus **respect for the player's time and intelligence in the specific contract each game sets up**.

---

## 6. Does the success analysis agree with the theory?

| Theory claim (from §2–3) | Evidence from the successful games | Verdict |
|--------------------------|-------------------------------------|---------|
| **Fairness and no-frustration protect immersion** (Gilbert) | The LucasArts catalogue is remembered as fair and warm, and appears at the top of nearly every list. Myst is fair by construction. Gabriel Knight 3's moon logic is the genre's standard cautionary tale. | **Supports**, for *critical reputation and long-term affection*. |
| **...and that translates into sales** | Sierra's harsher games sold more for years. Gilbert himself said so. | **Does not support** as a sales driver. Fair design is necessary for a lasting reputation, not sufficient for sales. |
| **Aesthetics (narrative, humour, fantasy) are the real "mechanic"** (MDA reading) | Every top-tier game has a strong, singular voice. | **Strongly supports.** |
| **Non-linear dependency structure (uncaging)** | Monkey Island, DOTT, Fate of Atlantis are the ones people praise for structure. | **Supports**, though it is hard to disentangle from other qualities of these games. |
| **Clear goals/sub-goals and incremental reward** | The best games open with a crisp objective. Genre-rejection stories come from "wandering around not knowing what to do". | **Supports** (qualitative). |
| **Interesting decisions / agency / replayability** | Fate of Atlantis is the main clear case, and its sales were strong. Most other classics are single-path. | **Mostly neutral.** The genre succeeds without much G3/G11. |
| **No real-time pressure** | The canon is overwhelmingly untimed. | **Supports.** |
| **Short, dense games** (Gilbert's 4–5 hours) | Full Throttle's shortness is a recurring complaint. Myst is a long, slow burn. Many classics are 8–15 hours. | **Mixed.** Gilbert's own advice does not obviously match what sold best. Quality-per-minute still seems to matter. |
| **Hint systems / modern accessibility** | *Return to Monkey Island* and *Thimbleweed Park* adopted them and were received well. | **Supports**, though the evidence is recent and modest. |
| **Play on the platform's strengths** (not in the design theory above) | Myst/CD-ROM, Grim Fandango/3D, Full Throttle/voice. | **New factor**: commercial success also depends on *technology showcase* and *timing*. |

### 6.1 Take-aways

1. **Design principles predict "loved and remembered", not "sold".** The principles in §3 (fairness, clarity, structure) are good predictors of a game's *critical and enduring* standing. Sales are predicted better by audience reach, timing and platform effects.
2. **Identity beats mechanics.** All the theory about loops and decisions is secondary to *what the world feels like and what the writing is like*, which in turn depends on a team with a strong voice (Gilbert/Schafer/Grossman at LucasArts, Rand and Robyn Miller at Cyan).
3. **The rules are a floor, not a ceiling.** Following Gilbert's rules avoids the common ways adventure games annoy people. It doesn't make a game great. Myst shows that you can break the standard rules, if you replace them with a coherent alternative contract.
4. **The contract must be consistent.** Games get criticised when they violate their own implied logic (moon logic), when they hide the next goal, or when they punish the player for something they were not told.
5. **Players now have a search engine.** The modern designer's equivalent of "no dead ends" is "no unrecoverable stuckness": hints, difficulty options and clear logging of goals.

### 6.2 Limits of this analysis

- Most evidence is retrospective and qualitative. There is no controlled comparison, and I could not find reliable per-title sales for many classics.
- Some secondary claims (for example from AI-generated search summaries) were not independently verified and are flagged above.
- "Best" lists inherit the taste of their voters, who skew towards experienced adventure fans.

---

## 7. Practical checklist

Derived from the above, for anyone designing a classic-style point-and-click (including this repo's act-based design, whose `act*.puml` files are already a natural place for dependency charts):

**Structure**
- [ ] Draw a **puzzle dependency chart** per act. Work backwards from the end of the puzzle chains. Check for diamond shapes: not too linear, not too open.
- [ ] End each act with a deliberate bottleneck, and use it to prune inventory.
- [ ] Make sure the player always has more than one open lead (no cages).

**Clarity**
- [ ] State the **end objective** early. Give the **first sub-goal** in-fiction.
- [ ] Every puzzle: *problem seen before solution*; *a clue exists in the fiction*; *the solution is sensible in hindsight*.
- [ ] No mandatory one-time-only pickups without an earlier guaranteed use or hint.
- [ ] Provide an in-game goal log, or hint system and/or difficulty option.

**Fail states**
- [ ] No unwinnable state without warning. If danger exists, it should be survivable by being clever.
- [ ] No reflex sequences. If there is a timed scene, use Hollywood time or make it skippable.

**Content**
- [ ] A distinctive voice that shows in even the *failure* lines ("I can't do that").
- [ ] A regular incremental reward: a new area, character, joke or plot reveal.
- [ ] Playtest with someone who has not read the design doc. Retell a full path as a story to find plot holes.

**Scope**
- [ ] Prefer a shorter, denser game over padding. Cut puzzles that only slow the player down.
- [ ] Decide on audience reach and platform early. Quality of design alone does not guarantee sales.

---

## Sources

**Primary or near-primary**
- Ron Gilbert, *Why Adventure Games Suck and What We Can Do About It* (1989, republished with 2004 preface): <https://grumpygamer.com/why_adventure_games_suck/>
- Ron Gilbert, *Puzzle Dependency Charts*: <https://grumpygamer.com/puzzle_dependency_charts/>
- Adventure Gamers Top 100 Adventure Games (2011), top 20 as reproduced in the Thimbleweed Park forum: <https://forums.thimbleweedpark.com/t/top-100-all-time-adventure-games/1425>

**Reference pages (Wikipedia, via API)**
- Grim Fandango, Myst, Day of the Tentacle, Monkey Island 2: LeChuck's Revenge, Broken Sword: The Shadow of the Templars, Indiana Jones and the Fate of Atlantis, Full Throttle (1995), Sam & Max Hit the Road, Return to Monkey Island, King's Quest, Maniac Mansion, Adventure game.

**Search-assisted summaries (secondary; used for orientation, verified where noted above)**
- General principles: Game Developer / Medium *Game Design Frameworks and Principles*, *gamedesign.gg Core Loops*, MDA framework (Wikipedia).
- Puzzle design: *A Study Into Puzzle Design* (Game Developer), *Adventure Game Designer's Handbook* (GitHub, brycecovert), NYU Game Center on Jonathan Blow, Blow's *Design Reboot* talk (YouTube, not watched by me).
- Lists: TechPlayGuide, The Daily Juice, ENEBA, TheGamer "point and click" best-of lists.
- Myst context: Strong National Museum of Play, GOG blog, Den of Geek.
- Sierra vs. LucasArts: PopMatters, bestdosgames, Adventure Gamers forums.
- Return to Monkey Island design: Polygon and IGN coverage of the hint system and casual mode.
