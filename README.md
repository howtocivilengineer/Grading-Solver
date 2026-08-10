# Grading Solver

**Pads, falls and batters for light civils — in the browser, offline.**

Drop in a survey, lay out your pads, set the levels, and read the cut, fill and
cost straight back. Grading Solver takes a site from ground surface to a graded
design without a desktop package or a licence, and nothing leaves your machine.

**→ [Open Grading Solver](https://howtocivilengineer.github.io/Grading-Solver/)**

---

## What it does

Grading Solver builds a design surface from pads and grade lines sitting on a
survey, then measures the earthworks against the ground. It is aimed at the
everyday light-civils job — a yard, a car park, a building platform, an access —
where you need honest cut/fill and a cost in minutes, not a full corridor model.

- **Start from a survey, a DXF, or nothing.** Drop a LandXML survey to set the
  ground. Drop a DXF of closed polylines to bring outlines straight in as pads,
  or open polylines as grade lines. With neither, you get a worked demo site to
  learn on.
- **Pads with real falls.** Each pad carries its own corner levels, string
  grades and batter slopes (cut and fill set independently, 1V : n). Edges can
  be retained instead of battered, and the wall lengths come back in the costs.
- **Grade lines between pads.** Draw a line stake-to-stake and it ties in
  exactly to the levels of the stakes at each end — move a stake and the line
  follows. Two stakes on one pad shapes that pad's surface; two stakes on
  different pads cuts a graded line with batters both sides down to daylight.
- **Batters to daylight.** Every pad and line battters out to meet the existing
  ground, clipped to a site boundary if you set one.
- **Cut, fill and balance.** Bulk earthworks are measured cell by cell against
  the stripped ground, with topsoil strip volumes reported separately over the
  works and over the whole site. A one-click balance moves a pad to null the net.
- **Cost the job.** Cut-to-fill, cut-to-waste, import and retained-wall rates
  give an order-of-cost, itemised with quantity and money per line against a
  grand total.
- **See it in plan, 3D and section.** Plan view with cut/fill shading and
  contours, an orbitable 3D surface, and a live section cut anywhere across the
  site.
- **Metric or imperial.** A single toggle reads the survey as metric (m, m³) or
  imperial (ft, yd³) — it relabels and reports, it never rescales your
  coordinates.

## Video

[![Watch the video](https://img.youtube.com/vi/3GtvRoUluCg/maxresdefault.jpg)](https://youtu.be/3GtvRoUluCg)

## Getting started

1. Open the [app](https://howtocivilengineer.github.io/Grading-Solver/).
2. Drop a **LandXML** survey onto the page to set the ground, or hit
   **Load the demo site** to explore with worked data.
3. Add pads — draw one, or drop a **DXF** of closed outlines.
4. Set corner levels, string grades and batters under **Grading**.
5. Read the cut, fill and balance in the summary, and the costed quantities
   under **Rates**.
6. Export when you are happy.

Everything runs on your machine. No account, no upload, no internet needed once
the page has loaded.

## Import

| Format | Comes in as |
|--------|-------------|
| LandXML | The existing ground surface |
| DXF (closed polylines) | Pad outlines |
| DXF (open polylines / lines) | Grade lines, tied into nearby pad stakes |
| Saved job (`.json`) | A full project, reopened as you left it |

## Export

- **LandXML** — the stripped, subgrade and finished surfaces, for handing on to
  another package or a machine-control system.
- **DXF** — pad outlines with corner levels, design contours and a legend, each
  on its own layer.
- **Save the job** — a single `.json` holding the whole project to reopen later.
- **Dev data** — everything as structured data, for scripting or checking.

Export the design surfaces at 1 m spacing if you want another tool to reproduce
the volumes shown here; coarser spacing loses a little accuracy.

## Notes on the numbers

- Quantities are **geometric** — no bulking or compaction factors are applied.
  Multiply by your own factors downstream.
- Volumes are measured on a grid. Finer grids are more accurate but heavier;
  the default is a sensible balance for light-civils work.
- Retained-wall lengths are taken from edges you have explicitly marked to
  retain rather than batter, split at a sensible height for pricing.

## Languages

English, Português, Français and Español, switchable from the header.

## Privacy

Grading Solver is a single HTML page that runs entirely in your browser. Your
survey, your design and your rates stay on your computer — nothing is uploaded
anywhere.

## Part of the Solver set

Grading Solver is one of a small set of browser-based civil tools from
[How To Civil Engineer](https://github.com/howtocivilengineer), alongside
**Topo Solver** (survey points to a reviewed surface) and **Volume Solver**
(compare two surfaces for cut and fill). They share a common look and workflow
and hand LandXML between one another.

## Licence & disclaimer

Grading Solver is provided as an engineering aid. It does not replace a
qualified engineer's judgement or a formal design check. Always verify
quantities and levels against your own calculations before construction.
