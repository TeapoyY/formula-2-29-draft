# 🏎 29-0 Formula 2 Draft

**X-0 Sports Draft #25** — Draft 5 GP2 / Formula 2 legends across 6 championship generations and try to win every sprint and feature race of the 29-race 2026 FIA Formula 2 calendar.

[▶ Play it live](https://teapoyy.github.io/formula-2-29-draft/)

## The concept

Formula 2 is F1's official feeder series, and its weekend format is unique: **every round runs two races** — a Saturday Sprint and a Sunday Feature race. The 2026 calendar has 14 rounds, and Baku was a "supersized" round with a second feature race, giving **29 races in total**.

That makes this the first X-0 variant built around a **double-header**, and it also uses the real FIA scoring tables:

| Session | Points-paying positions | P1 | P2 | P3 | P10 |
|---------|------------------------|----|----|----|-----|
| **Sprint** | top 8 | 10 | 8 | 6 | — |
| **Feature** | top 10 | 25 | 18 | 15 | 1 |

## Dataset

**84 legends × 6 eras**, every name drawn from Wikipedia's GP2 and Formula 2 championship standings tables (no invented names):

| Era | Years | Label | Anchors |
|-----|-------|-------|---------|
| 1 | 2005-2008 | GP2 | Nico Rosberg, Lewis Hamilton, Timo Glock, Giorgio Pantano |
| 2 | 2009-2012 | Feeder | Nico Hülkenberg, Pastor Maldonado, Romain Grosjean, Sergio Pérez |
| 3 | 2013-2016 | F3 Gen | Pierre Gasly, Stoffel Vandoorne, Fabio Leimer, Alexander Rossi |
| 4 | 2017-2020 | Modern | Charles Leclerc, George Russell, Nyck de Vries, Mick Schumacher |
| 5 | 2021-2023 | New Gen | Oscar Piastri, Théo Pourchaire, Jack Doohan, Liam Lawson |
| 6 | 2024-2026 | Now | Gabriel Bortoleto, Leonardo Fornaroli, Isack Hadjar, Rafael Câmara |

## Circuit types

| Type | Races | Modifier | Why |
|------|-------|----------|-----|
| `street` | 13 | −0.03 | Narrow street circuits — Melbourne, Monaco, Monaco, Baku, Madrid: high chaos |
| `barcelona` | 2 | 0.00 | High-downforce permanent circuit — neutral |
| `fast` | 14 | +0.02 | Flowing permanent circuits — Silverstone, Spa, Monza, Red Bull Ring: rewards smoothness |

Sprint sessions carry an extra −0.02 (shorter, tighter fight).

## Draft bonuses

Two independent bonuses, both capped at **6 OVR total**, so you must choose how to spend it:

- **Era synergy** — +1.5 OVR per extra driver from the same era beyond the first
- **Championship legacy** — +1.5 OVR per extra championship generation beyond the first (F2 is F1's feeder; a roster that spans generations is a class of its own)

## Difficulty

AI field is calibrated to **OVR 82-92** across a 36-car grid:

| Player OVR | Avg wins / 29 | Perfect 29-0 |
|-----------|---------------|--------------|
| 85 | 0.0 | 0.0% |
| 90 | 1.15 | 0.0% |
| 95 | 15.0 | 0.0% |
| 99 | **25.9** | **2.5%** |

Single-race win rate at OVR 99 is ~43/50 — a strong roster still loses races, and a perfect 29-0 season is rare enough to be worth sharing.

## Tech

- Single HTML file, vanilla JS, zero dependencies
- Seeded RNG (`mulberry32`) so a season is reproducible
- ~1,150 lines

## Lineage

X-0 Sports Draft: 38-0 NFL → 24-0 F1 → 36-0 NASCAR → 17-0 IndyCar → 20-0 MotoGP → 24-0 Endurance → 21-0 Tour de France → 17-0 Formula E → 13-0 WRC → 23-0 Giro → 21-0 Vuelta → 8-0 Tour de Suisse → 8-0 Critérium du Dauphiné → 5-0 Monuments → 7-0 Tirreno → 8-0 Paris-Nice → 7-0 Volta a Catalunya → 6-0 Tour de Romandie → 24-0 WSBK → 22-0 Moto2 → 17-0 AMA Supercross → 24-0 AMA Motocross → 22-0 Moto3 → 14-0 Dakar → **29-0 Formula 2**
