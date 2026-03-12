# read-arxiv-paper

A skill for reading and summarizing arxiv papers by fetching the TeX source.

## Source

This skill was originally created by **Andrej Karpathy** as part of the [nanochat](https://github.com/karpathy/nanochat) project.

- **Original Location:** https://github.com/karpathy/nanochat/tree/master/.claude/skills/read-arxiv-paper
- **License:** See the original repository for licensing terms

## What It Does

Given an arxiv URL (e.g., `https://www.arxiv.org/abs/2601.07372`), this skill:

1. Normalizes the URL to fetch the TeX source (`/src/` instead of `/abs/`)
2. Downloads the `.tar.gz` source file
3. Unpacks and locates the main `.tex` entrypoint
4. Reads through all relevant source files
5. Produces a markdown summary with connections to relevant projects

## Usage

Provide an arxiv URL and the skill will handle the rest automatically.
