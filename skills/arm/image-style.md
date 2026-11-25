# ARM User Facility — Image Direction

Scientific and atmospheric instrumentation imagery: cumulus and stratocumulus cloud fields, atmospheric observatories, radar domes, radiosonde launches, research aircraft, and clean data exhibits. Real observatory hardware, field sites, or personnel are represented via labeled placeholder frames unless supplied by the user; atmospheric sky backgrounds use the baked official ARM binary-cloud textures.

Prompt template: `{subject}, atmospheric science photography, expansive sky with cumulus clouds, natural daylight, clean scientific documentary style, deep navy and sky blue tones, high dynamic range, crisp detail`

Negative prompt: logos, trademarks, watermark, text overlay, neon cyberpunk, cartoon, clipart, people faces, futuristic sci-fi clutter

Search-query template: `{subject} atmospheric weather radar clouds research observatory`

Decision rules:
- `gradient | background | sky | clouds` → AI default
- `instrument | radar | observatory | aircraft` → stock
- `person | scientist | crew` → ask
- `building | facility | site` → stock
- `chart | diagram | profile` → AI default
