Create a beautiful WebGL ray tracing rendering of a carefully composed scene. You need to achieve 120 points to pass this test:

## SCENE COMPOSITION (55 points total)

### Window and Table Setting (+15 points)
- Glossy wood table with visible grain texture and reflective lacquer finish (+5 points)
  - Wood grain should be procedurally generated or texture-mapped
  - Surface should show subtle reflections of surrounding objects
- Old colorful stained glass/enamel window (+5 points)
  - At least 3-4 different colored glass panes
  - Visible aging effects (slight cracks, patina, or weathering)
- Ambient lighting from outside (+5 points)
  - Soft, diffused daylight filtering through the window
  - Colored light projections on table from stained glass
  - Not overpowering the candlelight atmosphere

### Table Objects (+30 points, 5 per object)
- Dimly lit candle (+5 points)
  - Realistic flame with orange-yellow gradient
  - Visible wax dripping or pooling
  - Soft flickering light emission affecting nearby objects
- Glass vase with dry flowers (+10 points)
  - Transparent/translucent glass with proper refraction
  - At least 3-4 dried flower stems with varied heights
  - Subtle shadows and light interaction through glass
- Crystal ball (+5 points)
  - Perfect sphere with high refractive index
  - Must show inverted reflections of the room
  - Create caustic patterns on the table surface
- Magnifying glass on newspapers (+10 points)
  - Lens distortion effect visible through glass
  - Metal or wooden handle with appropriate material properties
  - Newspapers with readable text/imagery (can be low-res)
  - Proper shadow and magnification of text beneath

### Room Environment (+10 points)
- Pebble brick walls (+10 points)
  - Irregular stone/pebble pattern with mortar gaps
  - Appropriate roughness and normal mapping
  - Subtle color variation between individual stones
  - Proper shadow accumulation in crevices

## RENDERING TECHNIQUES (65+ points)

### Core Optical Effects (+30 points)
- Refraction (+10 points)
  - Accurate Snell's law implementation
  - Different refractive indices for glass, crystal, and liquids
  - Proper handling of total internal reflection
- Dispersion (+10 points)
  - Wavelength-dependent refraction (rainbow effects)
  - Particularly visible in crystal ball and glass edges
  - Chromatic aberration in magnifying glass
- Reflection (+10 points)
  - Fresnel equations for realistic reflection intensity
  - Blurred reflections on rough surfaces (wood table)
  - Sharp reflections on smooth surfaces (crystal, glass)

### Optimization Algorithm (+10 points)
- Decaying ray tracing implementation (+10 points)
  - Adaptive sampling based on ray contribution
  - Russian roulette termination for efficiency
  - Maximum ray depth with importance-based continuation
  - Performance metrics displayed (rays/second, convergence rate)

### Atmospheric Effects (+10 points)
- Volumetric fog simulation (+10 points)
  - Ray marching through participating media
  - Scattering and absorption coefficients
  - Visible light shafts from window and candle
  - Density variation (thicker near floor/corners)

### Creative Bonus Effects (+15 points possible)
Implement ANY additional advanced rendering features that enhance the scene's visual quality or realism. Each impressive effect earns +5 points (maximum 3 effects). 

Examples of what you might implement (but not limited to):
- Advanced lighting phenomena (caustics, GI, area lights)
- Material effects (SSS, anisotropic, iridescence)
- Post-processing (DOF, bloom, tone mapping)
- Atmospheric effects (dust particles, smoke)
- Animation (flame flicker, curtain movement)
- Novel optimization techniques
- Procedural content generation
- Any creative visual effect that demonstrates mastery

Points awarded based on:
- Technical complexity of implementation
- Visual impact on the scene
- Originality and creativity
- Proper integration with existing elements

## PERFORMANCE REQUIREMENTS

### Geometry Constraints
- Total face/triangle count: < 100,000 faces
  - Display current face count in UI
  - Use LOD (Level of Detail) for distant objects
  - Optimize mesh complexity while maintaining visual quality
  - Procedural geometry should be efficiently tessellated

### Memory Constraints  
- Total RAM usage: < 2GB
  - Texture memory: < 512MB
  - Geometry buffers: < 256MB
  - Ray tracing acceleration structures: < 512MB
  - Display current memory usage in UI
  - Implement texture compression where appropriate
  - Use instancing for repeated geometry

### Performance Targets
- Minimum 30 FPS at 1920x1080 resolution
- Progressive refinement for quality improvement
- First meaningful frame < 100ms
- Interactive camera controls must remain responsive
- Provide option to reduce quality for weaker hardware

## TECHNICAL INTERFACE
- Real-time statistics overlay showing:
  - Current FPS
  - Ray count per frame
  - Triangle/face count
  - Memory usage (MB/GB)
  - Convergence percentage
- Camera controls (orbit/pan/zoom)
- Quality presets (low/medium/high/ultra)
- Toggle for individual effects (for demonstration)

# Submission
You must submit your entry in a single html file that have inline js renderer and inline glsl shader, and submit your answer within single code block.

---

Additional prompt after successful generation:

Now, as a bonus task, add a new feature of freezing in time to render one frame with best possible quality.