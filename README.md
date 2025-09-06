# Ads Creator — Black Forest Labs Hackathon (n8n workflow) 🚀🎨

A lightweight n8n workflow built for the Black Forest Labs hackathon that turns calendar events into ready-to-use social media ads, short videos, and SEO keyword suggestions for maximum reach. ✨

This project demonstrates an automated pipeline that:

- 📅 reads events from a calendar
- ✍️ generates ad copy and SEO keywords using an LLM
- 🖼️ produces image-based ads and short video clips using Flux Kontext model
- 📧 finalizes the report and sends it as an email

Examples of generated ads are available in `examples/generated_ads/`.

## Use case 🌟

As a marketing manager I would like to have all my assets for social media campaigns ready to go before any holiday or event and this automation helps to be ready for any event and make the social media push on time

## Quick overview 🔍

Inputs

- A calendar event (title, description, start/end times, location, optional image) 📆

Outputs

- 🖼️ Generated ad images (PNG/JPEG) and short videos (MP4) suitable for social media
- 🔑 Suggested SEO keywords (JSON or plain text)
- ✉️ Exported assets via email

## Prerequisites ✅

- An n8n instance (cloud or self-hosted)
- Credentials for Google Calendar (or your calendar provider) 🔐
- An LLM API key (Gemini or other) for generating copy and keywords 🧠
- Image generation service credentials from Black Forest 🖼️
- Video generation service credentials (custom video builder & Eleven Labs) 🎬

## Quick start (import into n8n) 🚀

1. Open your n8n editor 🧰
2. Import the workflow JSON (this repo contains only README and example outputs — add the exported workflow JSON here or paste it in the editor) 📥
3. Configure credentials for the nodes (Google Calendar, Gemini, image provider, etc.) 🔧
4. Test with a sample calendar event. Check `examples/generated_ads/` for sample outputs that illustrate expected results 👀

## Examples 🖼️

See `examples/generated_ads/` for sample images produced during the hackathon.

Files included in this repo (examples)

- `examples/generated_ads/sample (1).png`
- `examples/generated_ads/sample (2).png`
- `examples/generated_ads/sample (3).png`

These are example outputs — the live workflow can produce different variants depending on event content and API prompts.

### Example gallery 🌟

Below are thumbnails of generated assets included in `examples/generated_ads/` — click to view the full image.

[![Calendar Event](examples/calendar_event/image.png)](<examples/generated_ads/sample%20(1).png>)

Generated Assets:

<video controls width="640" poster="examples/generated_ads/image.png">
  <source src="examples/generated_ads/stitched.mp4" type="video/mp4">
  Your browser does not support the video tag. Download the video: [stitched.mp4](examples/generated_ads/stitched.mp4)
</video>

[![Sample 1](<examples/generated_ads/sample%20(1).png>)](<examples/generated_ads/sample%20(1).png>)

[![Sample 2](<examples/generated_ads/sample%20(2).png>)](<examples/generated_ads/sample%20(2).png>)

[![Sample 3](<examples/generated_ads/sample%20(3).png>)](<examples/generated_ads/sample%20(3).png>)

Report Generated

[![Report generated](examples/report/image.png)](examples/report/image.png)
