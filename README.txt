AI HVAC Diagnostic Copilot — V5.2

Critical fix:
The previous version stopped executing JavaScript during initial render because camera code referenced Edit Mode state before it had been initialized. This prevented autoplay, Play, and camera zoom from running.

V5.2:
- fixes the JavaScript initialization error
- autoplay starts as the animation enters the viewport
- adds IntersectionObserver fallback
- Play/Pause button is much larger
- camera zoom is intentionally stronger and easier to see
- 45-second timeline retained
- Edit Mode / drag / resize / dynamic wires retained
