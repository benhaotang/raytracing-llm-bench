# WebGL Raytracing LLM Comparison

A simple comparison of GPT-5, Claude Opus 4.1, and Gemini 2.5 Pro on a complex WebGL raytracing challenge.

## Results

- **Gemini 2.5 Pro**: 93/120 (Best score, $1.31)
- **GPT-5**: 86/120 (Most sophisticated, $3.12)
- **Claude Opus 4.1**: 80/120 (Most expensive, $34.86)

## Test Details

Each model was given the same raytracing prompt requiring:
- Scene composition (wood table, stained glass, candle, etc.)
- Advanced rendering (refraction, dispersion, volumetric fog)
- Performance optimization
- Interactive controls

All tests used default API temperature with no agentic setups.

Prompts: [webgl.md](./webgl.md)

## Files

- `index.html` - Interactive comparison interface
- `chatgpt.html` - GPT-5 raytracing demo
- `claude.html` - Claude Opus 4.1 raytracing demo  
- `gemini.html` - Gemini 2.5 Pro raytracing demo
- `webgl.md` - Original challenge prompt
- `description.md` - Detailed scoring breakdown

## Demo

Visit [GitHub Pages](https://pages.github.com) to compare the implementations.

⚠️ This is a vibe test, not a scientific benchmark.