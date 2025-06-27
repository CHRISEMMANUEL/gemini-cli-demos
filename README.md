# gemini-cli-demos

This repository contains Demos-in-a-box for Gemini CLI.

Available demos:

| Status | Demo | Category | Description |
|---|---|---|---|
| 🚧 | [auto-slide-creator](./demos/auto-slide-creator) | Google Workspace | This demo showcases how `gemini-cli` is able to create Google Slides. Missing features: image generation, proper formatting for backticks and bullet points. |
| 🚧 | [git-investigation](./demos/git-investigation) | Git | This demo will showcase git investigation capabilities. |
| ✅ | [sqlite-investigation](./demos/sqlite-investigation) | Database | This demo showcases how `gemini-cli` is able to read/write/understand a sqlite3 database and generate an E/R schema from it. |

## INSTALL

To install: `npx @gemini/gemini-cli`.
More info: https://github.com/google-gemini/gemini-cli

## CI/CD

We moved to LLM-Ops Gemini-based ci/cd, see for instance: `just update-readme`

```bash
$ gemini -a -p "Update README with [possibly new] articles under demos/"
I will update the main `README.md` to include the demos I found in the `demos/` directory. First, I'll list the contents of the `demos/` directory to identify all the demos. Then, for each demo, I will read its `STATUS.md` file to gather the necessary information to update the main `README.md`.
```

## CONTRIBUTING

Please do contribute to this repo. Add a new folder and make sure it's complete with:
- purpose
- repeatable code
- tests.

Every folder should have:

1. A `GEMINI.md` which shows users (and Gemini!) the purpose of what you're trying to build.
2. A `SCRIPT.md` , this is a README you're going to read if recording a video, basically.
3. A `README.md` which teases users on what this is about. This is linked from main README, so make it nice, engaging,
   short and full of images/screenshots which show the art of possible.
