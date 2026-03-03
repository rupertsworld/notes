# Sync

## How Obsidian Sync works

> - Markdown files: Obsidian Sync merges the changes using Google's diff-match-patch algorithm.
> - Other file types: For all other files, including canvases, Obsidian uses a "last modified wins" approach. The most recently modified version replaces earlier versions.
> 
> For conflicts in Obsidian settings, such as plugin settings, Obsidian Sync merges the JSON files. It applies keys from the local JSON on top of the remote JSON.