---
name: photo-packshot
description: Create accurate product packshots and controlled background variants from user-provided product references. Use for studio product images, angle variants, and backdrop options that need a clear review process.
---

# Photo Packshot

A repeatable workflow for creating studio-style product images while keeping the real product, its packaging, and its printed details as the source of truth.

Before generating images, read the packshot workflow and prompt guide at references/packshot-workflow.md.

## Core principles

- Treat user-provided product photos and source artwork as the authority for packaging geometry, proportions, print, closures, and product appearance.
- Give each reference image a specific role in the prompt: product and composition, style and lighting, or supplementary product detail.
- Keep the product separate from the background description. Do not change brand marks, package text, materials, structure, or product details unless the user asks.
- Make one representative image for a new direction and let the user review it before generating a full set.
- Treat every generated image as an unreviewed candidate. Check product accuracy independently from style.
- Keep approved source images intact. Only mark an output approved after the user confirms it.

## Scope

This skill covers product packshots, camera-angle variants, and controlled background or lighting variants. For lifestyle scenes, first create and validate a separate scene plan with a small number of samples before extending this workflow.


