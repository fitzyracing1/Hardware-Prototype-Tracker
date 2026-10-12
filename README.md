# Hardware-Prototype-Tracker

> **Simple structured data + status tracking for hardware prototypes, BOMs, and progress.**
> Designed for easy updates via **voice-to-text or text on your phone**, automatically turned into **GitHub Issues** and visualized in a **live GitHub Projects dashboard** (kanban / table / roadmap).

Perfect for ambitious projects like **Tesla Bot Cruiser**, **Open Source Spaceship**, **Nanocraft**, **Organic Spin Processor**, and other futuristic or open-source hardware initiatives.

**Repo:** https://github.com/fitzyracing1/Hardware-Prototype-Tracker

## 🚀 Quick Phone Update Workflow (Voice/Text Friendly)

1. Install/open the **GitHub mobile app** (or use mobile browser).
2. Navigate to this repo → **Issues** tab.
3. **Fastest way — Comment on existing tracking issue**:
   - Open the main issue for your project (e.g. "Tesla Bot Cruiser - Main Tracking").
   - Tap the comment box.
   - Tap the **microphone** on your phone keyboard and **dictate** your update naturally:
     > "Tesla Bot Cruiser update: Main chassis frame successfully 3D printed today. Overall progress now at 32 percent. Added two new BOM items for motor controllers — sourced from supplier. Next milestone is electronics integration and first power test next week. Status: Prototyping. No blockers right now."
   - Post the comment. Done! It's timestamped, searchable, and part of permanent history.
4. **For more structured reports**: Tap **New Issue** and choose the **"Hardware Progress Update"** template. Dictate field-by-field.
5. **View & manage live dashboard**: Go to **Projects** tab in repo (or your user Projects). See kanban board, sortable table with progress %, filter by project/label. On phone you can drag cards or edit fields directly for instant visual updates.

This turns voice notes on the go into professional, trackable artifacts without friction.

## 📊 Live Dashboard (GitHub Projects)

GitHub Projects gives you a beautiful, real-time dashboard:

- **Board view**: Kanban columns (Backlog → Concept → Prototyping → Testing → Complete)
- **Table view**: Sort/filter by Progress %, Last Updated, BOM Status, Next Milestone
- **Roadmap view**: Timeline of milestones across projects

**Setup instructions** (one-time, ~2 minutes):
1. In this repo go to **Projects** tab → "New project" (or create at https://github.com/users/fitzyracing1/projects and add this repo).
2. Add the main tracking issues as items.
3. In project settings, add custom fields if desired:
   - Status (single-select)
   - Progress (number 0-100)
   - BOM Status (single-select)
   - Next Milestone (text)
4. Create multiple views as above.
5. Link issues to the project for automatic inclusion.

On phone: Open in Safari/Chrome or GitHub app → Projects. Super responsive.

*Note: If full project automation is desired later, reconnect the GitHub connector in your tools with additional Projects permissions.*

## 📁 Structured Data Format (Optional but Recommended)

For version-controlled, machine-readable tracking beyond issues, create simple Markdown files with **YAML frontmatter** in the `projects/` folder (or root).

**Example `projects/tesla-bot-cruiser.md`**:

```yaml
---
project: "Tesla Bot Cruiser"
category: "Robotics / Mobile Platform"
status: "Prototyping"
progress_percent: 32
last_updated: "2026-07-21"
bom_version: "v0.9"
bom_status: "In Progress"
next_milestone: "Electronics integration & initial power-on test"
blockers: "None critical"
owner: "fitzyracing1"
---
```

Then add human-readable sections:

```markdown
# Tesla Bot Cruiser

**Description:** Cruiser-style autonomous mobile platform leveraging Tesla Bot/Optimus tech for logistics, exploration or research applications.

## Current Status
Prototyping phase. Chassis fabricated. Motors and basic electronics in procurement.

## BOM Summary (High-Level)

| Category     | Item                  | Qty | Status     | Notes / Supplier          | Est. Cost |
|--------------|-----------------------|-----|------------|---------------------------|-----------|
| Mechanical  | Main chassis frame   | 1   | Complete  | 3D printed / CNC         | TBD      |
| Propulsion  | Drive motors         | 4   | Sourced   | High-torque BLDC         | TBD      |
| Electronics | Motor controllers    | 2   | In Progress | Dual channel ESC        | TBD      |
| Power       | Battery pack         | 1   | TBD       | High capacity Li-ion     | TBD      |
| Sensors     | IMU + LIDAR          | 1+  | TBD       | For navigation           | TBD      |

## Progress Log
- **2026-07-21**: Tracker system initialized. Chassis prototype complete. Progress 32%.
- **2026-07-20**: Initial concept and high-level BOM drafted.

## References & Links
- Related: Tesla Optimus / Bot projects
- Issues: #2 (main tracking)
```

**Why use this?** Git history shows every BOM change and progress delta. Easy to parse with scripts later for aggregated dashboards or reports. Start minimal — expand as project grows.

## 🏷️ Recommended Labels

**Project tags**: `tesla-bot-cruiser`, `open-source-spaceship`, `nanocraft`, `organic-spin-processor`

**Categories**: `hardware`, `mechanical`, `electronics`, `power`, `sensors`, `software`, `firmware`, `bom`, `testing`, `documentation`

**Actions**: `progress-update`, `bom-update`, `milestone`, `blocker`, `idea`, `help-wanted`, `meta`

Use labels liberally for powerful filtering in Issues and Projects.

## 📋 Current Main Tracking Issues

- **Tesla Bot Cruiser** — [Main Tracking Issue](https://github.com/fitzyracing1/Hardware-Prototype-Tracker/issues/2) (create/update via template or comments)
- **Open Source Spaceship** — [Main Tracking Issue](https://github.com/fitzyracing1/Hardware-Prototype-Tracker/issues/3)
- **Nanocraft** — [Main Tracking Issue](https://github.com/fitzyracing1/Hardware-Prototype-Tracker/issues/4)
- **Organic Spin Processor** — [Main Tracking Issue](https://github.com/fitzyracing1/Hardware-Prototype-Tracker/issues/5)
- **Tracker System Itself** — [Meta Improvements](https://github.com/fitzyracing1/Hardware-Prototype-Tracker/issues/1)

Create new ones easily with the template or by labeling appropriately.

## 🛠️ How to Add Your Own Project

1. Create a new issue using the Hardware Progress Update template (or blank).
2. Optionally create `projects/your-project-name.md` with the YAML + sections above.
3. Add labels for easy discovery.
4. (Recommended) Add the issue to your Projects dashboard.

## 🔮 Future Enhancements (Roadmap)

- GitHub Action to automatically parse all `projects/*.md` YAML frontmatter and update Project item fields or post a daily summary comment.
- Phone automation examples (iOS Shortcuts / Android Tasker) to voice-create issues.
- Photo attachment support and wiki for build logs.
- CSV/JSON export scripts for external tools (Excel, Notion, Airtable sync).
- Multi-project aggregated dashboard page (GitHub Pages or wiki).

## 💡 Tips for Effective Tracking

- Update little and often — even 30-second voice notes after a work session keep momentum visible.
- Use consistent status terms across issues and YAML.
- Attach photos/screenshots to issue comments for visual progress (GitHub supports it well).
- For complex BOMs, maintain the table in the MD file and reference the latest issue comment.
- Review the Projects dashboard weekly for overview and prioritization.

---

**Track it simply. Update from anywhere (even in the shop or field). Visualize progress beautifully. Ship hardware faster.**

*For makers, engineers, and visionaries building the next generation of robots, spacecraft, nanocrafts, advanced processors, and beyond.*

---

*Initialized: 2026-07-21* | *Main branch* | *Open for collaboration and personal use*
## Documentation

- In-repo docs: [docs/](docs/index.md)
- Wiki: [https://github.com/fitzyracing1/Hardware-Prototype-Tracker/wiki](https://github.com/fitzyracing1/Hardware-Prototype-Tracker/wiki)
