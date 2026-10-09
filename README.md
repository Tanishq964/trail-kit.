# 🌿 Trail Kit

Offline-first, open-source AI tools that get you off the screen and into the world.

Built for the DEV "Touch Grass" challenge. Everything runs locally with open-weight models, so it works on a trail with no signal, keeps your data on your device, and costs nothing to run.

## Tools

- 🐦 **Trail Birder**: record a bird call and identify the species on-device, even in airplane mode.
- 🌱 **Frost Gardener**: enter your local frost dates and see what to plant this week. A local LLM explains why.
- 🍁 **Foliage Run Club**: build group-run routes from open map data, ranked by tree cover and peak colour.

## Why open source?

- **No signal needed**: open weights run where cloud APIs can't.
- **Private**: your location and recordings never leave your device.
- **Swappable**: fine-tune or swap models without rewriting the app.
- **Free**: no per-call fees, so run clubs and school gardens can use it.

## Quick start

```bash
git clone https://github.com/YOUR-USERNAME/trail-kit
cd trail-kit
ollama pull llama3.2
python -m trailkit serve
```

To try the garden planner demo only, open `index.html` in your browser.

## Tech stack

- Ollama / llama.cpp for local inference
- An open bird-sound classification model
- OpenStreetMap data
- SQLite

## Contributing (Hacktoberfest welcome! 🎃)

Contributions of all sizes are welcome. Good first issues:

- Add frost-date presets for your region
- Add crops to the planner table
- Translate the UI into your language
- Benchmark a new open model for bird calls

Look for issues labelled `good first issue` and `hacktoberfest`. See [CONTRIBUTING.md](CONTRIBUTING.md) for how to open a pull request.

## License

MIT. See [LICENSE](LICENSE).
