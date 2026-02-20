---
title: Global Illumination on mobile - Leo's World retrospective
image: /images/blog/il-mondo-di-leo/il-mondo-di-leo-cover.jpg
tags: [Unity] [Mobile] [Performance]
style: 
color: primary
description: 
external_url: 
---

Back in 2022 after a series of B2B titles I got the change to work on a title meant for the general public.
Even though it’s been a while since release, I think that the technical decisions I took still hold up quite well.

Since the project was meant to be released on mobile and that it would have a strong visual identity, correct planning was crucial from moment 0.

Requirements:
• 3/4 skinned meshes per environment as gameplay/toy elements
• Stable framerate
• Keep the build size as small as possible
• Retain the highest quality possible on textures (handpainted), animation backgrounds (npot) and animated characters
• Day/Night


Some technical decisions that worked particularly well:
• Used baked Global Illumination in Blender as a base, then painted over it to push stylization and readability.
• Built each environment as a single mesh and single unlit material since the camera was fixed which allowed tighter control and fewer draw calls.
• Kept everything intentionally lowpoly to stay within strict mobile constraints.
• Correct compression formats on textures
• Forward rendering


Other things that happened:
• Understand how to export high quality spritesheet from toon boom


Two assets I’m still particularly proud of:
• A stylized tree with a custom shader that allows flowers to “pop” dynamically.
• A rigged poster with an unroll control to animate it smoothly in-engine.

Working within mobile limitations really reinforced something I enjoy: constraints don’t limit creativity — they sharpen it.