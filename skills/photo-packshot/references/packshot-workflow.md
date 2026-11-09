# Packshot workflow and prompt guide

## Select the project references

Use the references supplied for the current product and task. They may include:

- **Approved style master:** establishes a confirmed camera angle, framing, or studio look.
- **Real product photos or original artwork:** establish packaging geometry, printed details, closures, materials, and the actual product appearance.
- **Style sample:** establishes background tone, lighting, and shadow treatment only.
- **Review index:** records which candidate images have been approved and which remain under review.

Do not assume a reference is approved just because it exists. Check its status and intended use. Prefer a clear product photo from the same angle as the desired output. For small print, barcodes, certification marks, and package backs, use a close-up or original artwork; image models may not reproduce these reliably.

## Assign a role to every reference

Tell the image model what each image controls:

1. **Product and composition reference:** the camera angle, product pose, crop, placement, and relative scale.
2. **Style reference:** the background color, tonal gradient, lighting, and shadow. It must not redefine the product or package design.
3. **Supplementary product reference (optional):** real print, seams, closures, material, or product appearance. It may have unsuitable lighting or a distracting background, so do not copy those unless asked.

Use one primary composition reference per output. Add other images only to supply specific details.

## Choose a background direction

Describe the requested background in concrete terms. For example:

- **Neutral light gray:** near-white, softly graduated, with a clean high-key studio look.
- **Pale sage:** a near-white center with a subtle, low-saturation gray-green toward the edges.
- **Warm ivory:** a near-white center with a restrained warm cream tone toward the edges.

Keep the package neutral and avoid strong color spill. Start a new palette with one representative angle so the user can check the gradient and shadow before extending it to other views.

For shadows, describe the contact area and falloff: slightly clearer next to the product, then progressively wider, softer, and lighter. Avoid hard outlines, dark halos, and an unintended floating appearance.

## Reusable prompt template

Replace the bracketed details and provide the references in the same order described below.

~~~
Image 1 defines the exact product and camera composition. Image 2 defines only the background, tonal treatment, lighting and shadow style. [Optional: Image 3 is a real product reference for ...]

Preserve image 1's exact [view / pose / crop / relative scale]. Keep the product geometry, package proportions, printed marks, logo, seams, closures, material details and [specific structure] faithful to the product references. Do not invent or rewrite text, change the product, or alter its proportions.

Change only the background and lighting/shadow. Use [requested palette and gradient], with soft high-key studio lighting. Keep the package neutral in color. Create a soft contact and cast shadow that starts near the contact area and gradually feathers and fades outward. No hard edges, dark halo, or charcoal field. No extra props, text, or graphics. Keep the framing and product placement.
~~~

### Floating product

Use only when the composition reference already shows a floating product:

~~~
Retain the slight floating gap shown in image 1. Keep the cast shadow broad, soft and low-opacity beneath the product, with a smooth gradual falloff and no hard outline.
~~~

### Flexible pouch

Adapt to the actual package design:

~~~
Preserve the real pouch aspect ratio, top and bottom seals, artwork, and print placement. Keep the packet neatly presented with only subtle natural volume; remove distracting dents or irregular wrinkles without changing its true outline or seal widths.
~~~

### Food products

Use only when the product is food and the supplied reference establishes its appearance:

~~~
Preserve the actual product count, size range and package-to-product ratio from the product reference. Keep the food's real surface, shape, and batch-accurate color; do not make it glossy, oversized, or artificially uniform.
~~~

## Generate, review, and archive

1. Confirm the requested views, the composition reference for each view, and the background direction.
2. For a new background or lighting direction, generate one representative sample and get the user's review before making a full set.
3. Give each output one primary composition reference. State clearly that style references control only the background and lighting.
4. Save outputs in a candidate folder, grouped by direction or view. Use filenames that include an index, view, and review status. Keep a review index with the file name, references, prompt version, and status.
5. Inspect each image for product silhouette and perspective, visible package faces, structural details, proportions, readable text, barcodes and marks, color shifts, crop, pose, and shadow.
6. Keep inaccurate results as candidates for revision. After the user confirms an image, copy it into the approved-output area. Do not move or overwrite the frozen source or style master.

## Limits

Image generators redraw product details. Even a prompt that requests only a background change cannot guarantee unchanged text, dimensions, geometry, or color. Treat generated images as visual candidates. For exact labels, regulatory marks, or packaging geometry, compare with the source photos or artwork and consider compositing a real product cutout over a generated background.

Do not invent product performance, health benefits, certifications, or usage claims. Lifestyle scenes are a separate workflow: agree on a scene and composition, then validate a small sample set before scaling it.
