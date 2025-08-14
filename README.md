# WebGL Raytracing LLM Comparison

A simple comparison of GPT-5, Claude Opus 4.1, and Gemini 2.5 Pro on a complex WebGL raytracing challenge.

Demo site [https://benhaotang.github.io/raytracing-llm-bench/](https://benhaotang.github.io/raytracing-llm-bench/)

The homepage and this README is mainly written by claude code, the scoring and description.md is written by a **biased human** like me.

## Results

- **Gemini 2.5 Pro**: 93/120 (Best score, $1.31)
- **GPT-5**: 86/120 (Most sophisticated, $3.12)
- **Claude Opus 4.1**: 80/120 (Most expensive, but the only one that 1-shot with a working renderer, $34.86)

## Test Details

Each model was given the same raytracing prompt requiring:
- Scene composition (wood table, stained glass, candle, etc.)
- Advanced rendering (refraction, dispersion, volumetric fog)
- Performance optimization
- Interactive controls

All tests used default API temperature with no agentic setups.

Prompts: [webgl.md](./webgl.md) for WebGL and [webgpu.md](./webgpu.md) for WebGPU
> I only tested with WebGL because at least when I tested with GPT-5 pro with my TEAM sub, after 8 shots still nothing renders due to browser standards/compatibility (tested with latest Chromium). As a result, I don't want to waste more money on this until WebGPU support is more mainstreamed.

Raw prompt before being expanded by claude opus 4.1
```
Make a beautiful WebGPU ray tracing rendering of a carefully set scene, you need to get 120 points to pass this test:
- a glossy wood table next to an old colorful enamel window, there is some light coming from outside, but not too much (+15 points)
- on the table there is a dimly lit candle, next to it is a glass vase with some dry flowers, a crystal ball, a magnifier on some casually set newspapers (+30 points, meaning 5 per object)
- the room is made of pebble bricks (+10 points)
for rendering
- need to include basic refraction, dispersion and reflection effects (+30 points)
- simulate with optimization methods like a decaying ray strength to save on computational power (+10 points)
- simulate volumetric fog (+10 points)
- any other additional effects to the renderer will lead you to higher points, one additional lighting effect will land you an additional 5 points
```

## Files

- `index.html` - Interactive comparison interface
- `chatgpt.html` - GPT-5-High raytracing demo
- `claude.html` - Claude Opus 4.1-Thinking raytracing demo  
- `gemini.html` - Gemini 2.5 Pro raytracing demo
- `webgl.md` - Original challenge prompt
- `description.md` - Detailed scoring breakdown

## Demo

Visit [https://benhaotang.github.io/raytracing-llm-bench/](https://benhaotang.github.io/raytracing-llm-bench/) to compare the implementations.

⚠️ **This is a vibe test, not a scientific benchmark.**

## Gallery

<img width="3106" height="1970" alt="2025-08-14 01 26 03 localhost 449fce7184a6" src="https://github.com/user-attachments/assets/fd72ca35-b78b-499c-8f1c-e8733b224700" />
<img width="3114" height="1970" alt="2025-08-14 03 39 17 localhost 5287b312345f" src="https://github.com/user-attachments/assets/838321f6-f89f-40ea-a408-710559c05d79" />
<img width="3114" height="1970" alt="2025-08-14 04 00 45 localhost ec45abbafafe" src="https://github.com/user-attachments/assets/b3a5e520-0b86-42e3-9fb5-3bb8117a4bbe" />
