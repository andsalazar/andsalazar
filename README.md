# Hi, I'm Andy Salazar 👋

I build at the edge of what AI-assisted development can actually **ship** — probing how far modern tools can take an ambitious idea across very different domains, then turning the ones that work into real products.

That curiosity has run from **quantitative pipelines** → **original research** → a **production consumer app** → a **released album** → a **playable game** → a **one-shot AI film studio** — with a few deliberate dead ends along the way that taught me where the frontier really is.

## 🚀 Field Notes — Study Guide · *live on the App Store*

A physics app that **rebuilds quantum field theory from a mass on a spring** — 38 interactive concepts, each with a live simulation backed by unit-tested physics and a source-grounded AI tutor. Native iOS + Android (React Native / Expo) and a Next.js web app sharing one tested physics core.

- 📱 App Store: https://apps.apple.com/us/app/field-notes-study-guide/id6792985711
- 🌐 Website: https://fieldnotestudy.guide
- 💻 Showcase: https://github.com/andsalazar/field-notes-showcase

## 🔬 Weight-Space Programming — a replication, and what didn't extend

Can one model **read another model's weights**, and can a tiny adapter make a large video model faster? Two published claims, tested on rented GPUs. **One repeated:** given the 23,824 raw weights of a small diffusion model and no tools, GPT-6 Astra named what the model draws — on the paper's networks, on fresh ones trained for the test, and on a shape the paper never used — and declined to guess on a shuffled control. Four cheaper models could not. **One didn't extend:** a 313k-parameter adapter on **Ovi**, an 11.66B video + audio model, was no faster at equal quality across 210 clips. Designs and scoring rules were pushed **before** the runs, the quoted numbers are recomputed from committed evidence by the test suite, and every early result that failed re-measurement is still in the repo with a correction banner.

- 💻 Repo: https://github.com/andsalazar/model-training
- 📄 Reading weights: https://github.com/andsalazar/model-training/blob/main/docs/stage8-reading-weights.md
- 📄 The adapter result: https://github.com/andsalazar/model-training/blob/main/docs/stage7-v4-decide.md

## 📉 Quant rebuild — a trading system rebuilt to catch its own mistakes · *paper trading*

My first trading pipeline had an excellent backtest that was **wrong**: a date bug had taught the model the day of the week, and it lost money live. The rebuild is designed so a result like that can't pass quietly — data checks that gate every trade, a **locked holdout used once**, every trial counted, and paper trading compared with its own backtest every day. It is built by a team of AI agents with a read-only reviewer and a guard that keeps them away from the real account. So far **nothing has beaten buying and holding SPY**, and the write-up says so.

- 💻 Showcase: https://github.com/andsalazar/quant-rebuild-showcase

## 📄 Research papers — three working papers on SSRN · *not peer reviewed*

Three working papers, each posted to SSRN as a preprint. None is peer reviewed.

**Economics · March 2026**

- **The Distributional Consequences of Federal Fiscal Policy, FY2000–FY2025: A Quarter-Century of Structural Shift and the 2025 Inflection Point** — an experiment to see how close an LLM-driven workflow could get to a genuinely *publishable* research paper. The result is a distributional analysis of 26 fiscal years of U.S. federal budget data, using structural-break tests to separate long-run trends from genuine policy discontinuities, with an open replication package. [📄 SSRN](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6285038) · [repo](https://github.com/andsalazar/FederalBudgetAnalysis)

**Physics · September 2026**

Two papers on one question in pilot-wave theory: if a particle is modeled as a localized lump of a nonlinear wave, what makes that lump travel at the velocity its pilot wave assigns? Researched and written with AI tools under my direction; the questions, direction and final judgment are mine.

- **Guidance Selection in Localized-Wave Theories: State-space Criteria and the Asymptotics of Phase Locking** — the theory. Being localized does not by itself select that velocity. The paper sets out what else a model must supply and analyzes phase locking as one way to supply it. [📄 SSRN](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=7418038)
- **Dynamical velocity selection by a zeroth-order phase lock: numerical tests in one dimension** — the test. In one-dimensional simulations a phase-locked soliton does settle onto the pilot wave's velocity, within a limited range of detuning. The exactly matched case usually taken as the definition of phase harmony sits at the edge of that range, where the carrier is not captured, and the fully variational form of the lock selects no velocity at all. [📄 SSRN](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=7452178)

## 🛰️ The Entity — a voice AI that answers for my portfolio · *private, access on request*

My portfolio has an AI presence on it: a shader orb that follows the cursor, answers questions about my work and speaks its answers. It can say **only what is written in one record I maintain**, and it says so when the answer isn't there. A **61-question gate** runs before every deploy (grounding, privacy, refusals, prompt injection), a guard on the reply stream blocks prompt leaks, and the site sits behind expiring per-recipient access codes. Measuring where the lag was cut the time to the first spoken word from **2.9s to 1.2s**, and the write-up lists what didn't help as well as what did.

- 💻 Showcase: https://github.com/andsalazar/portfolio-AI-entity-showcase
- 🔒 Site (access code on request): https://salazar-andy.com

## 🎬 Torn Pages — one-shot AI films from public-domain stories · *Live*

Pick a passage from Project Gutenberg and come back to a finished short film. A **director made of code and models** casts the text, writes a treatment, plans the shots, films them, checks its own takes, then scores and masters the film — with nobody approving anything by hand. Every film's page publishes the full record of what the director decided. A Python engine in **Docker**, a static site with standard-library functions on **Vercel + Supabase**, and social cuts rendered and posted by code.

- 🎞️ Watch the films: https://www.tornpages.app
- ▶️ YouTube: https://www.youtube.com/@officialtornpages
- 💻 Showcase: https://github.com/andsalazar/tornpages-showcase

## ⚔️ ASCENDANT — browser-playable action RPG demo

An isekai action RPG where power is **debt**: skills and gear are loans, interest accrues, and when you can't pay, the Ledger repossesses your memories. Built from scratch in **Babylon.js + TypeScript** — no engine, no editor — with ~2,700 unit tests, a reachability gate that fails the build when code is never called from the running game, and a harness that plays the whole demo in headless Chrome with real mouse and key events.

- 🎮 Play in the browser: https://ascendant-rosy.vercel.app
- 💻 Showcase: https://github.com/andsalazar/ascendant-demo

## 🎸 The Commons Machine — a 13-track concept album · *live on streaming*

A concept album released as **American Horse Pirate**: 13 tracks, 67 minutes, **one labor fight per song**, from the 1877 railroad strike to the AI era. It shipped on the **third design**. The first, a dub-punk album with a sung lead and a spoken-word narrator, was built with ElevenLabs and FFmpeg through twelve rounds of auditions and parked in July when the tracks didn't clear the bar. In September one song tested as fast punk worked, so all fourteen were rewritten with the narrator cut and the citations moved to the liner notes. The released album, re-scoped to start in 1877, was generated in **Suno**. It was made end to end with AI tools; the concept, direction and final selection are mine.

- 🎧 Spotify: https://open.spotify.com/album/0t4iJzWp6TrZTOfvFZEFEl
- 🍎 Apple Music: https://music.apple.com/us/album/the-commons-machine/6809263498
- 💻 Showcase: https://github.com/andsalazar/commons-machine-showcase

## 🧪 Other work & experiments

- **Quant trading pipeline (first attempt, archived)** — the quantitative project that kicked off this whole build arc. Its headline backtest did not hold up, and the README now opens with the correction. [repo →](https://github.com/andsalazar/quant-trading-pipeline)
- **Episodic animation (parked):** parked when the tooling wasn't yet good enough to clear the bar. It came back as Torn Pages.

## 🛠️ Tools I reach for

`TypeScript` · `React / React Native (Expo)` · `Next.js` · `Babylon.js` · `Three.js` · `Node` · `Supabase / Postgres` · `Vercel` · `Stripe / RevenueCat` · `Python` · `PyTorch` · `Hugging Face (Transformers, PEFT)` · `vLLM` · `XGBoost / LightGBM` · `Docker` · `GitHub Actions` · `FFmpeg` · LLM tooling (`Claude`, `GPT`, `Gemini`, `DeepSeek`, `OpenRouter`) · generative media (`ElevenLabs`, `Suno`, `Higgsfield`) · `RunPod` (H100 / A100 GPUs) · `Doppler` · testing (`Vitest`, `Playwright`, `pytest`) · evaluation harnesses

## 📫 Elsewhere

- Field Notes: https://fieldnotestudy.guide
- Portfolio (private, access code on request): https://salazar-andy.com
- Torn Pages: https://www.tornpages.app
- The Commons Machine: https://open.spotify.com/album/0t4iJzWp6TrZTOfvFZEFEl
