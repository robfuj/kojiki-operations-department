# Bots of Operations  (docx S5 candidate menu)

These are the **Major sub-functions** of Operations from the spec. Each is a bot — a
child decision system that can be instantiated to do the actual work.

## Install flow (matches the Orientation Protocol)
1. **Orient** — the agent runs the Kojiki Orientation Protocol (name / industry /
   jurisdiction / siblings).
2. **Research** — the agent researches the field and decides which sub-functions this
   specific org needs.
3. **Install** — instantiate only the chosen bots:
   ```bash
   cd bots
   python3 install_bots.py brand growth performance-marketing
   ```
   (use the slugs listed below; omit args to install all). Each installed bot becomes a
   full decision system under `bots/<slug>/` with README + AGENT.md + schemas + a stub
   decision record, and registers under this department's group_id for handoffs.

Total candidates: 8.

- `business-operations` — **Business Operations**  ·  titles: COO, VP Operations, Operations Director, Operations Manager, Business Operations Manager, Process Improvement Manager, Quality Manager
- `process-management` — **Process Management**  ·  titles: COO, VP Operations, Operations Director, Operations Manager, Business Operations Manager, Process Improvement Manager, Quality Manager
- `service-operations` — **Service Operations**  ·  titles: COO, VP Operations, Operations Director, Operations Manager, Business Operations Manager, Process Improvement Manager, Quality Manager
- `quality` — **Quality**  ·  titles: COO, VP Operations, Operations Director, Operations Manager, Business Operations Manager, Process Improvement Manager, Quality Manager
- `continuous-improvement` — **Continuous Improvement**  ·  titles: COO, VP Operations, Operations Director, Operations Manager, Business Operations Manager, Process Improvement Manager, Quality Manager
- `workforce-management` — **Workforce Management**  ·  titles: COO, VP Operations, Operations Director, Operations Manager, Business Operations Manager, Process Improvement Manager, Quality Manager
- `operational-analytics` — **Operational Analytics**  ·  titles: COO, VP Operations, Operations Director, Operations Manager, Business Operations Manager, Process Improvement Manager, Quality Manager
- `exception-management` — **Exception Management**  ·  titles: COO, VP Operations, Operations Director, Operations Manager, Business Operations Manager, Process Improvement Manager, Quality Manager
