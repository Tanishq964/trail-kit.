🌿 Open source · Offline-first · Hacktoberfest friendly

# Trail Kit: make the screen the shortest part of your day.

Small open-weight models running on your own laptop or phone, so your bird ID, garden plan and fall-foliage run work with no signal and no account.

[Try the garden planner](#try)[Contribute](#contribute)

## Three tools, one local stack

### 🐦 Trail Birder

Record a call on the trail; an on-device bird-sound model names the species. Works in airplane mode.

### 🌱 Frost Gardener

Tell it your local frost dates; it tells you what to plant this week. A local LLM explains the “why”.

### 🍁 Foliage Run Club

Builds group-run routes from open map data, ranked by tree cover and peak colour.

## Why open matters here

### No signal needed

Trails have no bars. Open weights run where cloud APIs can't.

### Your data stays yours

Your location and recordings never leave the device.

### Swap and fine-tune

Tune a model on your region's birds or crops. Swap models without rewriting the app.

### Costs nothing to run

No per-call fees, so a run club or school garden can use it freely.

## Try it: what should I plant this week?

A rule-based demo of the Frost Gardener (the local-LLM explanations live in the repo). Enter your frost dates:

Last spring frost

First fall frost

## Run it locally

```
git clone https://github.com/YOUR-USERNAME/trail-kit
cd trail-kit
ollama pull llama3.2        # any open-weight model works
python -m trailkit serve    # runs fully offline
```

Stack: Ollama / llama.cpp for inference, an open bird-sound classifier, OpenStreetMap data, SQLite. Replace `YOUR-USERNAME` with your GitHub handle.

## Contribute this Hacktoberfest

Good first issues, all small and well scoped:

Add frost-date presets for your regiondata

Add crops to the planner tabledata

Translate the UI into your languagei18n

Benchmark a new open model for bird callsml

[About Hacktoberfest](https://hacktoberfest.com)

MIT licensed. Built for the DEV “Touch Grass” challenge. Go outside.