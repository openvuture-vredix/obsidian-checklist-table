![](assets/logo.png)

<br>
<br>


# Checklist Table

A powerful Obsidian plugin that transforms simple markdown into beautiful, interactive checklist tables with customizable columns, progress tracking, and multiple task states.

## Features

### Flexible Task Management
- **Multiple task states**: Open, Done, Cancelled, Important, Forwarded, Scheduled
- **Custom columns**: Define your own column structure for different workflows
- **Quick task addition**: Add new tasks directly from the table interface
- **Visual progress tracking**: Real-time progress bar with color-coded completion status

### Beautiful Design
- Clean, modern table design that integrates seamlessly with your Obsidian theme
- Color-coded checkboxes for different task states
- Smooth animations and hover effects
- Responsive layout that works on desktop and mobile

### Multilingual Support
- English and German translations included
- Auto-detection of system language
- Easy to extend with additional languages

### Customizable
- Configure default column headers, or set them as needed per table
- Choose when to show controls (on hover or always visible)
- Flexible table structure with support for sections and separators (no limitations)



## Installation

### From Obsidian Community Plugins (Recommended)

... coming soon ...


### Manual Installation

1. Download the latest release from the [releases page](https://github.com/openvuture-vredix/obsidian-checklist-table/releases)
2. Extract the folder to your vault's `.obsidian/plugins/` folder
3. Reload Obsidian
4. Enable the plugin in Settings → Community Plugins



## Usage

### Basic Syntax

Create a checklist table using a code block with the `checklist` language identifier:
(The first line, which starts with a | gets rendered as the Header)

![](assets/progress-bar-and-button.png)


````markdown
```checklist

| Task | Details |

[ ] Write documentation
[ ] Test features
[ ] Deploy to production

```
````

### Task States

Change task states by right-clicking on a checkbox:

![](assets/multiple-states-with-context-menu.png)

- `[ ]` - Open task (empty checkbox)
- `[x]` - Completed task (✓)
- `[-]` - Cancelled task (−)
- `[!]` - Important task (!)
- `[>]` - Forwarded task (›)
- `[<]` - Scheduled task (‹)

### Multiple Columns

Add as many columns and headings as you need:

![](assets/unlimited-headings.png)

````markdown
```checklist

| Project | Task | Priority | Due Date |

[ ] Website Redesign | Update homepage | High | 2024-03-15
[ ] Mobile App | Fix login bug | Medium | 2024-03-10
[ ] Documentation | Write API docs | Low | 2024-03-20

```
````

### Adding Tasks

Hover over the table to reveal the **+** button, which allows you to add new tasks without editing the markdown directly.
(Can be changed to permanently visible in the plugin settings)

### Sections with Separators

Use `---` to create visual separators between task groups:

![](assets/separator-line.png)

````markdown
```checklist

| Task | Details |

[ ] Design phase task
[ ] Design review
---
[ ] Development phase task
[ ] Code review
```
````

### Links and Formatting

Use standard Obsidian markdown syntax within cells:

![](assets/linked-notes.png)

````markdown
```checklist

| Task | Notes |

[ ] Review [[Project Plan]] | See **Section 3** for details
[ ] Update [GitHub](https://github.com) | Check open issues

```
````

## ⚙️ Configuration

Open **Settings → Checklist Table** to customize:

### Language
Choose between English, German, or automatic system detection.

### Default Columns
Set your preferred column headers (comma-separated). These will be used when inserting a new checklist block via command.

### Always Show Controls
Toggle whether the progress bar and add button should always be visible or only appear on hover.

## Command Palette

Access these commands via `Ctrl/Cmd + P`:

- **Insert Checklist Block**: Quickly insert a new checklist template at your cursor



## Example Use Cases

### Project Management
````markdown
```checklist

| Phase | Task | Status | Owner |

[ ] Planning | Define requirements | In Progress | Alice
[x] Planning | Create timeline | Completed | Bob
[ ] Development | Setup environment | Not Started | Charlie

```
````

### Study Planning
````markdown
```checklist

| Subject | Topic | Progress |

[!] Math | Calculus review | Urgent
[ ] Physics | Quantum mechanics | Chapter 3
[x] Chemistry | Organic reactions | Finished

```
````

### Shopping List
````markdown
```checklist

| Item | Store | Notes |

[x] Milk | Supermarket | 2 liters
[ ] Bread | Bakery | Whole grain
[-] Eggs | Supermarket | Cancelled - already have

```
````

## 🛠️ Development

### Building from Source

```bash
# Clone the repository
git clone https://github.com/openvuture-vredix/obsidian-checklist-table.git

# Install dependencies
npm install

# Build the plugin
npm run build

# Development mode with auto-rebuild
npm run dev
```

### Project Structure

```
obsidian-checklist-table/
├── main.js          # Bundled plugin code
├── manifest.json    # Plugin metadata
├── styles.css       # Plugin styles

```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🐛 Bug Reports & Feature Requests

Found a bug or have an idea for a new feature? Please open an issue on the [GitHub issues page](https://github.com/openvuture-vredix/obsidian-checklist-table/issues).

## 💖 Support

If you find this plugin helpful, consider:
- ⭐ Starring the repository
- 🐛 Reporting bugs to help improve the plugin
- 💡 Suggesting new features
- 📣 Sharing it with other Obsidian users

## 🔗 Links

- [Reddit](https://www.reddit.com/user/vuture44/)

- [GitHub Repository](https://github.com/openvuture-vredix/obsidian-checklist-table)
- [Report Issues](https://github.com/openvuture-vredix/obsidian-checklist-table/issues)
- [Obsidian Community](https://obsidian.md/community)

## 📜 Changelog

### Version 1.0.0
- 🎉 Initial release
- Multiple task states (Open, Done, Cancelled, Important, Forwarded, Scheduled)
- Progress tracking with color-coded progress bar
- In-table task addition
- Multilingual support (English, German)
- Customizable columns and settings
- Mobile and desktop support

---

Made by [Vredix](https://github.com/openvuture-vredix)
