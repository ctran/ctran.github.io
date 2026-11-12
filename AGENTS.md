# AGENTS.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Current state

This is a personal site (`ctran.github.io`, a GitHub Pages user site) built as plain static files: `index.html` and `style.css`. There is no build step, package manager, tests, or CI. Preview by opening `index.html` in a browser, or run `python3 -m http.server` in the repo root.

`style.css` uses CSS variables on `:root` with a `prefers-color-scheme: dark` override, so new colors should be added as tokens there.

## Notes

- As a GitHub user site repo, the default branch (`main`) is what gets published to `https://ctran.github.io`.
