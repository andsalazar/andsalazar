# Hi, I'm Andy Salazar 👋

I build at the edge of what AI-assisted development can actually **ship** — probing how far modern tools can take an ambitious idea across very different domains, then turning the ones that work into real products.

That curiosity has run from **quantitative pipelines** → **original research** → a **production consumer app** → a **playable game** → a **one-shot AI film studio** — with a few deliberate dead ends along the way that taught me where the frontier really is.

## 🚀 Field Notes — Study Guide · *live on the App Store*

A physics app that **rebuilds quantum field theory from a mass on a spring** — 38 interactive concepts, each with a live simulation backed by unit-tested physics and a source-grounded AI tutor. Native iOS + Android (React Native / Expo) and a Next.js web app sharing one tested physics core.

- 📱 App Store: https://apps.apple.com/us/app/field-notes-study-guide/id6792985711
- 🌐 Website: https://fieldnotestudy.guide
- 💻 Showcase: https://github.com/andsalazar/field-notes-showcase

## 🎬 Torn Pages — one-shot AI films from public-domain stories · *Live*

Pick a passage from Project Gutenberg and come back to a finished short film. A **director made of code and models** casts the text, writes a treatment, plans the shots, films them, checks its own takes, then scores and masters the film — with nobody approving anything by hand. Every film's page publishes the full record of what the director decided. A Python engine in **Docker**, a static site with standard-library functions on **Vercel + Supabase**, and social cuts rendered and posted by code.

- 🎞️ Watch the films: https://www.tornpages.app
- ▶️ YouTube: https://www.youtube.com/@officialtornpages
- 💻 Showcase: https://github.com/andsalazar/tornpages-showcase

## ⚔️ ASCENDANT — browser-playable action RPG demo

An isekai action RPG where power is **debt**: skills and gear are loans, interest accrues, and when you can't pay, the Ledger repossesses your memories. Built from scratch in **Babylon.js + TypeScript** — no engine, no editor — with ~2,700 unit tests, a reachability gate that fails the build when code is never called from the running game, and a harness that plays the whole demo in headless Chrome with real mouse and key events.

- 🎮 Play in the browser: https://ascendant-rosy.vercel.app
- 💻 Showcase: https://github.com/andsalazar/ascendant-demo

## 🔬 Weight-Space Programming — a replication, and what didn't extend

Can one model **read another model's weights**, and can a tiny adapter make a large video model faster? Two published claims, tested on rented GPUs. **One repeated:** given the 23,824 raw weights of a small diffusion model and no tools, GPT-6 Astra named what the model draws — on the paper's networks, on fresh ones trained for the test, and on a shape the paper never used — and declined to guess on a shuffled control. Four cheaper models could not. **One didn't extend:** a 313k-parameter adapter on **Ovi**, an 11.66B video + audio model, was no faster at equal quality across 210 clips. Designs and scoring rules were pushed **before** the runs, the quoted numbers are recomputed from committed evidence by the test suite, and every early result that failed re-measurement is still in the repo with a correction banner.

- 💻 Repo: https://github.com/andsalazar/model-training
- 📄 Reading weights: https://github.com/andsalazar/model-training/blob/main/docs/stage8-reading-weights.md
- 📄 The adapter result: https://github.com/andsalazar/model-training/blob/main/docs/stage7-v4-decide.md

## 🧪 Other work & experiments

- **Quant trading pipeline** — the quantitative project that kicked off this whole build arc. [repo →](https://github.com/andsalazar/quant-trading-pipeline)
- **AI-assisted economics paper** — an experiment to see how close an LLM-driven workflow could get to a genuinely *publishable* research paper. The result is a working paper on U.S. federal budget analysis, posted on SSRN. [📄 SSRN](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6285038) · [repo](https://github.com/andsalazar/FederalBudgetAnalysis)
- **Generative explorations (paused):** full album music generation — parked when the tooling wasn't yet good enough to clear the bar. Episodic animation was parked for the same reason and came back as Torn Pages.

## 🛠️ Tools I reach for

`TypeScript` · `React / React Native (Expo)` · `Next.js` · `Babylon.js` · `Node` · `Supabase / Postgres` · `Python` · `Docker` · `FFmpeg` · LLM tooling (`Claude`, `Gemini`, `DeepSeek`, `OpenRouter`) · `RunPod` · `Doppler` · evaluation harnesses & testing

## 📫 Elsewhere

- Field Notes: https://fieldnotestudy.guide
- Torn Pages: https://www.tornpages.app
- Portfolio: https://salazar-andy.com
