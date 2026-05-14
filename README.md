[![GitHub Repo stars](https://img.shields.io/github/stars/ducktapekiller/obsidian-aubade?style=flat&logo=obsidian&color=%23f39c12)](https://github.com/ducktapekiller/obsidian-aubade/stargazers)
[![GitHub issues](https://img.shields.io/github/issues/DuckTapeKiller/obsidian-aubade?logo=obsidian&color=%23f39c12)](https://github.com/DuckTapeKiller/obsidian-aubade/issues)
[![GitHub closed issues](https://img.shields.io/github/issues-closed/DuckTapeKiller/obsidian-aubade?logo=obsidian&color=%23f39c12)](https://github.com/DuckTapeKiller/obsidian-aubade/issues?q=is%3Aissue+is%3Aclosed)
[![GitHub manifest version](https://img.shields.io/github/manifest-json/v/DuckTapeKiller/obsidian-aubade?logo=obsidian&color=%23f39c12)](https://github.com/DuckTapeKiller/obsidian-aubade/blob/main/manifest.json)
[![Downloads](https://img.shields.io/github/downloads/DuckTapeKiller/obsidian-aubade/total?logo=obsidian&color=%23f39c12)](https://github.com/DuckTapeKiller/obsidian-aubade/releases)

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/ducktapekiller)

![aubade](screenshots/cover.png)

**Aubade** is a retro-brutalist theme for [Obsidian](https://obsidian.md). It prioritises strict geometry, high contrast, and tactile interactions over soft gradients and rounded corners. Designed for users who require their digital workspace to feel like a structural tool.

# Table of contents

1. [Visual Identity](#1-visual-identity)
2. [Colour Schemes](#2-colour-schemes)
3. [Select your favourite pattern](#3-select-your-favourite-pattern)
4. [Key Features](#4-key-features)
5. [Typography](#5-typography)
   1. [Sans Serif](#51-sans-serif)
   2. [Monospace](#52-monospace)
   3. [Serif](#53-serif)
6. [Layout and Configuration](#6-layout-and-configuration)
   1. [Alignment](#61-alignment)
   2. [Note Width Control](#62-note-width-control)
   3. [Typography Settings](#63-typography-settings)
7. [Per-Note Overrides](#7-per-note-overrides)
   1. [Custom Widths](#71-custom-widths)
   2. [Interface Hiding](#72-interface-hiding)
8. [Dashboard and Masonry Layout](#8-dashboard-and-masonry-layout)
9. [CSS-Only Timelines](#9-css-only-timelines)
10. [Image Captions](#10-image-captions)
11. [Installation](#11-installation)
    1. [Method 1: Community Themes (CURRENTLY PENDING REVIEW BY OBSIDIAN)](#111-method-1-community-themes-currently-pending-review-by-obsidian)
    2. [Method 2: Manual Installation](#112-method-2-manual-installation)
12. [Gallery](#12-gallery)
    1. [Dark Mode](#121-dark-mode)
    2. [Light Mode](#122-light-mode)
- [SUMMARY: ALL CSSCLASSES AVAILABLE](#summary-all-cssclasses-available)

## 1 Visual Identity

* **Strict Geometry:** A zero-radius policy applied globally. Every corner is sharp; every container is a box.
* **Tactile Feedback:** Buttons and interactive elements feature hard, directional shadows (4px offset) that flatten physically when pressed.
* **High Contrast Borders:** 2px thick borders define every UI element, ensuring clear separation between panes, notes, and metadata.
* **Retro Typography:** Defaults to `Space Mono` for UI and `Azeret Mono` for text, reinforcing the terminal/typewriter aesthetic.

## 2 Colour Schemes

| | |
|:---:|:---:|
| **Default**<br>![Default](screenshots/default.png) | **Reader**<br>![Reader](screenshots/reader.png) |
| **Amber**<br>![Amber](screenshots/ambar.png) | **Solarized**<br>![Solarized](screenshots/solarised.png) |
| **Midnight**<br>![Midnight](screenshots/midnight.png) | **Sunset**<br>![Sunset](screenshots/sunset.png) |
| **Ocean**<br>![Ocean](screenshots/ocean.png) | **Forest**<br>![Forest](screenshots/forest.png) |
| **Lavender**<br>![Lavender](screenshots/lavender.png) | **Warm**<br>![Warm](screenshots/warm.png) |
| **Cool**<br>![Cool](screenshots/cool.png) | **Monochrome**<br>![Monochrome](screenshots/monochrome.png) |
| **Brutalist**<br>![Brutalist](screenshots/brutalist.png) | |

## 3 Select your favourite pattern

**Patterns**<br>![Patterns](screenshots/paterns.png)

## 4 Key Features

* **Dashboard Ready:** Built-in grid support for dashboard layouts, automatically handling column breaks and gap spacing.
* **Mobile Optimised:** Features a custom bottom navigation bar, neutralised animations for better performance, and enlarged touch targets.
* **Nuclear Anti-Roundness:** Specific overrides ensure no plugin or native element introduces rounded corners.
* **Striped Headers:** Classic vintage MacOS-style pinstripe gradients on window titles and tab containers.

## 5 Typography

This theme contains the following typefaces:

### 5.1 Sans Serif

* **iA Writer Quattro S** by Information Architects: [Source](https://github.com/iaolo/iA-Fonts)
* **iA Writer Duo S** by Information Architects: [Source](https://github.com/iaolo/iA-Fonts)
* **Sen** by Akira Yoshino: [Source](https://fonts.google.com/specimen/Sen)
* **Montserrat** by Julieta Ulanovsky: [Source](https://fonts.google.com/specimen/Montserrat)
  
### 5.2 Monospace

* **Azeret Mono** by Displaay: [Source](https://fonts.google.com/specimen/Azeret+Mono)
* **Space Mono** by Colophon Foundry: [Source](https://fonts.google.com/specimen/Space+Mono)
* **iA Writer Mono S** by Information Architects: [Source](https://github.com/iaolo/iA-Fonts)
* **JetBrains Mono** by JetBrains: [Source](https://www.jetbrains.com/lp/mono/)
  
### 5.3 Serif

* **Marcellus** by Eduardo Tunni: [Source](https://fonts.google.com/specimen/Marcellus)
* **IBM Plex Serif** by IBM: [Source](https://fonts.google.com/specimen/IBM+Plex+Serif)
* **Lora** by by Cyreal Type: [Source](https://fonts.google.com/specimen/Lora)

**Clarification:** Typefaces are embedded within the theme, ensuring they are available offline and on any device without requiring local installation.

In **Style Settings**, you can choose any of these fonts for either the Body or the UI/Headers.

## 6 Layout and Configuration

You can fine-tune the reading experience in **Style Settings**.

### 6.1 Alignment
Modify the text alignment of your notes using the dropdown menu:
* Left aligned (Default)
* Right aligned
* Centre aligned
* Justified

### 6.2 Note Width Control
When Obsidian's **“Readable line length”** setting is enabled, the editor width defaults to **700px**. You can adjust this global maximum width in Style Settings using a slider ranging from **500px** to **1600px**.

> **Note on Mobile:** These width constraints apply to **Desktop** only. On mobile devices, the theme automatically fits content to the screen width.

### 6.3 Typography Settings
* **Line Height:** Adjust line spacing between **1.0** and **3.0** (Default: 1.5).
* **Inline Title Size:** Adjust the size of the inline title between **1.0em** and **5.0em** (Default: 3em).

## 7 Per-Note Overrides

Use the `cssclasses` property in your frontmatter (YAML) to override global settings for specific files. These classes function regardless of your global “Readable line length” setting.

### 7.1 Custom Widths
Useful for notes containing wide tables or diagrams:
* `width-800` (800px)
* `width-900` (900px)
* `width-1000` (1000px)
* `width-1200` (1200px)
* `width-1600` (1600px)
* `full-width` (100% of pane width)

### 7.2 Interface Hiding
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

## 8 Dashboard and Masonry Layout

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

## 9 CSS-Only Timelines

The theme features a native, CSS-only timeline layout that transforms standard bulleted lists into a professional split-view chronology without requiring any external plugins. To activate it, add `cssclasses: custom-timeline` to your note's frontmatter.

Structure your timeline as a single, continuous unordered list. Every event must consist of exactly three bullet points in this strict sequence: Date, Title, and Content. The theme will automatically remove the default bullet points, draw a vertical line, and format the items into a structured grid.

**Example:**

```markdown
---
cssclasses:
  - custom-timeline
  - hide-all
---

- 1493
- Bulas Inter Caetera y segundo viaje de Colón
- El papa Alejandro VI expide las bulas Inter Caetera, concediendo a la Corona castellana las tierras descubiertas y por descubrir, a cambio de la conversión de sus habitantes al cristianismo. En este mismo segundo viaje de Colón participa fray Ramón Pané, quien se dedicará a investigar los mitos taínos y llevará a cabo las primeras labores evangelizadoras en el Caribe. Es el primer europeo en recopilar sistemáticamente la mitología indígena americana.

- 1494
- Tratado de Tordesillas
- Con mediación papal, España y Portugal regulan la repartición de los territorios descubiertos. El tratado establece una línea divisoria que determinará el reparto colonial del continente americano y consolida la autoridad del papa como única fuente de derecho temporal y espiritual sobre los nuevos territorios.
```

![timeline](screenshots/timeline.png)

## 10 Image Captions

This theme includes built-in support for displaying image captions. The caption text is automatically extracted from the image embed syntax and displayed directly beneath the image, utilising the theme's interface font.

#### How to use

To add a caption, insert your text after a pipe character (`|`) within the standard Obsidian image embed brackets:

```markdown
![[filename.jpg|Your caption text goes here]]
```

#### Expected behaviour

When rendered, the text provided after the pipe will appear as a formatted caption block beneath the image. 

Please note a technical limitation: if you embed an image without specifying a custom caption, Obsidian automatically assigns the file name as the alternative text. In this scenario, the theme will display the file name beneath the image instead of remaining blank.

## 11 Installation

### 11.1 Method 1: Community Themes (CURRENTLY PENDING REVIEW BY OBSIDIAN)
1. Open **Settings** > **Appearance**.
2. Click **Manage** under Themes.
3. Search for **Aubade**.
4. Click **Install** and then **Use**.

### 11.2 Method 2: Manual Installation
1. Download `theme.css` and `manifest.json` from the [Releases](../../releases) page.
2. Open your Obsidian vault folder.
3. Navigate to `.obsidian/themes`.
4. Create a new folder named `Aubade`.
5. Paste the files into this folder.
6. Reload Obsidian and select **Aubade** in **Settings > Appearance > Themes**.

## 12 Gallery

### 12.1 Dark Mode
![Aubade Dark Mode](screenshot.png)

### 12.2 Light Mode
![Aubade Light Mode](screenshot-light.png)


## SUMMARY: ALL CSSCLASSES AVAILABLE

| `cssclass` | Function | Behaviour Details |
| :--- | :--- | :--- |
| `width-800` | Sets fixed note width | Constrains the editor and reading view content to a maximum width of 800px. Centers the content. |
| `width-900` | Sets fixed note width | Constrains the editor and reading view content to a maximum width of 900px. Centers the content. |
| `width-1000` | Sets fixed note width | Constrains the editor and reading view content to a maximum width of 1000px. Centers the content. |
| `width-1200` | Sets fixed note width | Constrains the editor and reading view content to a maximum width of 1200px. Centers the content. |
| `width-1600` | Sets fixed note width | Constrains the editor and reading view content to a maximum width of 1600px. Centers the content. |
| `full-width` | Sets responsive width | Forces the note content to span 100% of the available viewing pane. |
| `hide-all` | UI visibility toggle | Completely hides the frontmatter container, metadata properties, and inline note titles. |
| `dashboard` | Activates grid layout | Transforms the note into a responsive masonry grid structure. Converts standard callouts into floating dashboard cards. |
| `custom-timeline` | Activates timeline layout | Converts standard unordered lists into a split-view, CSS-only vertical chronology grid. |
