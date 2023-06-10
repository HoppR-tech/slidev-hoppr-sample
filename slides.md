---
theme: ./theme
background: https://source.unsplash.com/collection/94734566/1920x1080

themeConfig:
  color: "#F3EFF5"
  background: "#131415"

  code-background: "#0F131E"
  code-border: "#242d34"

  accents-purple: "#5865F2"
  accents-yellow: "#FFF154"
  accents-red: "#F85352"
  accents-lightblue: "#00CCA5"
  accents-blue: "#54AAFF"
  accents-vulcan: "#0E131F"

  default-headingBg: var(--slidev-theme-accents-yellow)
  default-headingColor: var(--slidev-theme-accents-vulcan)
  default-background: var(--slidev-theme-background)

  center-headingBg: var(--slidev-theme-accents-blue)
  center-headingColor: var(--slidev-theme-accents-vulcan)
  center-background: var(--slidev-theme-background)

  cover-headingBg: var(--slidev-theme-accents-purple)
  cover-headingColor: var(--slidev-theme-accents-vulcan)
  cover-background: var(--slidev-theme-background)

  section-headingBg: var(--slidev-theme-accents-lightblue)
  section-headingColor: var(--slidev-theme-accents-vulcan)
  section-background: var(--slidev-theme-background)

  aboutme-bg: var(--slidev-theme-color)
  aboutme-color: var(--slidev-theme-background)
  aboutme-helloBg: var(--slidev-theme-accents-yellow)
  aboutme-helloColor: var(--slidev-theme-background)
  aboutme-nameColor: var(--slidev-theme-accents-red)

title: Slidev - HoppR
---

# Slidev - HoppR

Created by [Maxime Deroullers](https://www.linkedin.com/in/maxime-deroullers-1b5791137/)


---
layout: about-me
helloMsg: Hello!
name: Maxime Deroullers
imageSrc: /my-profile-picture.png
job: Agency Leader @ HoppR
line1: "#President @ Cloud Alpes"
line2: "#Co-Organizer @ Cloud Nord"
social1: "@mderoullers"
---

---
layout: cover
---

# Cover title

Subtitle for the cover

---
layout: section
---

# Section title

Subtitle for the section

---
layout: center
---

# Center title

Subtitle for the center layout

---

# Code with Shiki and The unnamed theme

The code highlighting is powered by Shiki and [The unnamed - VS Code theme](https://marketplace.visualstudio.com/items?itemName=eliostruyf.vscode-unnamed-theme)

```ts
interface User {
  id: number
  firstName: string
  lastName: string
  role: string
}

function updateUser(id: number, update: Partial<User>) {
  const user = getUser(id)
  const newUser = { ...user, ...update }
  saveUser(id, newUser)
}
```

---

# Table 

| Title | Description | Default |
| --- | --- | --- |
| `layout` | The layout to use for the slide | `default` |
| `theme` | The theme to use for the slide | `the-unnamed` |
| `highlighter` | The highlighter to use for the slide | `shiki` |
| `background` | The background to use for the slide | `none` |

## Content test underneath

Some content to place here

---

# Todo 

- [ ] Add a todo list
- [ ] Add a todo list
- [x] Add a todo list

---

# Heading 1

## Heading 2

### Heading 3

#### Heading 4

##### Heading 5

> **Info**: This is a note

---

# What is Slidev?

Slidev is a slides maker and presenter designed for developers, consist of the following features

- 📝 **Text-based** - focus on the content with Markdown, and then style them later
- 🎨 **Themable** - theme can be shared and used with npm packages
- 🧑‍💻 **Developer Friendly** - code highlighting, live coding with autocompletion
- 🤹 **Interactive** - embedding Vue components to enhance your expressions
- 🎥 **Recording** - built-in recording and camera view
- 📤 **Portable** - export into PDF, PNGs, or even a hostable SPA
- 🛠 **Hackable** - anything possible on a webpage

<br>
<br>

Read more about [Why Slidev?](https://sli.dev/guide/why)


---

# Navigation

Hover on the bottom-left corner to see the navigation's controls panel

### Keyboard Shortcuts

|     |     |
| --- | --- |
| <kbd>space</kbd> / <kbd>tab</kbd> / <kbd>right</kbd> | next animation or slide |
| <kbd>left</kbd>  / <kbd>shift</kbd><kbd>space</kbd> | previous animation or slide |
| <kbd>up</kbd> | previous slide |
| <kbd>down</kbd> | next slide |

---
layout: image-right
image: 'https://source.unsplash.com/collection/94734566/1920x1080'
---

# Code

Use code snippets and get the highlighting directly!

```ts
interface User {
  id: number
  firstName: string
  lastName: string
  role: string
}

function updateUser(id: number, update: Partial<User>) {
  const user = getUser(id)
  const newUser = { ...user, ...update }
  saveUser(id, newUser)
}
```

---
layout: center
class: "text-center"
---

# Learn More

[Documentations](https://sli.dev) / [GitHub Repo](https://github.com/slidevjs/slidev)
