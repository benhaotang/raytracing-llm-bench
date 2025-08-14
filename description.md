# GPT 5
- 5 shots to see anything
- Another 4 shots to add the freeze in time function
Pros:
- Most sophisticated geometry, good wood details.
- Good control panel with fine adjustments.
- No need human intervention, just provide error and problem it will come to a solution.
Cons:
- Worst performance.
- Visual tearing and artifacts.
- Somehow it always start up-side-down(fixed this 3 shots but failed, in the end just ask it to add a flip button).

## Ray Tracing Scene Score: 86/120

### Scene Composition (26/55)
- ✅ Wood table: 5/5
- ✅ Stained glass window: 5/5  
- ✅ Ambient lighting: 5/5
- ✅ Candle: 5/5
- ？ Glass vase with flowers: 3/10 (-2 for flowers not looking like flowers)
- ？ Crystal ball: 3/5 (-2 for not transparent)
- ❌ Magnifying glass + newspapers: 0/10
- ❌ Pebble brick walls: 0/10

### Rendering Techniques (60/65+)
- ✅ Refraction: 10/10
- ✅ Dispersion: 10/10
- ✅ Reflection: 10/10
- ？ Ray tracing optimization: 5/10 (5 for good control, -5 for bad performance)
- ✅ Volumetric fog: 10/10
- ✅ Caustics: 5/5
- ✅ Bloom: 5/5
- ✅ Chromatic aberration: 5/5
- ❌ Depth of field 0/5 (very bad, no Bonus here.)

# Gemini
- 2 shots to see anything
- 2 shots to fix geometry
- 3 shots to add the freeze in time function
Pros:
- Visually nice, have the most details as required, good instruction following.
- No need human intervention, Generation is fast, just provide error and problem it will come to a solution.
- Very good fps.
Cons:
- The scene is a bit simple.
- Less fine control on the control panel.
- Provide depth of field but no focal distance settings making it useless.

## Ray Tracing Scene Score: 93/120

### Scene Composition (37/55)
- ✅ Wood table: 5/5 
- ✅ Stained glass window: 5/5 
- ✅ Ambient lighting: 5/5 
- ✅ Candle: 7/5 (+2 because it have live flame effects)
- ？ Glass vase with flowers: 4/10 (-3 for flowers, -3 for the vase floating and too simple)
- ✅ Crystal ball: 5/5 (transparent sphere with reflections visible)
- ？ Magnifying glass + newspapers: 1/10 (1 for attempt)
- ？ Pebble brick walls: 5/10 (have pebble texture, but not in bricks)

### Rendering Techniques (56/65+)
- ✅ Refraction: 10/10
- ✅ Dispersion: 10/10
- ✅ Reflection: 10/10
- ✅ Ray tracing optimization: 10/10
- ✅ Volumetric fog: 10/10 
- ？ Depth of Field: 1/5 (better than GPT-5, but still not usable)
- ✅ Volumetric lighting 5/5

# Claude

- 1 shot to see anything(but the lighting is wrong).
- After that there is constant shader compiling issue, in the end it took a total of 14 shots to reach this final result.
Pros:
- Good rendering process, fast and stable, good FPS.
- Only model that made a Magnifying glass and 1 shot the prompt.
- The animation is good with fine controls of Depth of Field.
Cons:
- Need heavy human intervention after initial prompt(because it always hit shader compiling error without useful error message as feedback), I need to manually fix tune matching and shader code to move on.
- Strange artifacts.
- Most expensive(almost $2 per shot).

## Ray Tracing Scene Score: 80/120

### Scene Composition (31/55)
- ？ Wood table: 3/5 (not very good wood grain)
- ✅ Stained glass window: 5/5
- ✅ Ambient lighting: 5/5
- ✅ Candle: 5/5 
- ❌ Glass vase with flowers: 0/10
- ✅ Crystal ball: 5/5 (multiple spheres with reflections and refractions)
- ？ Magnifying glass + newspapers: 5/10 (-5 for missing newspapers)
- ？ Pebble brick walls: 3/10 (have brick lines, but not correct texture)

### Rendering Techniques (49/65+)
- ✅ Refraction: 10/10
- ✅ Dispersion: 10/10
- ✅ Reflection: 10/10
- ✅ Ray tracing optimization: 10/10
- ❌ Volumetric fog: 0/10 
- ？ Depth of Field: 4/5 (Have bokeh effect, but tend to be too strong)
- ✅ Caustics: 5/5