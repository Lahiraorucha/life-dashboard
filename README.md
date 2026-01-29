# Life Dashboard

A beautiful, minimal productivity dashboard to track your goals and daily tasks. Built as a single HTML file - no server, no database, no setup required.

## Features

- **Daily Task Management** - Add, complete, and track tasks for each day
- **Weekly Overview** - See your entire week at a glance with color-coded categories
- **Goal Tracking** - Monitor progress on up to 4 major life goals
- **Customizable Templates** - Set up your ideal weekly schedule, then activate tasks as you do them
- **Works Offline** - All data stored in your browser's localStorage
- **Mobile Friendly** - Responsive design works on phone, tablet, and desktop
- **Zero Dependencies** - Pure HTML, CSS, and JavaScript in a single file

## Quick Start

1. Visit the live demo: [lahiraorucha.github.io/life-dashboard](https://lahiraorucha.github.io/life-dashboard/)
2. Follow the setup wizard to add your goals and weekly schedule
3. Start tracking!

**Or download and run locally:**
- Download `index.html` and open in your browser
- Your data stays in YOUR browser - private and offline

## Files in This Repo

| File | Description |
|------|-------------|
| `index.html` | **Start here!** Clean template with setup wizard - create your own goals & schedule |
| `chaiti-dashboard.html` | Creator's personal dashboard (example of a configured dashboard) |

**Note:** Each person's data is stored in their OWN browser. You cannot see other people's tasks, and they cannot see yours.

## How It Works

### Views

| View | Purpose |
|------|---------|
| **Today** | Focus on today's tasks. Check them off as you complete them. |
| **Week** | See your whole week. Faded = planned, Solid = activated, Strikethrough = done |
| **Goals** | Track progress on your big-picture goals with visual progress bars |

### Task States

- **Faded/Dashed** - Template task (planned but not started)
- **Solid** - Activated (you're committed to doing it today)
- **Strikethrough** - Completed!

### Categories

Customize these in the setup wizard:
- 🏃 Fitness/Training
- 🎨 Creative Work
- 💼 Career/Job
- 💻 Projects
- 📌 Other

## Customization

### First-Time Setup

When you first open the dashboard, you'll see a setup wizard that lets you:

1. **Set Your Goals** - What are you working toward? (e.g., "Run a marathon", "Launch my app")
2. **Set Deadlines** - When do you need to achieve them?
3. **Create Your Weekly Template** - What's your ideal week look like?

### Editing Later

Click the ⚙️ button anytime to:
- Modify your goals
- Adjust your weekly template
- Change category colors
- Reset everything

### For Developers

The dashboard is a single HTML file with embedded CSS and JavaScript. Key sections:

```
<style>        - All styling (CSS variables at top for easy theming)
<body>         - HTML structure
<script>       - All functionality
  - templateSchedule  - Your weekly template
  - tasks            - Stored task data
  - Goals config     - Your goal definitions
```

To customize colors, find the CSS variables at the top of the `<style>` section.

## Data Storage

All data is stored in your browser's `localStorage`. This means:
- ✅ Works offline
- ✅ No account needed
- ✅ Your data stays on your device
- ⚠️ Clearing browser data will reset the dashboard
- ⚠️ Data doesn't sync between devices

**To backup your data:** Use the built-in Export feature in Settings (⚙️ → Export Data)

**To restore:** Use Import Data in Settings, or open browser console:
```javascript
// View your config
console.log(localStorage.getItem('lifeDashCfg'));
// View your task data
console.log(localStorage.getItem('lifeDashData'));
```

## Philosophy

This dashboard is built on a few principles:

1. **Simplicity over features** - One HTML file, no build process, no dependencies
2. **Templates as guides, not rules** - Your weekly template suggests tasks, but you decide what to actually do each day
3. **Progress over perfection** - The goal is to show up consistently, not to check every box
4. **Your data is yours** - No accounts, no tracking, no cloud

## Contributing

Found a bug? Have an idea?
- Open an issue
- Submit a pull request
- Or fork it and make it your own!

## License

MIT License - Do what you need to build a better tracking system for your daily life!

---

Built with ❤️ as a personal project to help track multiple life goals simultaneously.
