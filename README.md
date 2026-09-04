# Bay Area Robotics Calendar

Static site for the weekly robotics / embodied-AI / AI-agent event sweep.
`index.html` is fully self-contained — no build step, no dependencies.

Regenerate from the newest sweep:

```bash
cd ~/robotics-events-scout
python3 -m scout.site --fresh   # collect, then rebuild site/index.html
python3 -m scout.site           # rebuild from the cached sweep only
```

Publish (GitHub Pages serves this folder from `main`):

```bash
cd ~/robotics-events-scout/site
git add -A && git commit -m "Update calendar" && git push
```
