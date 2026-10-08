Obsidian Note Template
======================

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

This template demonstrates one way of using Obsidian for work.
The structure is organized to largely support individual contributor work that follows Agile development workflows, but can be adapted for other types of work and workflows.
Review the remainder of the README and the sample note vault in this repository for more details and examples.

Keyboard Short Cuts
-------------------

These short cuts are defined for Mac, but should work similarly on Linux and Windows.
Some of these are automatic, 

- `cmd + p`: Open the search bar for the command.
- `cmd + left arrow`: Show / hide the left toolbar.
- `cmd + right arrow`: Show / hide the right toolbar.

Managing Assets
---------------

You can decide where Obsidian should save dragged-and-dropped into a Markdown files.
I find it clearest to place them near the note itself, so within `Settings -> Files and links` I set the following two settings:

- `Default location for new attachments`: `In subfolder under current folder`
- `Subfolder name`: `Assets`

Required Plugins
----------------

**Calendar - Liam Cain:**
Use this plugin to have a calendar within your Obsidian interface.
I place this on the right sidebar to have it easily accessible.

**Dataview - Michael Brenan:**
For unique occasions, I need to timestamp something the moment it happens.
This plugin creates a useful set of timestamps such as `@time` `@Today`, or `@Tomorrow`.
Once you accept the tag it will convert into the actual value for the time or date.

**Excalidraw - Zsolt Viczian:**
I frequently use diagrams in my work and find it useful to be able to draw them directly in my notes.
This plugin pops up as as a tab in the left toolbar and you can press it to generate a new drawing.
You can then making a drawing and save it natively in your Obsidian interface.

**Metadata Menu - mdelobelle:**
Use this plugin for drop-down menus within file metadata.
I use this for pre-defined categories within notes.
For example, I use a `Priority` tag that has options of `low`, `medium`, and `high`.

**Natural Language Dates - Obsidian Community:**
I use dates within my notes to denote when something occured.
To standardize these references, I use this template to have my date format as `YYYY-MM-DD`.

**Templater - SilentVoid:**
The template tool within Obsidian is useful, but has limitations when creating files.
This templater plugin allows for custom fields such as automatically setting the date for `Date Created`.
Note that to use this plugin, you need to invoque `templater`, not `template`.

Snippets
--------

Inside of the `.obsidian` directory, we can add custom snippets to adjust how the interface works.
I use the following snippets:

- `no-strikethrough.css`:
I prefer to not draw a line through items that I check off.
This snippet removes the line and lets the check mark work in isolation.

```css
.markdown-preview-view :is(ul > li.task-list-item.is-checked) {
  text-decoration: none;
  color: var(--text-normal);
}
body {
  --checklist-done-decoration: none;
  --checklist-done-color: var(--text-muted);
}
```

Synchronizing Notes
-------------------

I backup my notes vault automatically, but do not sync my notes to a server to make them available on other devices.
However, there are tools to do this, including the native `Obsidian Sync` feature.
