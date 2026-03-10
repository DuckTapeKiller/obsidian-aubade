[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/ducktapekiller)

![aubade](screenshots/cover.png)

**Aubade** is a retro-brutalist theme for [Obsidian](https://obsidian.md). It prioritises strict geometry, high contrast, and tactile interactions over soft gradients and rounded corners. Designed for users who require their digital workspace to feel like a structural tool.

# Table of contents

<!--toc:start-->
- [Visual Identity](#visual-identity)
- [Colour Schemes](#colour-schemes)
- [Select your favourite pattern](#select-your-favourite-pattern)
- [Key Features](#key-features)
- [Typography](#typography)
  - [Sans Serif](#sans-serif)
  - [Monospace](#monospace)
- [Layout & Configuration](#layout--configuration)
  - [Alignment](#alignment)
  - [Note Width Control](#note-width-control)
  - [Typography Settings](#typography-settings)
- [Per-Note Overrides](#per-note-overrides)
  - [Custom Widths](#custom-widths)
  - [Interface Hiding](#interface-hiding)
- [Dashboard & Masonry Layout](#dashboard--masonry-layout)
  - [CSS-Only Timelines](#css-only-timelines)
- [Installation](#installation)
  - [Method 1: Community Themes (CURRENTLY PENDING REVIEW BY OBSIDIAN)](#method-1-community-themes-currently-pending-review-by-obsidian)
  - [Method 2: Manual Installation](#method-2-manual-installation)
- [Gallery](#gallery)
  - [Dark Mode](#dark-mode)
  - [Light Mode](#light-mode)
<!--toc:end-->

## Visual Identity

* **Strict Geometry:** A zero-radius policy applied globally. Every corner is sharp; every container is a box.
* **Tactile Feedback:** Buttons and interactive elements feature hard, directional shadows (4px offset) that flatten physically when pressed.
* **High Contrast Borders:** 2px thick borders define every UI element, ensuring clear separation between panes, notes, and metadata.
* **Retro Typography:** Defaults to `Space Mono` for UI and `Azeret Mono` for text, reinforcing the terminal/typewriter aesthetic.

## Colour Schemes

| | |
|:---:|:---:|
| **Default**<br>![Default](screenshots/default.png) | **Reader**<br>![Reader](screenshots/reader.png) |
| **Amber**<br>![Amber](screenshots/ambar.png) | **Solarized**<br>![Solarized](screenshots/solarised.png) |
| **Midnight**<br>![Midnight](screenshots/midnight.png) | **Sunset**<br>![Sunset](screenshots/sunset.png) |
| **Ocean**<br>![Ocean](screenshots/ocean.png) | **Forest**<br>![Forest](screenshots/forest.png) |
| **Lavender**<br>![Lavender](screenshots/lavender.png) | **Warm**<br>![Warm](screenshots/warm.png) |
| **Cool**<br>![Cool](screenshots/cool.png) | **Monochrome**<br>![Monochrome](screenshots/monochrome.png) |
| **Brutalist**<br>![Brutalist](screenshots/brutalist.png) | |

## Select your favourite pattern

**Patterns**<br>![Patterns](screenshots/paterns.png)

## Key Features

* **Dashboard Ready:** Built-in grid support for dashboard layouts, automatically handling column breaks and gap spacing.
* **Mobile Optimised:** Features a custom bottom navigation bar, neutralised animations for better performance, and enlarged touch targets.
* **Nuclear Anti-Roundness:** Specific overrides ensure no plugin or native element introduces rounded corners.
* **Striped Headers:** Windows 95-style pinstripe gradients on window titles and tab containers.

## Typography

This theme contains the following typefaces:

### Sans Serif

* **iA Writer Quattro S** by Information Architects: [Source](https://github.com/iaolo/iA-Fonts)

### Monospace

* **Azeret Mono** by Displaay: [Source](https://fonts.google.com/specimen/Azeret+Mono)
* **Space Mono** by Colophon Foundry: [Source](https://fonts.google.com/specimen/Space+Mono)
* **Noto Sans Mono** by Google: [Source](https://fonts.google.com/noto/specimen/Noto+Sans+Mono)
* **iA Writer Duo S** by Information Architects: [Source](https://github.com/iaolo/iA-Fonts)
* **iA Writer Mono S** by Information Architects: [Source](https://github.com/iaolo/iA-Fonts)

**Clarification:** Typefaces are embedded within the theme, ensuring they are available offline and on any device without requiring local installation.

In **Style Settings**, you can choose any of these fonts for either the Body or the UI/Headers.

## Layout & Configuration

You can fine-tune the reading experience in **Style Settings**.

### Alignment
Modify the text alignment of your notes using the dropdown menu:
* Left aligned (Default)
* Right aligned
* Centre aligned
* Justified

### Note Width Control
When Obsidian's **"Readable line length"** setting is enabled, the editor width defaults to **700px**. You can adjust this global maximum width in Style Settings using a slider ranging from **500px** to **1600px**.

> **Note on Mobile:** These width constraints apply to **Desktop** only. On mobile devices, the theme automatically fits content to the screen width.

### Typography Settings
* **Line Height:** Adjust line spacing between **1.0** and **3.0** (Default: 1.5).
* **Inline Title Size:** Adjust the size of the inline title between **1.0em** and **5.0em** (Default: 3em).

## Per-Note Overrides

Use the `cssclasses` property in your frontmatter (YAML) to override global settings for specific files. These classes function regardless of your global "Readable line length" setting.

### Custom Widths
Useful for notes containing wide tables or diagrams:
* `width-800` (800px)
* `width-900` (900px)
* `width-1000` (1000px)
* `width-1200` (1200px)
* `width-1600` (1600px)
* `full-width` (100% of pane width)

### Interface Hiding
To hide the frontmatter, inline title, and property metadata for a specific note:
* `hide-all`

**Example:**
```yaml
---
cssclasses:
  - width-1200
  - hide-all
---
```

## Dashboard & Masonry Layout

The theme allows you to organise your notes into a clean, visual grid. The system supports native **Obsidian Callouts** and automatically handles column distribution (responsive flow).

To activate, add `cssclasses: dashboard` to your note's frontmatter. Every Callout within that note will transform into a masonry card.

```markdown
---
cssclasses:
  - dashboard
---

> [!abstract] General
> - [[Link 1]]
> - [[Link 2]]

> [!abstract] Essays
> - [[Link A]]
> - [[Link B]]
> - [[Link C]]

> [!abstract] Projects
> - [[Project X]]
> - [[Project Y]]
```

### CSS-Only Timelines

The theme features a native, CSS-only timeline layout that transforms standard bulleted lists into a professional split-view chronology without requiring any external plugins. To activate it, add `cssclasses: custom-timeline` to your note's frontmatter.

Structure your timeline as a single, continuous unordered list. Every event must consist of exactly three bullet points in this strict sequence: Date, Title, and Content. The theme will automatically remove the default bullet points, draw a vertical line, and format the items into a structured grid.

**Example:**

```markdown
---
cssclasses: custom-timeline
---

- 1950–1953
- Land Reform Movement
- Shortly after the establishment of the PRC, the Chinese Communist Party (CCP) launched a nationwide campaign to confiscate land from rural landlords and redistribute it to landless peasants.

- 1951–1952
- Three-Anti and Five-Anti Campaigns
- These were urban reform movements designed to consolidate state control over the economy...
```

![timeline](screenshots/timeline.png)

## Installation

### Method 1: Community Themes (CURRENTLY PENDING REVIEW BY OBSIDIAN)
1. Open **Settings** > **Appearance**.
2. Click **Manage** under Themes.
3. Search for **Aubade**.
4. Click **Install** and then **Use**.

### Method 2: Manual Installation
1. Download `theme.css` and `manifest.json` from the [Releases](../../releases) page.
2. Open your Obsidian vault folder.
3. Navigate to `.obsidian/themes`.
4. Create a new folder named `Aubade`.
5. Paste the files into this folder.
6. Reload Obsidian and select **Aubade** in **Settings > Appearance > Themes**.

## Gallery

### Dark Mode
![Aubade Dark Mode](screenshot.png)

### Light Mode
![Aubade Light Mode](screenshot-light.png)
