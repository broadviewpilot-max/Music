# Sonic Studio

Single-page AI music app built on the [Suno API](https://docs.sunoapi.org/). Users bring their own API key (get one at https://sunoapi.org/api-key).

**Features:** Describe-it and Custom song creation (V6 / V6 Wild / V6 Mini plus legacy models, style/weirdness/audio weight/variety, vocal gender, negative tags, personas, duration, reference media), AI lyrics writer, style booster, Studio (cover, extend, add vocals, add instrumental, mashup, file upload), sound & loop generator, library with player, karaoke timestamped lyrics, extend, replace section, WAV, stem split, MIDI, music video, cover art, persona creation, credit balance. Light, dark and system themes.

**Deploy:** static site on Netlify (`publish = "."`). `netlify.toml` proxies `/suno/*` → `api.sunoapi.org` and `/suno-upload/*` → the Suno file-upload host so the browser avoids CORS. The key is stored only in the user's browser.
