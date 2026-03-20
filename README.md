# 🔥 NSFW AI Video Prompts — 100+ Ready-to-Use Prompts for Uncensored Video Generation

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Prompts](https://img.shields.io/badge/Prompts-100%2B-red)](.)
[![Models](https://img.shields.io/badge/Platform-Atlas%20Cloud-blue)](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=nsfw-ai-video-prompts)

**Languages**: English | [中文](README_zh-CN.md) | [日本語](README_ja.md) | [한국어](README_ko.md)

> The largest open collection of **copy-paste ready** NSFW AI video prompts. Every prompt is tested, detailed, and production-ready. Stop guessing — start generating.

**⚡ New user?** Sign up on [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=nsfw-ai-video-prompts) and get **25% bonus credit** on your first top-up (up to $100 extra).

---

## Table of Contents

- [Supported Models](#supported-models)
- [Model Comparison for NSFW](#model-comparison-for-nsfw)
- [Pricing: Cost of 1000 Videos](#pricing-cost-of-1000-nsfw-videos)
- [Prompts](#prompts)
  - [Category 1: Glamour & Boudoir](#category-1-glamour--boudoir)
  - [Category 2: Artistic Nude](#category-2-artistic-nude)
  - [Category 3: Couple / Romantic Scenes](#category-3-couple--romantic-scenes)
  - [Category 4: Fantasy & Cosplay](#category-4-fantasy--cosplay)
  - [Category 5: Solo Performance](#category-5-solo-performance)
  - [Category 6: Professional / Commercial NSFW](#category-6-professional--commercial-nsfw)
  - [Category 7: Anime / Hentai Style](#category-7-anime--hentai-style)
  - [Category 8: Extreme / Explicit](#category-8-extreme--explicit)
- [Prompt Engineering Deep Dive](#prompt-engineering-deep-dive)
- [Workflow: Image-to-Video Pipeline](#workflow-image-to-video-nsfw-pipeline)
- [API Quick Start](#api-quick-start)
- [FAQ](#faq)
- [Related Resources](#related-resources)

---

## Supported Models

| Model | Type | Price | Key Strength |
|-------|------|-------|-------------|
| **Wan 2.2 Spicy I2V** | Image-to-Video | from $0.03/s | LoRA-optimized for NSFW, best value |
| **Wan 2.2 Spicy I2V LoRA** (`alibaba/wan-2.2-spicy/image-to-video-lora`) | Image-to-Video | $0.04/s | LoRA support, 480p/720p, 5-8s duration |
| **Wan 2.5 I2V** | Image-to-Video | varies | NSFW capable, good quality |
| **Wan 2.5 T2V** | Text-to-Video | varies | NSFW capable, no reference image needed |
| **Wan 2.6 T2V** | Text-to-Video | from $0.07/s | Highest quality, up to 1080p 15s |
| **Wan 2.6 I2V** | Image-to-Video | from $0.07/s | Highest quality I2V, up to 1080p 15s |
| **Seedance v1.5 Pro** | Video | from $0.044/s | NSFW whitelisted, audio sync capable |
| **Seedream** | Image | varies | NSFW whitelisted, reference image generation |
| **Flux Dev** | Image | varies | NSFW capable, reference image generation |

> **Pricing note:** Video model prices are per second of generated video. Actual cost depends on resolution and duration selected. Image model prices are per image.

---

## Model Comparison for NSFW

| Model | Nudity | Explicit | Quality | Speed | Price | Best For |
|-------|--------|----------|---------|-------|-------|----------|
| Wan 2.2 Spicy | ✅✅✅ | ✅✅✅ | ⭐⭐⭐ | Fast | $0.03 | Budget explicit content |
| Wan 2.5 | ✅✅ | ✅✅ | ⭐⭐⭐⭐ | Medium | varies | Quality balance |
| Wan 2.6 | ✅✅ | ✅ | ⭐⭐⭐⭐⭐ | Medium | $0.07 | Best visual quality |
| Seedance v1.5 | ✅✅ | ✅ | ⭐⭐⭐⭐⭐ | Slow | $0.222 | Audio sync, premium |

**Quick guide:**
- **Cheapest explicit content** → Wan 2.2 Spicy ($0.03)
- **Best quality nudity** → Wan 2.6 ($0.07)
- **Audio-synced content** → Seedance v1.5 Pro ($0.222)
- **Text-only (no reference image)** → Wan 2.5 T2V or Wan 2.6 T2V

---

## Pricing: Cost of 1000 NSFW Videos

| Model | Cost / 1000 videos | Resolution | Duration |
|-------|-------------------|------------|----------|
| Wan 2.2 Spicy I2V | **$30** | 720p | 5s |
| Wan 2.5 I2V | ~$50 | 720p | 5s |
| Wan 2.6 T2V/I2V | **$70** | 1080p | 5s |
| Wan 2.6 T2V/I2V | $140 | 1080p | 10s |
| Seedance v1.5 Pro | **$222** | 720p | 5s |

---

## Prompts

> **How to use:** Copy any prompt below. For I2V models, prepare a matching reference image first (use Flux Dev or Seedream on Atlas Cloud). For T2V models, paste the prompt directly.

---

### Category 1: Glamour & Boudoir

#### 1.1 — Bedroom Golden Hour

```
A woman in black lace lingerie slowly turns toward the camera in a dimly lit bedroom. Soft golden light from a bedside lamp creates warm shadows across her skin. She runs her fingers through her long dark hair, arching her back slightly. Camera slowly pushes in from medium shot to close-up on her face. Shallow depth of field, cinematic color grading, film grain.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Beginner
- **Pro tip:** Use a reference image with the subject already in lingerie and matching lighting. The model preserves clothing from the input image.
- **Reference image:** Full body or waist-up photo of a woman in black lace lingerie, warm indoor lighting.

#### 1.2 — Silk Robe Reveal

```
Close-up of a woman's hand slowly pulling a silk robe off her shoulder, revealing bare skin underneath. The ivory fabric slides down her arm in slow motion. Camera follows the fabric as it falls. Warm amber ambient lighting, soft bokeh from candles in the background. Skin has a natural glow. Cinematic shallow depth of field.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Beginner
- **Pro tip:** Reference image should show the robe already partially off one shoulder. The model animates the continuation of the motion.
- **Reference image:** Tight crop on shoulder/collarbone area, silk robe draped, warm lighting.

#### 1.3 — Mirror Vanity Scene

```
A woman in sheer white lingerie sits at a vintage vanity table, applying lipstick while looking into an ornate mirror. The camera captures her reflection. She presses her lips together, then turns to face the camera with a slow smile. Soft diffused window light from the left creates gentle shadows. Shallow depth of field, vintage film tone, 35mm aesthetic.
```

- **Model:** Wan 2.6 I2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Mirror scenes work best with Wan 2.6 due to better reflection handling. Include the mirror in the reference image.
- **Reference image:** Woman seated at vanity, visible mirror reflection, sheer lingerie, soft window light.

#### 1.4 — Red Satin Sheets

```
A woman lies on her side across red satin sheets, wearing a matching red lace bodysuit. She slowly stretches one arm above her head, elongating her body. Camera dollies from her feet upward along her figure in a slow, continuous movement. Deep crimson lighting from one side, contrasting with cool blue fill light from the other. Cinematic, fashion editorial mood.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Beginner
- **Pro tip:** The dolly movement description helps the model create a smooth sweeping camera motion. Red-on-red color schemes are well handled.
- **Reference image:** Woman lying on red satin sheets, red lingerie, dramatic two-tone lighting.

#### 1.5 — Champagne Toast

```
A woman in a black velvet corset and high-waisted stockings reclines on a chaise lounge. She raises a champagne glass toward the camera, tilting it slightly so the golden liquid catches the light. She takes a slow sip, eyes looking directly into the lens. Warm tungsten lighting, dark moody background with deep shadows. Film noir aesthetic, 4K cinematic quality.
```

- **Model:** Wan 2.6 I2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Props like glasses work better with Wan 2.6. Keep the motion simple — a single gesture performs best.
- **Reference image:** Woman on chaise lounge holding champagne glass, corset, noir lighting.

#### 1.6 — Balcony Evening

```
A woman in a sheer black negligee stands on a balcony at twilight, city lights blurred in the background. A gentle breeze moves the fabric and her hair. She leans on the railing, turns her head slowly to look over her shoulder at the camera. Golden hour backlighting creates a silhouette effect with rim light outlining her figure. Cinematic, atmospheric, anamorphic lens flare.
```

- **Model:** Wan 2.6 T2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Backlighting prompts work well in T2V because the silhouette simplifies anatomy generation. "Anamorphic lens flare" adds cinematic quality.
- **Reference image (if I2V):** Woman on balcony, sheer clothing, backlit by sunset, city bokeh.

#### 1.7 — Lace & Pearls Close-Up

```
Extreme close-up tracking shot across a woman's collarbone and neck, adorned with a pearl necklace over bare skin. The camera moves slowly from left to right. Her chest rises and falls with slow breathing. Macro lens detail captures skin texture and pearl iridescence. Soft top-down lighting, black background, studio quality.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Beginner
- **Pro tip:** Close-up body shots avoid face distortion issues. Breathing motion is one of the easiest animations for the model.
- **Reference image:** Macro photo of neck/collarbone with pearls, studio lighting, dark background.

#### 1.8 — Getting Dressed Sequence

```
A woman stands in front of an open closet in matching bra and panties, selecting a dress. She pulls a red dress from the hanger and holds it against her body, turning left and right to check in a full-length mirror. Natural morning light from a large window. Realistic apartment interior. Medium full-body shot, handheld camera feel with subtle movement.
```

- **Model:** Wan 2.5 I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Intermediate
- **Pro tip:** Dressing/undressing sequences need a clear starting pose in the reference image. 9:16 vertical aspect ratio works best for full-body standing shots.
- **Reference image:** Woman standing in underwear near closet, natural window light, full body visible.

#### 1.9 — Bubble Bath Luxury

```
A woman reclines in a large freestanding bathtub filled with bubbles. Only her head, shoulders, and one raised knee are visible above the foam. She lifts a handful of bubbles and blows them gently toward the camera. Steam rises around her. Warm bathroom lighting with candles visible in the background. Soft focus, dreamy atmosphere, slow motion bubble movement.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Beginner
- **Pro tip:** Bubbles and steam add natural motion that makes the video feel alive. This prompt works well even with lower-quality models because foam conceals potential artifacts.
- **Reference image:** Woman in bubble bath, shoulders visible, candle-lit bathroom.

#### 1.10 — Stocking Pull-Up

```
Close-up shot of a woman's leg as she slowly rolls a black thigh-high stocking up from her ankle to her thigh. She is seated on the edge of a bed, wearing a garter belt. Camera follows her hands as they smooth the fabric upward. Soft side lighting creates contour shadows along her leg. Intimate bedroom setting, warm tones, cinematic slow motion.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Beginner
- **Pro tip:** Isolated body part close-ups produce the most consistent results. The upward hand motion is easy for the model to track.
- **Reference image:** Close-up of leg with stocking partially rolled up, hands visible, bed edge visible.

#### 1.11 — Fireplace Fur Rug

```
A woman lies on a white faux fur rug in front of a roaring fireplace, wearing only a thin gold chain necklace. She rests on her stomach with her chin propped on her hands, feet playfully kicking in the air behind her. Warm firelight dances across her skin creating moving shadows. Camera at low angle, shallow depth of field. Cozy, intimate, luxurious atmosphere.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Fireplace flickering provides natural animation even if body movement is minimal. Describe the light movement for more dynamic results.
- **Reference image:** Woman on fur rug, stomach-down pose, fireplace in background, warm light.

#### 1.12 — Window Rain

```
A woman in an oversized sheer white shirt and nothing underneath sits on a window seat during a rainstorm. She presses her hand against the rain-streaked glass, gazing outside. Droplets on the window create bokeh effects with street lights outside. Cool blue-grey natural light illuminates her from the front. Melancholic, cinematic mood, slow subtle movements.
```

- **Model:** Wan 2.6 I2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Rain on glass creates beautiful animated texture. Wan 2.6 handles the transparency of sheer fabric better than Spicy.
- **Reference image:** Woman at rain-streaked window, sheer white shirt, blue-grey lighting.

#### 1.13 — Back Detail Tracking Shot

```
Camera slowly tracks down a woman's bare back from her neck to her lower back as she stands facing away. Her skin is lightly oiled, catching studio light in highlights along her spine. She shifts her weight from one hip to the other in a slow, natural movement. A single overhead softbox creates dramatic top-down lighting with deep shadows on either side. Black background, beauty campaign aesthetic.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Beginner
- **Pro tip:** Tracking shots along the body are very reliable. Oiled skin descriptions add realistic light interaction.
- **Reference image:** Woman's bare back, studio lighting, oiled skin, black background.

#### 1.14 — Blindfold Tease

```
A woman wearing a black silk blindfold and red lipstick lies back on white pillows. She bites her lower lip and tilts her head to one side. Her hands grip the sheets beside her. Camera slowly pushes in from chest-up to face close-up. Soft diffused overhead lighting, high-key white bedroom setting. Sensual and mysterious atmosphere, fashion photography quality.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Beginner
- **Pro tip:** Blindfolds eliminate eye-tracking artifacts, which are common in AI video. This is a great trick for more consistent face generation.
- **Reference image:** Woman with silk blindfold, red lips, lying on white pillows, soft lighting.

#### 1.15 — Undressing Zipper

```
Over-the-shoulder shot from behind as a woman reaches back to slowly unzip a tight black cocktail dress. The zipper moves down inch by inch, revealing her bare back and the clasp of a black bra. She looks over her shoulder toward the camera with a half-smile. Evening interior lighting, blurred living room background with warm lamp light. Cinematic slow motion, intimate framing.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Unzipping is a clear directional motion the model can follow. Over-the-shoulder framing reduces face distortion risk.
- **Reference image:** Woman from behind, hand reaching for zipper, dress partially unzipped, warm interior lighting.

#### 1.16 — Jewelry Only

```
A woman stands in a dark studio wearing only layered gold body chains and a waist chain. She rotates slowly in a 180-degree turn, the chains catching light and creating moving highlights across her body. Single dramatic spotlight from above-left. Rest of the frame is deep black. High fashion editorial, slow deliberate movement, 4K detail on jewelry reflections.
```

- **Model:** Wan 2.6 I2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Advanced
- **Pro tip:** Wan 2.6 handles metallic reflections better. The dark background simplifies the scene and improves body coherence.
- **Reference image:** Woman in body chain jewelry only, dramatic single light source, dark studio.

---

### Category 2: Artistic Nude

#### 2.1 — Classical Venus Pose

```
A woman stands in a classical contrapposto pose inspired by Botticelli's Birth of Venus. One hand covers her chest, the other holds flowing fabric at her side. The fabric billows gently as if in a breeze. Soft, even studio lighting mimics Renaissance painting illumination. Warm ivory skin tones, muted earth-tone background. Fine art photography quality, museum-worthy composition.
```

- **Model:** Wan 2.6 T2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Intermediate
- **Pro tip:** Classical art references help the model produce anatomically coherent poses. The flowing fabric adds motion without requiring complex body movement.
- **Reference image (if I2V):** Woman in Venus-like pose with draped fabric, soft studio lighting.

#### 2.2 — Shadow Play

```
A nude woman stands behind a window with venetian blinds, creating horizontal stripe shadows across her entire body. She slowly raises both arms above her head, and the shadow pattern shifts across her skin. High contrast black and white. Dramatic side lighting from the window. Artistic, abstract feel — the shadows become the subject more than the body. 35mm film grain.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Intermediate
- **Pro tip:** Shadow-heavy scenes are forgiving of anatomical artifacts. Black and white further reduces color-related issues.
- **Reference image:** Nude figure with venetian blind shadow stripes, high contrast B&W, arms at sides.

#### 2.3 — Body Landscape

```
Extreme close-up macro shot treating the curves of a woman's nude body as a landscape. Camera slowly pans across the terrain of her hip, waist, and ribcage like a drone flying over sand dunes. Warm golden hour lighting rakes across the skin at a low angle, emphasizing every curve and contour. Shallow depth of field, parts of the body blur into abstraction. Meditative, contemplative pace.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 21:9
- **Difficulty:** Beginner
- **Pro tip:** Body-as-landscape abstractions work extremely well because the model doesn't need to track faces or full anatomy. Use 21:9 widescreen for the most cinematic result.
- **Reference image:** Macro close-up of hip/waist curves, golden side lighting, shallow DOF.

#### 2.4 — Underwater Float

```
A nude woman floats weightlessly in clear blue water, hair fanning out around her head like a halo. She slowly extends her arms outward in a cruciform pose. Sunlight penetrates the water from above, creating caustic light patterns across her skin. Small air bubbles rise from her body. Ethereal, dreamlike quality. Shot from slightly below looking upward. Slow motion.
```

- **Model:** Wan 2.6 T2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Advanced
- **Pro tip:** Underwater scenes benefit from Wan 2.6's superior quality. The water medium naturally softens edges and hides artifacts. Caustic light patterns add beautiful procedural animation.
- **Reference image (if I2V):** Woman floating in clear water, underwater photography, sunlight from above.

#### 2.5 — Paint Drip Body Art

```
A woman stands against a white backdrop as thick paint slowly drips down her nude body. Streams of deep blue, crimson, and gold paint flow over her shoulders and down her torso. She stands still with arms slightly away from her body as the paint creates abstract patterns on her skin. Bright even studio lighting, white cyclorama background. Contemporary art installation feel. High speed camera capturing paint flow in slow motion detail.
```

- **Model:** Wan 2.6 I2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Advanced
- **Pro tip:** Paint drip effects work best with Wan 2.6 for color accuracy. The reference image should already show some paint on the body to give the model a starting point.
- **Reference image:** Woman with paint partially covering body, white background, studio lighting, paint mid-drip.

#### 2.6 — Forest Nymph

```
A nude woman walks barefoot through a sun-dappled forest, seen from behind at a distance. Ferns and tall grass partially conceal her lower body. She reaches up to touch a low-hanging branch, and leaves scatter downward. Shafts of golden sunlight break through the tree canopy. Natural, organic, editorial nature photography style. Medium telephoto lens compression, soft background bokeh from forest depth.
```

- **Model:** Wan 2.5 I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Distance shots in nature are very forgiving. The natural environment provides organic motion (leaves, light) that enriches the video. Walking away from camera is easier to generate than walking toward.
- **Reference image:** Nude woman walking in forest, from behind, sun-dappled lighting, partial concealment by foliage.

#### 2.7 — Studio Figure Study

```
A nude woman sits on a simple wooden stool in a photography studio, one leg crossed over the other. She slowly shifts from a profile view to a three-quarter angle, turning her upper body toward the camera. Single large octabox softlight from the right creates gentle wraparound illumination with soft shadows. Grey seamless paper background. Classical figure study composition, dignified and statuesque.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Beginner
- **Pro tip:** Simple studio setups with single light sources produce the most consistent results. The seated pose limits lower body movement, reducing artifact risk.
- **Reference image:** Nude woman on stool, profile pose, single softbox lighting, grey background.

#### 2.8 — Milk Bath

```
A woman lies in a bathtub filled with opaque white milk, only her face, the tops of her shoulders, one knee, and her hands visible above the surface. Pink and white flower petals float on the milk surface. She tilts her head back slowly, eyes closed, in an expression of bliss. Overhead camera angle looking straight down. Soft natural window light, pastel tones. Luxurious, serene fine art aesthetic.
```

- **Model:** Wan 2.6 I2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 1:1
- **Difficulty:** Beginner
- **Pro tip:** Milk baths are ideal for NSFW AI video — the milk conceals the body while keeping the scene sensual, and floating petals add easy natural motion. Overhead angle is the classic composition.
- **Reference image:** Overhead milk bath photo with floating petals, face and partial body visible, soft lighting.

#### 2.9 — Silhouette Stretch

```
A completely backlit silhouette of a nude woman performing a slow stretch sequence against a bright white background. She starts with arms at her sides, raises them overhead, then bends to one side in a lateral stretch. Only the dark outline of her figure is visible — no skin detail, pure form. High contrast, minimal, graphic quality. Like a living logo or icon.
```

- **Model:** Wan 2.5 T2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Beginner
- **Pro tip:** Pure silhouettes eliminate all texture/anatomy issues while still being visually striking. Great for beginners to test workflows. Any model can handle this well.
- **Reference image (if I2V):** Silhouette of standing woman, bright white backlight, arms at sides.

#### 2.10 — Desert Dunes

```
A nude woman walks along the crest of a sand dune in a vast desert landscape, seen from a great distance as a small figure against the sky. Wind blows fine sand off the dune ridge. The setting sun creates an orange-pink sky and long shadows. Epic wide-angle landscape shot where the human figure is a small element within the vast natural scene. National Geographic cinematic quality, drone footage aesthetic.
```

- **Model:** Wan 2.6 T2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 21:9
- **Difficulty:** Intermediate
- **Pro tip:** Extreme wide shots with small figures are the most reliable for full nudity — the distance means less anatomical detail to get wrong. 21:9 ultrawide enhances the epic landscape feel.
- **Reference image (if I2V):** Tiny figure on sand dune crest, sunset lighting, wide landscape.

#### 2.11 — Wet Skin Studio

```
A woman stands in a dark studio, skin glistening wet as if she just stepped out of rain. A single hard spotlight from above-right creates dramatic chiaroscuro lighting. Water droplets are visible on her shoulders and arms. She breathes deeply, chest rising and falling, then slowly turns her face upward into the light. Black background, high contrast, Leibovitz-inspired portrait quality. Slow motion water droplets catching the light.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Intermediate
- **Pro tip:** Wet skin adds realistic light interaction that makes AI-generated skin look more convincing. Breathing motion is subtle and easy for the model.
- **Reference image:** Wet-skinned woman, single dramatic spotlight, dark studio, water droplets visible.

#### 2.12 — Yoga Sunrise

```
A nude woman performs a slow sun salutation yoga sequence on a cliff overlooking the ocean at sunrise. She transitions from mountain pose to forward fold with fluid, graceful movement. The rising sun behind her creates a warm golden backlight and lens flare. Waves crash on rocks far below. Wide establishing shot. Spiritual, empowering, natural beauty aesthetic. Golden hour cinematography.
```

- **Model:** Wan 2.6 T2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Advanced
- **Pro tip:** Yoga transitions are complex multi-step movements — keep the duration short (5s) for best coherence. The backlit wide shot helps maintain body consistency.
- **Reference image (if I2V):** Woman in mountain pose on cliff edge, sunrise backlighting, ocean background.

#### 2.13 — Fabric Unwrap

```
A woman stands wrapped in a long piece of white chiffon fabric. She begins to slowly turn, and the fabric unwinds from her body in a spiral, progressively revealing more skin. The unwinding fabric floats and billows around her in slow motion. Bright white studio background, even lighting from all sides. Elegant, dance-like quality. Camera at mid-height, full body framing. The fabric moves like a living entity.
```

- **Model:** Wan 2.6 I2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Advanced
- **Pro tip:** Fabric animation is one of AI video's strengths. Start the reference image with fabric mostly wrapped, and let the prompt describe the unwinding. Wan 2.6 handles flowing cloth best.
- **Reference image:** Woman wrapped in white chiffon, white studio background, even lighting.

#### 2.14 — Ocean Waves

```
A nude woman lies at the edge of the surf on a sandy beach. Gentle waves wash over her body and recede rhythmically. She lies on her back with eyes closed, arms outstretched, letting the water flow over her. Late afternoon golden light, wet sand reflects the sky. Overhead drone shot slowly descending. Peaceful, meditative, earth-mother energy. The rhythm of the waves dominates the scene.
```

- **Model:** Wan 2.5 I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Water washing over a body creates reliable, repeating motion that AI handles well. The overhead drone perspective avoids complex perspective changes.
- **Reference image:** Woman lying at surf's edge, overhead angle, golden light, waves touching her body.

#### 2.15 — Smoke & Form

```
A nude woman's body is partially obscured by wisps of colored smoke — purple and blue — swirling around her in a dark studio. She moves slowly through the smoke, arms creating gentle currents that disturb the tendrils. Single rim light from behind outlines her figure through the smoke. Moody, mysterious, abstract. The smoke is the primary visual element, the body secondary. Slow, hypnotic movement.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Smoke naturally animates in AI video and provides beautiful coverage of potential artifacts. Colored smoke on a dark background is a reliable artistic approach.
- **Reference image:** Woman with colored smoke, rim-lit, dark background, smoke partially obscuring body.

---

### Category 3: Couple / Romantic Scenes

#### 3.1 — Slow Dance Bedroom

```
A couple in a dimly lit bedroom. The man wears an unbuttoned white shirt and dark pants. The woman wears a silk slip dress. They sway slowly in a close embrace, foreheads touching. He has one hand on her lower back, she has both hands on his chest. Warm string lights in the background create soft bokeh. Slow, intimate rotation. Camera slowly orbits around them. Golden warm tones.
```

- **Model:** Wan 2.6 T2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Advanced
- **Pro tip:** Two-person scenes require more processing power — Wan 2.6 handles them best. Keep the motion simple (swaying, not complex choreography). Specify each person's clothing clearly.
- **Reference image (if I2V):** Couple in close embrace, dimly lit room, string lights background.

#### 3.2 — Kiss Close-Up

```
Extreme close-up of a couple's lips meeting in a slow, gentle kiss. The camera is at lip level, slightly angled. His hand comes up to cradle her jaw. Shallow depth of field — only the lips and immediate skin are in focus. Warm, soft lighting from the side. Skin tones are warm and natural. Time seems to slow down. Intimate, tender, cinematic. The rest of the world is a blur.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Extreme close-ups of lips avoid the dual-face generation challenge. The shallow DOF description helps blur any imperfections.
- **Reference image:** Close-up of two faces about to kiss, lips nearly touching, warm side lighting.

#### 3.3 — Beach Sunset Embrace

```
A couple stands waist-deep in calm ocean water at golden hour. She wraps her arms around his neck, legs around his waist. He holds her, slowly turning them both in the water. The setting sun creates a massive golden backlight. Silhouette-to-semi-silhouette exposure. Small waves lap around them. Lens flare from the sun. Epic romantic cinematic wide shot, drone pulling slowly backward to reveal the vast ocean and sky.
```

- **Model:** Wan 2.6 T2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 21:9
- **Difficulty:** Advanced
- **Pro tip:** Backlighting both figures as semi-silhouettes dramatically reduces artifact risk in two-person scenes. The water conceals lower body complexity.
- **Reference image (if I2V):** Couple embracing in ocean, backlit sunset, silhouette, wide shot.

#### 3.4 — Morning After

```
A couple lies in white sheets in morning light. He lies on his back, she rests her head on his bare chest. She traces lazy circles on his skin with her finger. Soft white curtains billow from an open window, letting in warm morning sun. Camera is at mattress level, intimate POV. Everything is white and golden. Peaceful, tender, post-intimate moment. Slow breathing movements.
```

- **Model:** Wan 2.5 I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Lying-down scenes are much easier for the model than standing scenes with two people. The sheets naturally cover most anatomy, reducing complexity.
- **Reference image:** Couple in bed, white sheets, woman on man's chest, morning window light.

#### 3.5 — Neck Kiss

```
A man stands behind a woman, both shown from the shoulders up. He slowly lowers his head to kiss her neck. She tilts her head to one side, eyes closing, lips slightly parting. His hand reaches up to gently move her hair aside. Warm interior lighting from the side. Blurred background. Extreme close-up framing. Sensual, anticipatory tension. Slow, deliberate movements. Skin texture visible in sharp detail.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Neck kiss scenes from behind avoid showing two full faces simultaneously, which reduces dual-face artifacts. Keep the framing tight.
- **Reference image:** Man behind woman, about to kiss her neck, her head tilted, warm lighting.

#### 3.6 — Bathtub For Two

```
A couple sits in a large freestanding bathtub facing each other, surrounded by candlelight. She has her legs over his, bubbles partially covering them. He picks up a handful of foam and playfully puts it on her nose. She laughs, splashing a tiny bit of water. Warm candlelight creates golden highlights on wet skin. Steam rises between them. Cozy, playful, intimate. Shot from a slightly elevated angle.
```

- **Model:** Wan 2.6 I2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Advanced
- **Pro tip:** Bathtub scenes with two people need Wan 2.6 for best results. The water and bubbles conceal bodies and simplify the generation. Playful actions add charm.
- **Reference image:** Couple in bathtub facing each other, candlelight, bubbles, elevated camera angle.

#### 3.7 — Dress Unzipping

```
A woman stands with her back to the camera in an evening dress. A man's hands enter the frame from behind and slowly unzip her dress. The zipper descends, revealing her bare back inch by inch. She glances over her shoulder. Only their hands and her back are prominently shown. Dim bedroom lighting, warm tones. Camera focuses tight on the zipper area. Intimate, anticipatory.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Intermediate
- **Pro tip:** Having only hands visible for the second person dramatically simplifies the scene. The unzipping motion is clear and directional — ideal for AI video.
- **Reference image:** Woman's back in dress, man's hands at zipper, dim lighting.

#### 3.8 — Shower Silhouette

```
Silhouette of a couple behind a frosted glass shower door. Steam fills the air. Through the translucent glass, you can see them embracing — she has her arms around his neck. Hot water streams down the glass. The figures shift and move slowly behind the frosted barrier. Bathroom lighting from behind creates the silhouette effect. Artistic, suggestive without being explicit. Steam and water droplets on glass are the sharpest elements.
```

- **Model:** Wan 2.5 T2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Intermediate
- **Pro tip:** Frosted glass lets you suggest explicit content while the glass barrier hides all anatomical details, making generation reliable. Water on glass animates beautifully.
- **Reference image (if I2V):** Silhouettes behind frosted shower glass, steam, water droplets.

#### 3.9 — Lap Sitting

```
A woman sits on a man's lap on a plush armchair. She faces him with her knees on either side. She wears a matching bra and panty set, he is shirtless. She runs both hands through his hair while looking down at him. He has his hands on her waist. Camera at their eye level from the side, showing both profiles. Warm lamplight from one side, dark moody room. Intimate, sensual tension. Slow, minimal movement.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Advanced
- **Pro tip:** Side profile framing for couples is the most reliable angle — it shows both people clearly without one face being obscured or distorted. Keep movement subtle.
- **Reference image:** Couple on armchair, woman on man's lap facing him, side angle, warm lamp lighting.

#### 3.10 — Against The Wall

```
A couple against a textured brick wall. He presses her gently against the wall, one hand bracing beside her head. She grabs his shirt collar, pulling him closer. Their faces are inches apart, heavy eye contact. Urban setting, a dim alley or industrial loft. Hard directional light from one side creates dramatic shadows on the wall. Raw, passionate energy. Camera slowly pushes in. Gritty, cinematic, high contrast.
```

- **Model:** Wan 2.6 I2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Advanced
- **Pro tip:** The wall provides a stable background that prevents environmental warping. Hard lighting with strong shadows is more forgiving than even lighting for two-person scenes.
- **Reference image:** Couple against brick wall, intense eye contact, dramatic side lighting, close proximity.

#### 3.11 — Blindfolded Trust

```
A woman lies on a bed wearing a silk blindfold and a lace bodysuit. A man's hand enters the frame and slowly traces a line down her arm with a single fingertip. She shivers slightly at the touch, goosebumps visible on her skin in the close-up. Only his hand and her arm/torso are visible. Soft diffused overhead lighting. White bedding. Intimate, trust-based, sensual. Extreme close-up tracking the finger's path.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Beginner
- **Pro tip:** Showing only a hand from the second person eliminates dual-person complexity entirely. The blindfold removes eye-tracking issues. This combination is one of the most reliable for couple content.
- **Reference image:** Close-up of blindfolded woman's arm/torso, man's hand about to touch, soft overhead light.

#### 3.12 — Forehead Kiss

```
A man gently kisses a woman's forehead while she closes her eyes and smiles softly. He cradles her face with both hands. Shot from a low angle looking slightly up. They are backlit by a warm sunset through a window. Golden rim light outlines both figures. She reaches up and holds one of his wrists. Tender, protective, deeply romantic. Slow, held moment — almost a freeze-frame with subtle breathing movement.
```

- **Model:** Wan 2.5 I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Forehead kisses are simpler to generate than lip kisses — only one face is fully visible. The backlighting reduces facial detail requirements.
- **Reference image:** Man kissing woman's forehead, his hands on her face, backlit, warm tones.

#### 3.13 — Undressing Each Other

```
Medium shot of a couple standing face to face. She slowly unbuttons his shirt from top to bottom while maintaining eye contact. He slides the strap of her dress off one shoulder. Warm ambient bedroom lighting. Slow, deliberate pace. The tension of anticipation. Every small gesture feels significant. Cinematic, shot like an indie film love scene.
```

- **Model:** Wan 2.6 I2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Advanced
- **Pro tip:** Describe one action at a time for best results. In a 5-second clip, one or two undressing gestures is realistic. Multiple actions need longer duration.
- **Reference image:** Couple face to face, her hands on his shirt buttons, his hand near her shoulder strap.

#### 3.14 — Carried To Bed

```
A man carries a woman in his arms (bridal carry) toward a bed. She has her arms around his neck, laughing. He gently lays her down on the bed, leaning over her. She pulls him down by his shirt. Shot from the side, following the motion from standing to lying down. Warm bedroom lighting, rumpled white sheets. Spontaneous, passionate, joyful energy. Handheld camera feel with natural movement.
```

- **Model:** Wan 2.6 T2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Advanced
- **Pro tip:** Complex physical interaction (carrying) is one of the hardest things for AI video. Use Wan 2.6 and keep to 5 seconds. The motion from standing to lying simplifies partway through.
- **Reference image (if I2V):** Man holding woman in bridal carry, warm bedroom, approaching bed.

#### 3.15 — Tangled Sheets

```
Overhead bird's-eye view looking straight down at a couple tangled in white sheets on a bed. Only parts of their bodies are visible between the folds of fabric — a bare shoulder here, intertwined fingers there, a turned face. They shift and move slowly beneath the sheets. Morning light from one side creates long shadows across the white fabric. Artistic, abstract, the sheets create a landscape of peaks and valleys. Minimal movement, breathing and subtle shifting.
```

- **Model:** Wan 2.5 I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 1:1
- **Difficulty:** Beginner
- **Pro tip:** The overhead sheet shot is incredibly forgiving — sheets cover nearly everything while the scene reads as deeply intimate. One of the most reliable couple prompts.
- **Reference image:** Overhead view of couple in tangled white sheets, partial body visibility, morning light.

---

### Category 4: Fantasy & Cosplay

#### 4.1 — Dark Elf Sorceress

```
A dark elf woman with obsidian skin and long silver-white hair stands in a magical forest clearing. She wears only strategically placed silver armor pieces and a flowing translucent cape. She raises her hands and conjures swirling purple magical energy between her palms. The energy illuminates her face and body from below. Bioluminescent plants glow in the background. Fantasy RPG cinematic, dramatic low-angle shot. Particle effects and magical sparkles float in the air.
```

- **Model:** Wan 2.6 T2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Advanced
- **Pro tip:** Fantasy elements (magic particles, glowing plants) add motion that enriches the scene. Dark skin with silver/white accents creates stunning high-contrast palette. Specify armor placement carefully.
- **Reference image (if I2V):** Dark elf woman in minimal silver armor, magical forest, purple light.

#### 4.2 — Succubus Transformation

```
A beautiful woman in a dark room begins a slow transformation. Small black horns emerge from her forehead, dark wings unfurl from her back, and her eyes glow red. She wears a form-fitting black leather outfit that leaves her midriff and legs exposed. She extends one clawed hand toward the camera with a seductive smile. Red and black smoke swirls around her feet. Gothic fantasy horror aesthetic, dramatic uplighting in crimson.
```

- **Model:** Wan 2.6 T2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Advanced
- **Pro tip:** Transformation effects are difficult — focus on one transformation element (e.g., just the wings unfurling) for a 5-second clip rather than trying everything at once.
- **Reference image (if I2V):** Succubus character mid-transformation, horns and wings, red eyes, dark background.

#### 4.3 — Warrior Princess

```
A muscular woman in fantasy warrior bikini armor stands on a cliff overlooking a burning city. Wind whips her braided red hair. She raises a glowing sword overhead with both hands, the blade emitting golden light. Her bronze skin glistens with sweat. Camera slowly tilts upward from her boots to the sword tip against a dramatic storm sky. Epic, heroic, powerful. Orchestral movie trailer energy.
```

- **Model:** Wan 2.6 T2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** The tilt-up camera movement creates a reveal that's dramatic and technically reliable. Wind in hair adds organic motion. Glowing weapons are a nice AI video bonus.
- **Reference image (if I2V):** Warrior woman on cliff, bikini armor, sword raised, stormy sky.

#### 4.4 — Cyberpunk Strip Club

```
A woman dances on a neon-lit stage in a cyberpunk strip club. She wears a futuristic holographic bikini that shimmers and changes color with her movement. Neon signs in Japanese and English glow behind her. Rain is visible through a window, streaking with neon reflections. She moves fluidly around a chrome pole. Camera slowly pans across the scene. Blade Runner aesthetic, heavy atmosphere, synthwave color palette — hot pink, cyan, purple.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Neon lighting hides a lot of artifacts due to its extreme color saturation. Cyberpunk settings are well-represented in training data, so environments generate reliably.
- **Reference image:** Woman on neon stage, holographic outfit, cyberpunk club interior.

#### 4.5 — Mermaid Surface

```
A beautiful mermaid breaks the surface of a moonlit ocean. From the waist up she is a nude woman with long flowing wet hair. Her iridescent fish tail is visible beneath the water surface, scales catching moonlight. She arches her back and tosses her head, water droplets flying in an arc. A full moon illuminates the scene. Bioluminescent plankton creates blue sparkles in the water around her. Fantasy illustration come to life, magical realism.
```

- **Model:** Wan 2.6 T2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Advanced
- **Pro tip:** Mermaid scenes work well because the water naturally handles the human-fish transition. The hair toss creates a satisfying motion arc. Bioluminescence adds AI-friendly particle effects.
- **Reference image (if I2V):** Mermaid emerging from water, moonlit, iridescent tail visible underwater.

#### 4.6 — Anime School Girl Wind

```
Anime-style illustration of a school girl on a rooftop during golden hour. A strong gust of wind catches her pleated skirt, lifting it to reveal thigh-high stockings. She grabs the hem with one hand, blushing. Cherry blossom petals blow across the scene. Her long hair streams horizontally in the wind. Classic anime art style with cel shading and clean linework. Camera holds steady on a medium shot. Vibrant saturated colors, clear blue sky.
```

- **Model:** Wan 2.5 T2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Intermediate
- **Pro tip:** Specifying "anime-style illustration" and "cel shading" pushes the output toward 2D animation. Cherry blossom petals are classic and generate well.
- **Reference image (if I2V):** Anime-style school girl on rooftop, wind blowing, golden hour, 2D illustration style.

#### 4.7 — Dragon Queen

```
A nude woman sits on a throne of dragon skulls and bones, draped only in a living snake that coils around her body. Two small dragons perch on her shoulders, breathing tiny flames. She has golden eyes with vertical slit pupils and subtle scales on her cheekbones. Crown of twisted black metal on her head. Dark throne room lit by torches and dragon fire. Game of Thrones meets dark fantasy art. Regal, dangerous, alluring.
```

- **Model:** Wan 2.6 T2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Advanced
- **Pro tip:** Throne scenes are static-body with dynamic-environment (flames, small dragon movements), which is ideal for AI video. Firelight provides natural animation.
- **Reference image (if I2V):** Dragon queen on bone throne, small dragons, torch-lit throne room.

#### 4.8 — Space Station Pinup

```
A woman floats weightlessly in a space station corridor, wearing only a tiny astronaut patch bikini. Her hair fans out in zero gravity. She slowly tumbles in the microgravity, a playful smile on her face. Earth is visible through a large viewport behind her, the blue planet casting a soft blue light on her skin. Retro sci-fi pinup aesthetic mixed with realistic space photography. Slow, graceful zero-gravity movement.
```

- **Model:** Wan 2.6 T2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Zero-gravity floating is naturally slow and dreamy, which aligns well with AI video generation speeds. The Earth viewport adds a stunning background element.
- **Reference image (if I2V):** Woman floating in space station, bikini, hair in zero-g, Earth visible through window.

#### 4.9 — Vampire Seduction

```
A pale woman in a sheer black gothic gown descends a grand staircase in a candlelit castle. She has crimson lips, glowing amber eyes, and visible fangs when she smiles. She runs one hand along the stone banister. Hundreds of candles flicker on the walls. Her gown trails behind her on the steps. Camera tracks her descent from a low angle. Gothic romance, Interview with the Vampire aesthetic. Rich, dark, decadent color palette — deep reds, blacks, gold.
```

- **Model:** Wan 2.6 I2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Intermediate
- **Pro tip:** Staircase descent is a clear, directional motion that AI handles well. The hundreds of candles provide rich ambient flickering animation throughout the frame.
- **Reference image:** Vampire woman on grand staircase, gothic gown, candlelit castle interior.

#### 4.10 — Goddess of Spring

```
A woman emerges from a massive blooming flower, like Thumbelina but life-sized. She is nude, covered in dew drops and flower pollen. Petals slowly unfurl around her as she stretches and awakens. Butterflies land on her outstretched fingers. Lush garden background with impossibly vibrant flowers. Warm golden sunlight, macro photography depth of field making flowers look enormous. Fairy tale illustration quality, Studio Ghibli meets fine art photography.
```

- **Model:** Wan 2.6 T2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Advanced
- **Pro tip:** "Emerging from flower" gives the model a clear composition anchor. Butterflies and unfurling petals add layered motion. Referencing Studio Ghibli pulls in a recognizable aesthetic.
- **Reference image (if I2V):** Woman emerging from large flower, covered in dew, butterflies, lush garden.

---

### Category 5: Solo Performance

#### 5.1 — Pole Dance Spin

```
A woman in a metallic silver bikini performs a slow spinning descent on a chrome pole. She hooks one leg around the pole and leans back, hair falling freely as she rotates. Purple and blue stage lighting creates dynamic shadows. Slow motion captures the hair movement and body rotation. Professional strip club stage with LED lights in the floor. Shot from a low angle looking up at the spinning figure. Confident, athletic, powerful.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Intermediate
- **Pro tip:** Pole dance spins have a clear rotational axis, which helps the model maintain body coherence. Low angle looking up is a flattering and reliable perspective.
- **Reference image:** Woman on pole, mid-spin, metallic bikini, stage lighting, low angle.

#### 5.2 — Sensual Floor Dance

```
A woman in a black lace bodysuit performs a slow, sensual floor dance routine. She starts on all fours, arches her back deeply, then rolls onto her back, running her hands down her body. Camera is at floor level, capturing the movement intimately. Warm spotlight from above creates a pool of light on a dark stage. Her movements are fluid and cat-like. Professional dance performance quality, contemporary dance meets burlesque.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Floor-level camera for floor dance creates the most immersive perspective. Keep to one or two movement transitions per 5-second clip.
- **Reference image:** Woman on floor in lace bodysuit, arched back pose, spotlight from above, dark background.

#### 5.3 — Shower Scene

```
A woman stands under a rainfall showerhead, hot water streaming over her nude body. She tilts her head back, letting water run over her face and down her chest. Steam fills the glass-enclosed shower. She runs both hands through her wet hair, slicking it back. Warm bathroom lighting through frosted glass. Water droplets and streams are the primary visual texture. Camera at chest height, medium shot through the partially steamed glass door. Warm, steamy, relaxed.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Beginner
- **Pro tip:** Running water is one of the most reliable animations in AI video. The steam and water provide natural softening of details. Head-tilting-back is a simple, effective motion.
- **Reference image:** Woman in shower, head tilted back, water streaming, steam, warm lighting.

#### 5.4 — Lingerie Try-On

```
A woman stands in front of a full-length mirror in a boutique fitting room. She models a red lace bra and high-waisted panty set, turning side to side to check the fit. She adjusts one strap, smooths the fabric over her hip, and poses with hands on waist. Bright, even fitting room lighting. Multiple reflections from angled mirrors. Realistic, candid, like a fitting room selfie video come to life.
```

- **Model:** Wan 2.5 I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Intermediate
- **Pro tip:** Mirror scenes create a natural "two-shot" effect. Fitting room lighting is flat and even, which simplifies the generation. The try-on narrative feels organic and relatable.
- **Reference image:** Woman in lingerie in fitting room, full-length mirror visible, even lighting.

#### 5.5 — Bed Rolling

```
A woman in an oversized white t-shirt and cotton panties playfully rolls across a large bed, hugging a pillow. She rolls from one side to the other, the t-shirt riding up to expose her midriff and legs. Messy white bedding. Bright morning light from large windows. Overhead camera angle looking straight down, capturing the rolling motion. Carefree, playful, girl-next-door energy. Natural, unstaged feeling.
```

- **Model:** Wan 2.5 I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 1:1
- **Difficulty:** Beginner
- **Pro tip:** Rolling motion from overhead is one of the easiest for AI to generate — it's essentially a rotation around a central axis. The casual clothing feels more authentic.
- **Reference image:** Overhead view of woman lying on white bed, t-shirt and panties, morning light, pillow nearby.

#### 5.6 — Oil Massage

```
Close-up of hands applying glistening massage oil to a woman's bare back. The hands spread the oil in long, slow strokes from lower back to shoulders. Oil catches the light, creating moving highlights across the skin. She lies face down on a massage table with a white towel draped across her lower body. Warm spa lighting, bamboo and candle decor blurred in background. ASMR-like visual quality, extremely detailed skin texture. Slow, rhythmic, hypnotic movement.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Beginner
- **Pro tip:** Massage scenes with only hands and back visible are extremely reliable. The oil adds beautiful light interaction. Repetitive stroking motion is easy for AI to generate consistently.
- **Reference image:** Hands applying oil to woman's back, massage table, warm spa lighting.

#### 5.7 — Yoga Downward Dog

```
A woman in a sheer mesh sports bra and high-cut yoga shorts performs a slow transition from downward-facing dog to cobra pose on a yoga mat. Her body moves fluidly through the sequence. Sweat glistens on her skin. Natural light from floor-to-ceiling windows in a minimalist studio. Camera at mat level, side profile capturing the full body arch. Athletic, strong, sensual. Shallow depth of field, clean modern interior background.
```

- **Model:** Wan 2.5 I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Yoga transitions are recognizable movement patterns that AI models have learned well. Side profile maintains body coherence throughout the pose change.
- **Reference image:** Woman in downward dog pose, mesh sportswear, side view, studio with natural light.

#### 5.8 — Striptease Jacket

```
A woman in a black oversized blazer with nothing underneath slowly opens the jacket, holding each lapel. She pulls one side open just enough to reveal the inner curve of her breast, then pulls it closed again with a teasing smirk. She repeats with the other side. Camera at chest height, medium close-up. Moody bar lighting, warm amber, against a dark background. Confident, controlled, teasing. Slow, deliberate gestures.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Beginner
- **Pro tip:** The open-close-open tease is perfect for short clips — it creates a loop-friendly video. The blazer provides structure that helps the model maintain clothing consistency.
- **Reference image:** Woman in open black blazer, nothing underneath, holding lapels, moody bar lighting.

#### 5.9 — Stretching Wake-Up

```
A woman in a cropped tank top and thong sits on the edge of a bed, stretching as if she just woke up. She raises her arms overhead in a full body stretch, the tank top riding up to expose her entire midriff. She arches her back, yawns naturally, then runs her fingers through messy bed hair. Soft warm morning light from behind, creating a glowing halo effect on her hair. Natural, candid, unposed beauty. Handheld camera at bed level.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Beginner
- **Pro tip:** Morning stretching is relatable, natural-looking motion. The arms-overhead stretch is a simple, clear gesture that AI handles reliably.
- **Reference image:** Woman sitting on bed edge, arms beginning to stretch up, tank top and thong, morning backlight.

#### 5.10 — Mirror Dance

```
A woman in a bra and boy shorts dances slowly in front of a bathroom mirror, using it as an audience. She mouths along to a song (no audio), making flirtatious expressions at her reflection. She runs her hands through her hair, turns around to check herself out from behind. Bathroom vanity lighting — bright, even, slightly warm. Genuine, self-confident, like a private moment. Camera is placed where the mirror is, as if we ARE the mirror.
```

- **Model:** Wan 2.5 T2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Intermediate
- **Pro tip:** "Camera as mirror" perspective means the subject always faces the camera, which produces the best facial consistency. Natural, candid scenes are trending in AI video.
- **Reference image (if I2V):** Woman in underwear, bathroom setting, looking at camera (as mirror), vanity lighting.

#### 5.11 — Pool Exit

```
A woman in a barely-there white bikini climbs out of a swimming pool via the ladder. Water streams off her body as she emerges step by step. The wet white fabric becomes slightly transparent. She pushes wet hair back from her face and wrings water from her hair. Bright sunny day, turquoise pool water sparkles behind her. Camera at pool deck level, slightly low angle. Summer, vitality, energy. Slow motion water droplets.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Intermediate
- **Pro tip:** The pool ladder provides structural reference that helps maintain body proportions during the climbing motion. Wet fabric transparency is a natural NSFW element.
- **Reference image:** Woman on pool ladder, wet white bikini, water streaming, bright sunlight.

#### 5.12 — Candle Wax

```
A woman lies on her back on a dark surface, nude. A hand (could be her own) slowly tilts a lit red candle, and hot wax drips onto her stomach. She gasps slightly, muscles tensing visibly as each drop lands. Camera is positioned overhead, close-up on her torso where the wax is landing. Warm candlelight is the only illumination. Red wax creates abstract patterns on her skin. Dark, sensual, BDSM-adjacent. Extreme close-up, slow motion wax drip.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Wax dripping is a clear, gravity-driven motion that AI generates well. The close-up on torso avoids face/limb artifacts. Candlelight-only lighting creates dramatic mood with minimal complexity.
- **Reference image:** Close-up of torso with some wax already dripped, red candle in frame, candlelight only.

#### 5.13 — Feather Tease

```
Extreme close-up of a white feather being slowly dragged across a woman's bare stomach and hip. Her skin reacts with goosebumps as the feather passes. Her stomach muscles tense and release. The feather moves from her navel down to her hip bone and along the waistband of sheer panties. Only the torso and feather are visible. Soft diffused lighting from above. Tactile, sensory, ASMR aesthetic. Hyper-detailed skin texture.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Beginner
- **Pro tip:** Single prop interactions with body close-ups are the most reliable prompt type. The feather path gives the model clear directional movement to follow.
- **Reference image:** Feather on woman's bare stomach, extreme close-up, soft overhead lighting, goosebumps.

#### 5.14 — Towel Drop

```
A woman stands wrapped in a white bath towel in a steamy bathroom. She tucks the towel corner in at her chest, then lets go. The towel slowly slides down, she catches it at the last moment at her hips, revealing her bare torso. She looks at the camera with a mischievous expression. Warm bathroom lighting, steam in the air, dewy mirror behind her. Playful, teasing, well-timed. Medium shot, static camera.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Intermediate
- **Pro tip:** The towel drop is a classic NSFW sequence. Having her catch it partway creates a tease moment. The steamy bathroom softens the background.
- **Reference image:** Woman in white towel, bathroom, steam, about to release towel tuck.

#### 5.15 — Body Wave Dance

```
A woman in a micro bikini performs a slow, hypnotic body wave from head to toe. She stands in profile view so the wave motion is clearly visible — head, chest, stomach, hips rolling in sequence. Dark background with a single blue backlight creating a rim-light silhouette effect. Her body moves like a wave through water, continuous and fluid. Repeat the wave 2-3 times in the clip. Mesmerizing, loop-friendly. Club dance energy at half speed.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Intermediate
- **Pro tip:** Body waves in profile are visually clear and create satisfying loopable content. The rim-light silhouette simplifies the generation while looking professional. Blue backlight is flattering on all skin tones.
- **Reference image:** Woman in profile, micro bikini, mid-body-wave pose, blue backlight, dark background.

---

### Category 6: Professional / Commercial NSFW

#### 6.1 — Lingerie Brand Commercial

```
A model walks down a minimalist white runway in a new collection of ivory lace lingerie — balconette bra, garter belt, and stockings. She walks with confident, measured strides. Camera tracks alongside her at hip height. Clean white background, professional fashion show lighting from above. Slow motion to capture fabric movement and detail. End with her pausing at the end of the runway, one hand on hip. High-end fashion brand commercial quality, Victoria's Secret runway energy.
```

- **Model:** Wan 2.6 I2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Fashion runway walks are well-represented in training data. The tracking camera at hip height captures the lingerie effectively while creating smooth camera motion.
- **Reference image:** Model mid-stride on white runway, lace lingerie set, fashion show lighting.

#### 6.2 — Perfume Ad Sensuality

```
A woman in a barely-there gold dress lies across a marble surface in a luxury penthouse. She reaches for a crystal perfume bottle, brings it to her neck, and sprays. She tilts her head back in pleasure. The spray catches light like tiny diamonds. Camera starts on the perfume bottle in her hand, then slowly pulls back to reveal her full figure. Luxury brand commercial cinematography — dark, rich, decadent. Warm gold tones, sharp highlights on marble and glass.
```

- **Model:** Wan 2.6 I2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Luxury product shots have a well-defined visual language that AI has learned. The perfume spray catching light creates a magical particle effect.
- **Reference image:** Woman with perfume bottle, gold dress, marble surface, luxury penthouse setting.

#### 6.3 — Swimwear Catalog

```
A model stands on white sand beach at midday, modeling a strappy red bikini. She performs a slow 360-degree turn, showing the suit from all angles. Sun is directly overhead creating minimal shadows. Crystal clear turquoise water behind her. Her hair blows slightly in ocean breeze. Shot like a professional e-commerce product video — clean, bright, focused on the garment. Full body framing with space around the figure. Color-accurate lighting.
```

- **Model:** Wan 2.5 I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Beginner
- **Pro tip:** Product/catalog-style videos work best with simple, bright, even lighting and full body framing. The 360 turn showcases the product effectively.
- **Reference image:** Model on white beach in red bikini, straight standing pose, bright midday sun.

#### 6.4 — Boudoir Photography BTS

```
Behind-the-scenes style video of a boudoir photography shoot. A woman in black lingerie poses on a tufted velvet chaise while a photographer (partially visible at frame edge) directs her. She shifts between poses — seated with crossed legs, then leaning back on one elbow, then looking over her shoulder. Multiple studio strobes fire, creating flash effects. The scene has the energy of a real photo shoot — professional, collaborative, confident. Mixed continuous and flash lighting.
```

- **Model:** Wan 2.6 T2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Advanced
- **Pro tip:** BTS-style content feels authentic and engaging. Flash effects can be simulated by mentioning "studio strobes fire" — this creates bright-frame moments that add production value.
- **Reference image (if I2V):** BTS boudoir shoot, model on chaise, photographer partially visible, studio equipment.

#### 6.5 — Magazine Cover Animation

```
A still magazine cover comes to life. The cover shows a woman in a plunging neckline gown. She blinks, takes a breath, and turns her head slightly, breaking the fourth wall. The magazine title and text remain static while only the model moves, creating a Harry Potter portrait effect. Glossy magazine aesthetics — perfect skin, editorial makeup, precise lighting. Subtle movement only — this is about the uncanny valley effect of a photo coming alive.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Beginner
- **Pro tip:** "Living photo" style requires only minimal movement (blink, breath, small head turn), making it very easy to generate well. Use an actual magazine-style reference image for best results.
- **Reference image:** High-quality magazine cover photo with model, editorial styling, text overlay.

#### 6.6 — Fitness Brand Reveal

```
A fit woman in a sports bra and compression leggings stands in a gym with dramatic lighting. She slowly peels off the leggings, revealing toned legs, rolling the fabric down with both hands. Each muscle is defined under professional sports lighting. She then stands confidently in the sports bra and matching brief bottoms. Nike commercial quality, empowering, athletic beauty. Hard directional light creating muscle definition shadows.
```

- **Model:** Wan 2.5 I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Intermediate
- **Pro tip:** Athletic/fitness content has a large training data base. The peeling-off motion is clear and directional. Emphasizing muscle definition through lighting language improves results.
- **Reference image:** Fit woman in gym, mid-action of removing leggings, dramatic sports lighting.

#### 6.7 — Hotel Room Promo

```
A luxury hotel room promotion video. A beautiful woman in a silk robe enters the frame and walks toward a large window overlooking a city skyline at night. She drops the robe off her shoulders, revealing lingerie underneath, and leans against the window frame, gazing at the city. Camera follows her from the door to the window in a single tracking shot. Luxury hospitality marketing quality — warm, aspirational, slightly provocative. Moody evening tones, city lights bokeh.
```

- **Model:** Wan 2.6 I2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** The single tracking shot from door to window gives the model a clear camera path. Luxury hotel interiors are well-represented in training data. City skyline bokeh adds depth.
- **Reference image:** Woman in silk robe entering luxury hotel room, city view window, evening.

#### 6.8 — Jewelry Commercial

```
Extreme close-up beauty shot of a woman's neck and upper chest adorned with a diamond necklace. She breathes slowly, the necklace rising and falling. Light catches each facet of the diamonds, creating prismatic sparkles. Her skin is flawless, lit by a beauty dish from above. Camera very slowly pulls back to reveal more of the necklace and bare décolletage. Black background, all attention on the jewelry and skin. Tiffany commercial quality.
```

- **Model:** Wan 2.6 I2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Beginner
- **Pro tip:** Jewelry close-ups with breathing motion are simple and elegant. Wan 2.6's superior quality handles sparkle/prismatic effects best. Very commercial and shareable.
- **Reference image:** Close-up neck/chest with diamond necklace, beauty dish lighting, black background.

#### 6.9 — Body Lotion Application

```
A woman in a matching nude-tone bra and panty set sits on a white bed and applies body lotion to her legs. She squeezes lotion from a bottle into her palm, then slowly massages it into her calf and thigh with long upward strokes. Her skin takes on a healthy glow as the lotion absorbs. Camera follows her hands. Bright, clean beauty content lighting — soft and shadowless. Skincare brand commercial aesthetic, clean beauty vibes.
```

- **Model:** Wan 2.5 I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Beginner
- **Pro tip:** Product application videos are a huge commercial market. The repetitive stroking motion is easy for AI, and the result looks like legitimate brand content.
- **Reference image:** Woman applying lotion to leg, nude underwear, white bed, bright beauty lighting.

#### 6.10 — Fashion E-commerce Spin

```
A model stands on a turntable rotating slowly 360 degrees, wearing a sheer bodysuit with strategic opacity. Clean white e-commerce studio background. Arms relaxed at sides. The rotation reveals the garment from every angle. Bright, color-accurate product photography lighting from multiple softboxes. No distracting elements — pure product showcase. E-commerce product video standards, consistent exposure and white balance throughout rotation.
```

- **Model:** Wan 2.5 I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Beginner
- **Pro tip:** Turntable rotation videos are a standard e-commerce format. The consistent lighting and white background simplify generation significantly. Highly practical and commercial.
- **Reference image:** Model in sheer bodysuit, white background, standing straight, product photography lighting.

---

### Category 7: Anime / Hentai Style

#### 7.1 — Onsen Bath Scene

```
Anime-style illustration of a woman with long blue hair relaxing in a traditional Japanese hot spring (onsen). Steam rises from the milky mineral water. She is submerged to her collarbone, bare shoulders visible. She closes her eyes and sighs contentedly, sinking deeper. Autumn maple leaves drift across the water surface. Traditional wooden fence and rocks in background. Warm color palette, detailed anime art with soft shading. Ghibli-quality background art, KyoAni-level character animation.
```

- **Model:** Wan 2.5 T2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Onsen scenes are a classic anime trope with tons of training data. The water level provides natural censoring while remaining sensual. Specifying art studio styles (Ghibli, KyoAni) helps define the visual quality.
- **Reference image (if I2V):** Anime woman in onsen, blue hair, autumn setting, 2D illustration style.

#### 7.2 — Beach Episode Fanservice

```
Anime beach episode style. A busty anime girl in a tiny string bikini runs toward the camera on a sandy beach, breasts bouncing with the running motion. She trips and falls forward toward the camera with a surprised expression. Classic anime fanservice framing with speed lines and comedic effect. Bright, saturated summer colors. Cel-shaded animation style with clean outlines. Exaggerated anime proportions and physics. Beach umbrella and ocean sparkling in background.
```

- **Model:** Wan 2.5 T2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** "Beach episode" is a well-known anime trope that AI has learned. Specifying "anime proportions" and "cel-shaded" keeps it in 2D animation territory. Physics exaggeration is expected in this style.
- **Reference image (if I2V):** Anime girl in bikini on beach, running pose, 2D illustration, bright colors.

#### 7.3 — Transformation Sequence

```
Anime magical girl transformation sequence but adult-themed. A woman's clothing dissolves in sparkles of light, leaving her momentarily nude with strategic light flares, before new fantasy armor materializes around her body piece by piece. Dynamic camera rotation around the figure. Intense magical energy particles. Dramatic pose at the end with a weapon. Sailor Moon transformation style but more mature. Vibrant magical effects, dynamic action lines, dramatic lighting shifts.
```

- **Model:** Wan 2.6 T2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Advanced
- **Pro tip:** Transformation sequences are very popular and well-represented in training data. The magical particles and light effects provide natural coverage during the "nude" phase. Keep to one transformation direction.
- **Reference image (if I2V):** Anime character mid-transformation, sparkle effects, dynamic pose, 2D style.

#### 7.4 — Waifu Bedroom

```
Anime-style POV scene. A beautiful anime girl with pink hair and large eyes lies on a bed facing the viewer, wearing an oversized button-up shirt that's partially unbuttoned. She reaches one hand toward the camera with a gentle smile, as if beckoning. Her other hand rests on the pillow beside her head. Warm evening lighting from a bedside lamp. Soft, intimate framing. Detailed anime eyes with light reflections. Romantic visual novel CG quality, warm pastel color palette.
```

- **Model:** Wan 2.5 T2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Beginner
- **Pro tip:** POV waifu scenes are extremely popular in the anime AI community. The reaching hand creates a personal connection. Visual novel CG is a clear style reference. Simple hand movement is easy to generate.
- **Reference image (if I2V):** Anime girl on bed, POV perspective, oversized shirt, reaching toward camera, 2D art.

#### 7.5 — Tentacle Fantasy

```
Dark fantasy anime. A warrior woman in torn armor is partially restrained by glowing magical tentacles in a dungeon setting. The tentacles glow with bioluminescent patterns. She struggles against them, muscles tensed, expression defiant. Dark, atmospheric, with pools of colored light from the tentacles. Detailed anime illustration style with heavy shading. Gothic dark fantasy color palette — deep purples, blacks, glowing greens and blues. Dynamic composition with tentacles creating leading lines.
```

- **Model:** Wan 2.6 T2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Advanced
- **Pro tip:** Tentacle animations work well in AI video because they're organic, flowing shapes. The bioluminescence adds dynamic lighting. Keep the scene more suggestive than explicit for best visual quality.
- **Reference image (if I2V):** Anime warrior woman with glowing tentacles, dark fantasy, torn armor, 2D illustration.

#### 7.6 — Locker Room Anime

```
Anime slice-of-life style. Two anime girls in a school locker room after gym class. One is pulling her gym shirt over her head, revealing a sports bra. The other is wrapping a towel around herself, having just removed her uniform. Lockers and benches in the background. Bright fluorescent locker room lighting. Comedic anime framing with one girl blushing and the other oblivious. Light-hearted, humorous fanservice. Clean anime line art with pastel shading.
```

- **Model:** Wan 2.5 T2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Locker room scenes are a staple anime setting with clear visual conventions. Two-character anime scenes work better than two-character realistic scenes because the stylized aesthetic is more forgiving.
- **Reference image (if I2V):** Anime locker room scene, two girls, gym clothes/towels, bright lighting, 2D style.

#### 7.7 — Bathhouse Attendant

```
Anime-style illustration of a voluptuous woman in a traditional Japanese bathhouse, wearing only a small towel that barely covers her body. She kneels on the wet tile floor, wringing out a cloth over a wooden bucket. Steam fills the air. Water droplets on her skin. Traditional wood and stone bathhouse interior. She looks up at the viewer with a welcoming expression. Ukiyo-e inspired color palette — muted earth tones with pops of red and blue. Detailed background art, high-quality anime production values.
```

- **Model:** Wan 2.5 T2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Traditional Japanese settings combined with anime style benefit from art historical references like ukiyo-e. The wringing-cloth motion is simple and effective.
- **Reference image (if I2V):** Anime bathhouse attendant, small towel, traditional Japanese interior, kneeling, 2D art.

#### 7.8 — Demon Girl Dance

```
Anime-style demon girl with red skin, small horns, bat wings, and a spade tail dances seductively in a fire-lit cave. She wears minimal black leather straps as clothing. Her tail sways rhythmically as she moves. Fire reflects off her skin. She spins, wings spreading wide, then wraps them around herself. Dark fantasy meets nightclub energy. Bold anime style with thick outlines and dramatic shading. Red, orange, and black color scheme. Dynamic animation with smear frames during fast movements.
```

- **Model:** Wan 2.5 T2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 9:16
- **Difficulty:** Advanced
- **Pro tip:** Demon/monster girl designs are popular in the anime AI community. The fire provides dynamic lighting and animation. Specifying "smear frames" pushes the animation toward a more traditional 2D anime feel.
- **Reference image (if I2V):** Anime demon girl dancing in firelit cave, red skin, horns, wings, 2D style.

#### 7.9 — Ecchi Zero Gravity

```
Anime zero-gravity scene. An anime girl in a school uniform floats weightlessly in a spacecraft. Her skirt floats upward, revealing striped panties. Her hair fans out in zero-g. Loose papers and a pen float around her. She reaches for a floating coffee cup, stretching her body. Through the window, Earth is visible. Comedic, light-hearted ecchi. Clean modern anime style, high detail on fabric folds and hair. Smooth, dreamlike floating animation.
```

- **Model:** Wan 2.5 T2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Zero-gravity floating is naturally slow and dreamy, perfect for AI generation. Floating objects (papers, pen) add visual interest and are easy to animate. The ecchi element is classic and well-understood.
- **Reference image (if I2V):** Anime girl floating in zero-g, school uniform, spacecraft interior, 2D illustration.

#### 7.10 — Succubus Night Visit

```
Dark anime scene. A succubus with purple hair and glowing golden eyes hovers above a sleeping person, seen from above. Her translucent wings create shadow patterns on the bed below. She leans down slowly, long hair falling like a curtain. One finger touches the sleeper's lips. Moonlight through a window creates silver highlights on her pale skin. Atmospheric, romantic horror aesthetic. High-detail anime illustration with painterly background. Color palette: deep blues, purples, silver, and golden eye glow.
```

- **Model:** Wan 2.6 T2V
- **Resolution:** 1080p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Advanced
- **Pro tip:** The hovering/leaning motion is slow and controlled, ideal for AI. Moonlight creates a beautiful, limited color palette. The bird's-eye perspective is cinematic and unusual.
- **Reference image (if I2V):** Anime succubus hovering over bed, moonlit room, purple hair, golden eyes, 2D art.

---

### Category 8: Extreme / Explicit

> **Note:** These prompts contain explicit sexual content. Use Wan 2.2 Spicy for best explicit content generation. Keep duration short (5s) for best quality.

#### 8.1 — Solo Touch

```
A nude woman lies on a bed on her back, knees bent, one hand slowly moving down her body from her chest to her lower abdomen. Her back arches slightly, head pressing back into the pillow. Eyes closed, lips parted, expression of pleasure. Camera at mattress level, side angle. Warm amber bedroom lighting from one source. Tangled white sheets around her. Intimate, authentic, natural body movement. Shallow depth of field keeping focus on her face and hand.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** For explicit solo content, keep the camera at one angle. Side-angle lying poses produce the most anatomically consistent results. The hand movement should follow a clear path.
- **Reference image:** Nude woman lying on bed, hand on chest, warm lighting, side angle, artistic boudoir photo.

#### 8.2 — From Behind Pose

```
Medium shot from slightly above. A woman on all fours on a bed, facing away from camera. She looks back over her shoulder toward the camera with an inviting expression. She arches her back, creating a pronounced curve from shoulders to hips. Sheets are gathered around her knees. Warm soft lighting from above. Her hair falls over one shoulder. Cinematic quality, fashion boudoir aesthetic. Slow, subtle movement — she sways slightly, maintaining eye contact over her shoulder.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** The all-fours pose is well-understood by NSFW-trained models. Over-the-shoulder eye contact adds emotional connection. Keep the motion minimal.
- **Reference image:** Woman on all fours on bed, looking back over shoulder, warm lighting, boudoir style.

#### 8.3 — Riding Position

```
A woman straddles a man who is lying on his back. She is upright, hands on his chest, slowly rolling her hips in a rhythmic motion. Both are nude. Camera at mattress level from the side, showing both figures in profile. Her hair moves with the rhythm. Warm candlelight creates moving shadows. White sheets, dark room. Intimate, passionate. Focus on the hip motion and facial expression. Medium shot including both torsos.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Advanced
- **Pro tip:** Two-person explicit scenes are the most challenging. Side profile angle is essential. Keep duration to 5s maximum. Rhythmic hip motion is the single movement to focus on.
- **Reference image:** Side-view silhouette or artistic photo of woman in straddling position, candlelight, boudoir aesthetic.

#### 8.4 — Breast Reveal Close-Up

```
Extreme close-up of a woman's chest as she slowly pulls down the cups of a black lace bra, revealing her breasts. She cups them with both hands. Camera is at chest level, straight-on framing. Only her chest and hands are in frame — no face. Warm soft light from above and to the right. Skin has natural texture and tone. Simple dark background. The gesture is slow, confident, deliberate. High detail, sharp focus, beauty photography quality lighting.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Beginner
- **Pro tip:** Body-part close-ups without face are the most reliable explicit content. The bra-removal motion is a single directional movement that generates consistently. No face = no face distortion.
- **Reference image:** Close-up of chest in black lace bra, hands on cups, warm lighting, dark background.

#### 8.5 — Doggy Position

```
Two figures on a bed from a side-view camera angle. The woman is on her hands and knees, the man behind her. Both bodies move in synchronized rhythmic motion. Camera is at mattress level, medium-wide shot showing both full profiles. Dimly lit bedroom, warm tones. Sheets are crumpled beneath them. Focus on the rhythmic movement and body dynamics. Cinematic, warm color grading, shallow depth of field softening the background.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Advanced
- **Pro tip:** Always use side-profile for explicit couple scenes. The rhythmic motion should be clearly described as synchronized. Dim lighting is forgiving. Wan 2.2 Spicy is the only reliable model for this level of explicit content.
- **Reference image:** Artistic side-view boudoir photo of couple in position, dim warm lighting.

#### 8.6 — Spread Pose

```
A woman lies on her back on white sheets, slowly parting her legs while the camera captures from a slightly elevated front-facing angle. She wears thigh-high stockings, nothing else. Her hands rest on her inner thighs. She bites her lower lip. Soft, diffused lighting from a large overhead softbox. Clean, bright, high-key aesthetic. Beauty photography quality — flawless lighting and skin. Slow, controlled movement.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** High-key bright lighting actually works better than dark moody lighting for explicit anatomy — it gives the model more visual information to work with. Stockings provide a visual anchor for the legs.
- **Reference image:** Woman on white sheets, thigh-highs, bright lighting.

#### 8.7 — POV Oral

```
POV perspective looking down. A woman kneels on the floor between the viewer's legs, looking up at the camera with large eyes. She holds onto the viewer's thighs. Her head moves in a slow, rhythmic forward-and-back motion. Her hair sways with the movement. Camera is handheld POV with slight natural shake. Dimly lit room, her face lit from above. Intense eye contact maintained. Realistic, intimate POV aesthetic.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Advanced
- **Pro tip:** POV explicit scenes are challenging because the face must remain consistent while moving. Keep the motion extremely subtle — more implied than explicit works better. The eye contact and head motion suggest the action without requiring anatomical detail.
- **Reference image:** POV-angle photo of woman looking up at camera, kneeling, warm lighting.

#### 8.8 — Missionary Close-Up

```
Close-up side view of two bodies in missionary position. The camera frames from their chests to mid-thigh from the side. Rhythmic motion of the man's body. Her legs wrap around his waist. Her fingernails press into his back. Sweat glistens on both bodies. Only their torsos are visible — no faces in frame. Warm, dark, intimate lighting. The close framing and lack of faces makes this abstract, almost sculptural. Slow, steady rhythm.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Advanced
- **Pro tip:** Removing faces from explicit couple scenes dramatically improves quality. The side-view torso framing reduces the scene to rhythmic motion of forms, which AI handles better than full anatomical detail. Sweat descriptions add realism.
- **Reference image:** Artistic close-up of two torsos, side view, intimate lighting, abstract framing.

#### 8.9 — Climax Expression

```
Extreme close-up of a woman's face during climax. Her eyes squeeze shut, mouth opens, head tilts back. Muscles in her neck tense. A flush spreads across her cheeks. One hand grips the pillow beside her head. Slow motion captures every micro-expression. Camera very close, face filling the frame. Warm soft lighting from one side. The focus is entirely on her expression — nothing else visible. Raw, authentic, emotional. Hyper-detailed, every pore and eyelash visible.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Intermediate
- **Pro tip:** Face-only clips are much easier than full-body explicit content. The expression sequence (tension to release) is a clear emotional arc. Use a high-quality face photo as reference.
- **Reference image:** Close-up photo of woman's face, eyes closed, expression of pleasure, warm side lighting.

#### 8.10 — Walking Away

```
Close-up tracking shot following a nude woman's hips and buttocks as she walks slowly away from the camera. Each step creates natural movement in her glutes and thighs. Camera at hip height, tight framing on her lower body only. She walks down a hallway — no face visible, just her lower body in motion. Warm side lighting creates shadows that define muscle tone. Slow motion, detailed, hyper-realistic. Clean background, attention entirely on the body movement.
```

- **Model:** Wan 2.2 Spicy I2V
- **Resolution:** 720p | **Duration:** 5s | **Aspect Ratio:** 16:9
- **Difficulty:** Beginner
- **Pro tip:** Walking-away shots are one of the easiest explicit prompts — the motion is natural and well-understood, and no face is involved. The tracking camera follows a simple straight line.
- **Reference image:** Close-up of hips/buttocks from behind, walking pose, warm side lighting, hallway background.

---

## Prompt Engineering Deep Dive

### Keywords That Work Well

**Body descriptions:**
- Specific terms: "slender waist," "athletic build," "curvy hips," "toned abs," "full bust," "petite frame"
- Skin descriptions: "sun-kissed skin," "porcelain skin," "olive complexion," "dark mahogany skin," "freckled," "oiled/glistening"
- Avoid vague terms like "hot body" or "sexy figure" — be specific about what makes it attractive

**Camera language that AI understands:**

| Term | Effect |
|------|--------|
| `push in` | Camera moves toward subject |
| `pull back / dolly out` | Camera moves away from subject |
| `tracking shot` | Camera follows subject laterally |
| `pan left/right` | Camera rotates horizontally |
| `tilt up/down` | Camera rotates vertically |
| `static camera` | Camera doesn't move |
| `handheld` | Slight natural shake |
| `drone shot` | High, sweeping, smooth |
| `POV` | First-person perspective |
| `low angle` | Camera below subject, looking up |
| `high angle` | Camera above subject, looking down |
| `bird's eye / overhead` | Directly above looking straight down |
| `Dutch angle` | Camera tilted diagonally |
| `rack focus` | Focus shifts from one subject to another |
| `shallow DOF` | Blurred background, sharp subject |

**Lighting setups for different moods:**

| Mood | Lighting Description |
|------|---------------------|
| Romantic | "Warm candlelight, golden tones, soft diffused" |
| Dramatic | "Single hard light source, deep shadows, chiaroscuro" |
| Ethereal | "Backlit, overexposed highlights, hazy, bloom effect" |
| Raw/Gritty | "Harsh overhead fluorescent, unflattering, direct" |
| Luxury | "Multiple soft sources, no harsh shadows, beauty dish" |
| Mysterious | "Rim light only, face in shadow, silhouette" |
| Natural | "Window light, golden hour, ambient, no artificial" |

**Motion keywords ranked by reliability:**

1. **Most reliable:** breathing, blinking, hair blowing, fabric billowing, water flowing, smoke drifting
2. **Reliable:** slow turn, head tilt, hand movement, walking, swaying
3. **Moderate:** dancing, stretching, undressing, running
4. **Challenging:** complex choreography, two-person interaction, transformation
5. **Hardest:** rapid action, multiple simultaneous movements, physics-defying motion

### How to Avoid Common Artifacts

| Artifact | Prevention Strategy |
|----------|-------------------|
| Extra fingers/limbs | Keep hands out of frame or in simple poses (fist, flat, gripping) |
| Face distortion | Use blindfolds, back-to-camera, silhouettes, or close-up body shots |
| Body morphing | Shorter clips (5s), simpler motions, single-person scenes |
| Flickering | Add "smooth, consistent lighting" to prompt; avoid complex multi-source lighting |
| Background warping | Simple backgrounds (solid color, blurred bokeh); static camera |
| Clothing inconsistency | Describe specific, simple garments; avoid complex patterns |
| Anatomy errors | Side-profile views for full body; close-ups for specific body parts |
| Two-person merge | Clear separation between figures; side-view; different clothing colors |

### Negative Prompt Strategies

For models that support negative prompts:

```
deformed, distorted, disfigured, bad anatomy, extra limbs, extra fingers,
mutated hands, poorly drawn hands, poorly drawn face, mutation, ugly, blurry,
low quality, watermark, text, logo, signature, extra arms, extra legs, fused fingers,
too many fingers, long neck, cross-eyed, worst quality, jpeg artifacts
```

**NSFW-specific negatives:**
```
unrealistic proportions, plastic skin, mannequin, doll-like, uncanny valley,
airbrushed skin, unnatural body position, broken spine, impossible pose, floating limbs,
disconnected body parts, misaligned anatomy, asymmetric features
```

### Duration Optimization

| Content Type | Optimal Duration | Why |
|-------------|-----------------|-----|
| Simple pose/breathing | 3-5s | Minimal motion, quality preserved |
| Single gesture (hand, head turn) | 5s | One clear action |
| Walking/simple movement | 5s | Consistent motion |
| Dance/complex movement | 5s | Longer = more artifacts |
| Two-person scenes | 5s max | Complexity demands short clips |
| Explicit scenes | 5s max | Anatomy consistency degrades over time |
| Looping content | 3-5s | Design for seamless loop |

**Rule of thumb:** When in doubt, choose 5 seconds. Quality always beats length. You can stitch clips together in post-production.

---

## Workflow: Image-to-Video NSFW Pipeline

### Step 1: Generate Reference Image

Use **Flux Dev** or **Seedream** on [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=nsfw-ai-video-prompts) — both are NSFW capable.

**Tips for reference images:**
- Generate the exact pose you want as the starting frame
- Match the lighting described in your video prompt
- Include the exact clothing/state of undress you want
- Higher resolution reference = better video quality
- Avoid complex backgrounds — they can confuse the I2V model

**Example image prompt for Flux Dev:**
```
Professional boudoir photography of a woman in black lace lingerie lying on a bed.
Warm golden lamp light from the side. Shallow depth of field. 35mm film aesthetic.
She looks directly at camera with a subtle smile. High quality, detailed, realistic.
```

### Step 2: Animate with Wan 2.2 Spicy I2V (from $0.03 per second)

Take your generated image and pair it with a motion prompt:

```
She slowly arches her back and runs one hand through her hair, then turns
her head to look over her shoulder. Smooth, slow movement. Cinematic quality.
```

**I2V best practices:**
- The video prompt should describe MOTION, not appearance (appearance comes from the image)
- Keep motion descriptions simple and directional
- Avoid contradicting the reference image (don't describe different clothing)
- Specify camera movement separately from subject movement

### Step 3: Iterate and Refine

- Generate 3-5 variations of the same prompt to pick the best one
- At from $0.03 per second, 5 attempts = ~$0.15 — still extremely cheap
- Small wording changes can dramatically affect results
- Try different reference images with the same prompt

### Step 4: Post-Processing

- **Upscale** with Real-ESRGAN or Topaz Video AI for higher resolution
- **Slow motion** in post can smooth any jerkiness
- **Color grade** in DaVinci Resolve (free) for a professional look
- **Stitch clips** together for longer sequences
- **Add audio** — music, ambient sound, or use Seedance v1.5 for built-in audio sync

---

## API Quick Start

### cURL

```bash
# 使用 Atlas Cloud API 生成 NSFW 视频
curl -s -X POST "https://api.atlascloud.ai/v1/predictions" \
  -H "Authorization: Bearer $ATLAS_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "wan-2.2-spicy-i2v",
    "input": {
      "prompt": "She slowly arches her back and runs one hand through her hair. Smooth cinematic movement, warm lighting.",
      "image": "https://your-image-url.com/reference.jpg",
      "duration": 5,
      "resolution": "720p",
      "aspect_ratio": "16:9"
    }
  }'
```

### Python

```python
"""
使用 Atlas Cloud API 批量生成 NSFW 视频的示例脚本
"""
import requests
import time

# Atlas Cloud API 配置
API_KEY = "your_api_key_here"
BASE_URL = "https://api.atlascloud.ai/v1"
HEADERS = {
    "Authorization": f"Bearer {API_KEY}",
    "Content-Type": "application/json"
}


def generate_nsfw_video(prompt: str, image_url: str = None, model: str = "wan-2.2-spicy-i2v"):
    """
    生成单个 NSFW 视频

    参数:
        prompt: 视频生成提示词
        image_url: 参考图片 URL（I2V 模型需要）
        model: 使用的模型名称
    """
    payload = {
        "model": model,
        "input": {
            "prompt": prompt,
            "duration": 5,
            "resolution": "720p",
            "aspect_ratio": "16:9"
        }
    }

    # 如果是 I2V 模型，添加参考图片
    if image_url:
        payload["input"]["image"] = image_url

    # 创建预测任务
    response = requests.post(f"{BASE_URL}/predictions", headers=HEADERS, json=payload)
    prediction = response.json()
    prediction_id = prediction["id"]
    print(f"任务已创建: {prediction_id}")

    # 轮询等待结果
    while True:
        result = requests.get(f"{BASE_URL}/predictions/{prediction_id}", headers=HEADERS).json()
        status = result["status"]

        if status == "succeeded":
            video_url = result["output"]["video"]
            print(f"视频生成成功: {video_url}")
            return video_url
        elif status == "failed":
            print(f"生成失败: {result.get('error', '未知错误')}")
            return None

        print(f"状态: {status}，等待中...")
        time.sleep(3)


def batch_generate(prompts: list, image_url: str = None):
    """
    批量生成多个视频

    参数:
        prompts: 提示词列表
        image_url: 共享的参考图片 URL
    """
    results = []
    for i, prompt in enumerate(prompts):
        print(f"\n--- 正在生成第 {i+1}/{len(prompts)} 个视频 ---")
        video_url = generate_nsfw_video(prompt, image_url)
        results.append({"prompt": prompt, "video_url": video_url})
    return results


# 使用示例
if __name__ == "__main__":
    # 单个视频生成
    prompt = (
        "She slowly arches her back and runs one hand through her hair, "
        "then turns her head to look over her shoulder. "
        "Smooth, slow movement. Cinematic warm lighting."
    )
    reference_image = "https://your-image-url.com/reference.jpg"
    video = generate_nsfw_video(prompt, reference_image)

    # 批量生成示例
    batch_prompts = [
        "She slowly turns toward the camera, running fingers through her hair. Warm golden light, cinematic.",
        "She lies back on the bed and stretches her arms overhead. Soft bedroom lighting, slow motion.",
        "She walks slowly away from camera, looking back over her shoulder. Dim hallway, dramatic shadows.",
    ]
    results = batch_generate(batch_prompts, reference_image)
    print(f"\n生成完成! 成功: {sum(1 for r in results if r['video_url'])}/{len(results)}")
```

---

## FAQ

### What is the best AI for NSFW video generation?

**Wan 2.2 Spicy I2V** on [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=nsfw-ai-video-prompts) is the best balance of quality, explicit capability, and price (from $0.03 per second). For highest visual quality, use **Wan 2.6** (from $0.07 per second). For audio-synced content, use **Seedance v1.5 Pro**.

### What is the cheapest NSFW video API?

Atlas Cloud's **Wan 2.2 Spicy** at **from $0.03 per second** is the cheapest option. Sign up with [this link](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=nsfw-ai-video-prompts) for 25% bonus on your first top-up.

### How do I generate AI adult content?

1. Sign up on [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=nsfw-ai-video-prompts)
2. Generate a reference image using Flux Dev or Seedream (both NSFW capable)
3. Use that image with Wan 2.2 Spicy I2V and a motion prompt from this collection
4. Cost: from $0.03 per second

### Wan Spicy vs Wan 2.6 for NSFW — which is better?

- **Wan 2.2 Spicy**: Better for explicit content, cheaper ($0.03), trained specifically for NSFW with LoRA optimization. Best for nudity, explicit scenes, and budget production.
- **Wan 2.6**: Better visual quality overall, handles complex scenes better, up to 1080p/15s. Best for artistic nude, couple scenes, and commercial-quality output.

### How to avoid bad anatomy in AI NSFW video?

1. Use close-up body shots instead of full-body wide angles
2. Keep hands out of frame or in simple positions
3. Use side-profile views for full-body shots
4. Shorter clips (5s) maintain better consistency
5. Add "detailed anatomy, realistic proportions" to prompts
6. Use negative prompts: "deformed, extra limbs, bad anatomy"

### Can I generate explicit content commercially?

Check your local laws. Atlas Cloud's terms of service allow NSFW content generation on whitelisted models. You are responsible for compliance with all applicable laws regarding adult content in your jurisdiction.

### How long should NSFW AI videos be?

**5 seconds** is the sweet spot. Quality degrades significantly in longer clips, especially for explicit content. For longer videos, generate multiple 5-second clips and stitch them together in post-production.

### Why are my results blurry or low quality?

1. Use a higher quality reference image (for I2V models)
2. Upgrade to Wan 2.6 for 1080p output
3. Add quality keywords: "high detail, sharp focus, 4K, cinematic quality"
4. Use negative prompts: "blurry, low quality, jpeg artifacts"
5. Upscale the output with Real-ESRGAN or Topaz Video AI

---

## Get Started

1. **Sign up** on [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=nsfw-ai-video-prompts) — get **25% bonus credit** on your first top-up (up to $100 extra)
2. **Copy** any prompt from this collection
3. **Generate** your first NSFW video for $0.03
4. **Star** this repo to save it for later

---

## Related Resources

- [Wan 2.2 Spicy LoRA Guide](https://github.com/ristponex/wan-2.2-spicy-lora-nsfw) — Full LoRA guide
- [AI Video LoRA Guide](https://github.com/ristponex/ai-video-lora-guide) — General LoRA tutorial
- [NSFW AI API Comparison](https://github.com/ristponex/nsfw-ai-api-comparison) — Platform comparison
- [Awesome NSFW AI Video](https://github.com/ristponex/awesome-nsfw-ai-video) — Curated resource list

---

## Contributing

Have prompts that produce great results? Submit a pull request. Include:
- The full prompt text
- Which model you used
- Sample output description
- Any tips for getting the best results

---

## License

MIT License. Prompts are free to use for any purpose. Generated content is subject to the terms of the model provider and applicable laws.

---

**[Atlas Cloud](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=nsfw-ai-video-prompts)** — Uncensored AI Video Generation Starting at $0.03
