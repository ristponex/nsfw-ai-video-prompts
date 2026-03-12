<div align="center">

```
 _   _  ______        ______        ___    ___   __     __ _     _
| \ | |/ ___\ \      / /  __|      / _ \  |_ _|  \ \   / /(_) __| | ___  ___
|  \| |\___ \\ \ /\ / /| |_       / /_\ \  | |    \ \ / / | |/ _` |/ _ \/ _ \
| |\  | ___) |\ V  V / |  _|     / _____ \ | |     \ V /  | | (_| |  __/ (_) |
|_| \_||____/  \_/\_/  |_|      /_/     \_\|___|    \_/   |_|\__,_|\___|\___/

 提示词库 — 100+ 即开即用的 NSFW AI 视频提示词
```

# NSFW AI 视频提示词库 — 100+ 条详细提示词，分类整理，即拿即用

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![提示词数量](https://img.shields.io/badge/提示词-100+-blue)]()
[![支持模型](https://img.shields.io/badge/支持模型-5个无审核-red)]()
[![最后更新](https://img.shields.io/badge/更新日期-2026年3月-green)]()
[![平台](https://img.shields.io/badge/平台-Atlas%20Cloud-purple)](https://www.atlascloud.ai?ref=JPM683)

**全网最大的开源 NSFW AI 视频提示词合集。每条提示词都经过实测，按场景分类，针对各模型优化。**

**[English](./README.md)** | **[简体中文](./README_zh-CN.md)** | **[日本語](./README_ja.md)** | **[한국어](./README_ko.md)**

---

> **免责声明：** 本仓库仅供合法成人内容创作使用。所有提示词仅限成年人（18+）在当地法律允许的地区使用。我们严格反对任何涉及未成年人、非自愿场景或其他违法内容的创作。使用者须自行确保符合当地法律法规。

</div>

---

## 目录

- [支持模型与价格](#支持模型与价格)
- [价格对比：Atlas Cloud vs fal.ai](#价格对比atlas-cloud-vs-falai)
- [快速开始（API）](#快速开始api)
- [提示词工程基础](#提示词工程基础)
- [分类一：浪漫情感（20 条）](#分类一浪漫情感20-条)
- [分类二：艺术裸体与人体研究（15 条）](#分类二艺术裸体与人体研究15-条)
- [分类三：内衣与时尚（15 条）](#分类三内衣与时尚15-条)
- [分类四：奇幻与神话（15 条）](#分类四奇幻与神话15-条)
- [分类五：动漫与成人动画（15 条）](#分类五动漫与成人动画15-条)
- [分类六：显性内容（15 条）](#分类六显性内容15-条)
- [分类七：电影叙事（10 条）](#分类七电影叙事10-条)
- [分类八：特殊偏好（10 条）](#分类八特殊偏好10-条)
- [模型专属优化指南](#模型专属优化指南)
- [高级提示词技巧](#高级提示词技巧)
- [批量生成脚本](#批量生成脚本)
- [常见问题](#常见问题)
- [开始使用](#开始使用)
- [Star 趋势](#star-趋势)
- [许可证](#许可证)

---

## 支持模型与价格

以下模型均可通过 [Atlas Cloud API](https://www.atlascloud.ai?ref=JPM683) 使用，且已开通 NSFW 内容生成权限。

| 模型 | 类型 | 价格 | 分辨率 | 时长 | NSFW 程度 | 最佳用途 |
|:-----|:-----|:-----|:-------|:-----|:----------|:---------|
| **Wan 2.2 Spicy** | I2V / I2V-LoRA | **$0.03**/次 | 480p, 720p | 5s, 8s | 完全无限制 | 低成本显性内容 |
| **Wan 2.5** | I2V / T2V | ~$0.05/次 | 720p, 1080p | 5s, 10s | 裸体 + 中等显性 | 中等质量 |
| **Wan 2.6** | I2V / T2V | $0.07/次 | 最高 1080p | 5–15s | 裸体（有限显性） | 高质量艺术裸体 |
| **Seedance v1.5 Pro** | T2V / I2V | **$0.222**/次 | 720p | 5–15s | 白名单 NSFW | 顶级电影质感 |
| **Vidu Q3-Pro** | T2V / I2V | **$0.06**/次 | 720p, 1080p | 5–10s | 白名单 NSFW | 质量/价格均衡 |
| **Kling v3.0 Pro** | T2V / I2V | **$0.204**/次 | 最高 1080p | 5–10s | 白名单 NSFW | 运动质量、面部 |

> **白名单**表示在 Atlas Cloud 平台上经审批后可生成 NSFW 内容，标准安全过滤已为白名单账户关闭。Vidu 系列同样已开通白名单 NSFW 内容生成。

### 信任与安全

- **SOC I & II 认证** — 企业级安全合规
- **HIPAA 合规** — 医疗级数据保护
- **美国注册公司** — 受美国数据保护法管辖
- **首次充值赠送 25%**（最高赠送 $100）— [立即注册](https://www.atlascloud.ai?ref=JPM683)
- **支持微信/支付宝直接付款** — 无需国际信用卡，对国内用户友好

---

## 价格对比：Atlas Cloud vs fal.ai

如果你一直在用 fal.ai，下面是你多花的钱：

### Wan 模型（5秒视频）

| 平台 | 计费方式 | 5秒视频费用 | 100个视频费用 |
|:-----|:---------|:-----------|:-------------|
| **Atlas Cloud** | 按次计费 | **$0.05** | **$5.00** |
| fal.ai | 按秒计费 ($0.05/秒) | $0.25 | $25.00 |
| **节省** | | **80%** | **$20.00** |

### Kling 模型（5秒视频）

| 平台 | 计费方式 | 5秒视频费用 | 100个视频费用 |
|:-----|:---------|:-----------|:-------------|
| **Atlas Cloud** | 按次计费 | **$0.204** | **$20.40** |
| fal.ai | 按秒计费 ($0.224/秒) | $1.12 | $112.00 |
| **节省** | | **82%** | **$91.60** |

### Wan 2.2 Spicy（Atlas Cloud 独家）

| 平台 | 5秒视频费用 | 100个视频费用 | 1000个视频费用 |
|:-----|:-----------|:-------------|:--------------|
| **Atlas Cloud** | **$0.03** | **$3.00** | **$30.00** |
| fal.ai | 不提供 | 不提供 | 不提供 |

> fal.ai 不提供无审核/NSFW 模型。Atlas Cloud 是极少数提供完全无限制 NSFW 视频生成 API 的平台之一。

---

## 快速开始（API）

### 前置条件

1. 在 [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683) 注册账号
2. 充值（首次充值赠送 25%，最高赠送 $100，支持微信/支付宝）
3. 在控制面板复制 API Key

### Python — 完整流程

```python
"""
NSFW AI Video Generation — Complete Python Example
Supports: Wan 2.2 Spicy, Wan 2.5/2.6, Seedance, Vidu, Kling
Platform: Atlas Cloud (https://www.atlascloud.ai?ref=JPM683)
"""

import requests
import time
import os

API_KEY = os.environ.get("ATLAS_API_KEY", "your_api_key_here")
BASE_URL = "https://api.atlascloud.ai/v1"
HEADERS = {
    "Authorization": f"Bearer {API_KEY}",
    "Content-Type": "application/json"
}


def generate_nsfw_video(prompt: str, model: str = "alibaba/wan-2.2-spicy/image-to-video",
                        image_url: str = None, resolution: str = "720p",
                        duration: int = 5) -> str:
    """
    Generate an NSFW video using Atlas Cloud API.

    Args:
        prompt: Video generation prompt (detailed scene description)
        model: Model identifier on Atlas Cloud
        image_url: Reference image URL (required for I2V models)
        resolution: Output resolution ("480p", "720p", "1080p")
        duration: Video duration in seconds

    Returns:
        Video URL string
    """
    payload = {
        "model": model,
        "input": {
            "prompt": prompt,
            "resolution": resolution,
            "duration": duration,
        }
    }

    # Add reference image for image-to-video models
    if image_url:
        payload["input"]["image"] = image_url

    # Submit generation request
    response = requests.post(
        f"{BASE_URL}/predictions",
        headers=HEADERS,
        json=payload
    )
    response.raise_for_status()
    prediction_id = response.json()["id"]
    print(f"Submitted: {prediction_id}")

    # Poll for completion
    for _ in range(120):  # 10 minute timeout
        time.sleep(5)
        result = requests.get(
            f"{BASE_URL}/predictions/{prediction_id}",
            headers=HEADERS
        ).json()

        status = result.get("status")
        if status == "succeeded":
            video_url = result.get("output", {}).get("video")
            if isinstance(result.get("output"), list):
                video_url = result["output"][0]
            print(f"Done! Video: {video_url}")
            return video_url
        elif status in ("failed", "canceled"):
            raise RuntimeError(f"Generation failed: {result.get('error', 'Unknown')}")

    raise TimeoutError("Generation timed out after 10 minutes")


# ── Example ──────────────────────────────────────────────────────
if __name__ == "__main__":
    prompt = (
        "A woman in a sheer silk robe stands by a floor-to-ceiling window at golden hour. "
        "She slowly turns toward the camera, the robe sliding off one shoulder. "
        "Warm sunlight traces the contours of her body. "
        "Shallow depth of field, cinematic color grading, slow sensual motion."
    )

    video = generate_nsfw_video(
        prompt=prompt,
        model="alibaba/wan-2.2-spicy/image-to-video",
        image_url="https://example.com/reference.jpg",
        resolution="720p",
        duration=5
    )
```

### cURL — 快速测试

```bash
# Submit NSFW video generation request
curl -s -X POST "https://api.atlascloud.ai/v1/predictions" \
  -H "Authorization: Bearer $ATLAS_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "alibaba/wan-2.2-spicy/image-to-video",
    "input": {
      "image": "https://example.com/reference.jpg",
      "prompt": "The woman reclines on silk sheets, arching her back slowly. Soft warm studio lighting. Her fingers trace along her collarbone. Cinematic, shallow depth of field.",
      "resolution": "720p",
      "duration": 5
    }
  }'

# Poll result (replace PREDICTION_ID)
curl -s "https://api.atlascloud.ai/v1/predictions/PREDICTION_ID" \
  -H "Authorization: Bearer $ATLAS_API_KEY"
```

---

## 提示词工程基础

在使用提示词库之前，掌握以下核心原则能让你的生成质量有质的飞跃。

### 六要素 NSFW 视频提示词公式

每条高质量 NSFW 视频提示词都应该包含以下六个要素：

```
[主体人物] + [动作/运动] + [场景/环境] + [灯光] + [镜头] + [风格/氛围]
```

| 要素 | 作用 | 示例 |
|:-----|:-----|:-----|
| **主体人物** | 谁在画面里 | "A tall woman with long dark hair and olive skin" |
| **动作/运动** | 发生了什么（视频核心） | "slowly removes her dress, letting it fall to the floor" |
| **场景/环境** | 在什么地方 | "in a minimalist loft apartment with exposed brick walls" |
| **灯光** | 影响皮肤渲染和氛围 | "warm golden hour light streaming through venetian blinds" |
| **镜头** | 画面怎么拍 | "medium shot, slight low angle, shallow depth of field" |
| **风格/氛围** | 整体视觉和情感调性 | "cinematic, sensual, intimate atmosphere" |

### NSFW 专属技巧

**1. 需要时明确描述身体细节**
- 差：「She takes off her clothes」
- 好：「She slowly unbuttons her blouse from top to bottom, revealing a black lace bralette underneath. The fabric parts to show her midriff and décolletage.」

**2. 按时间顺序描述动作**
- 差：「She dances seductively」
- 好：「She sways her hips left and right in a slow rhythm, raises her arms above her head, then slowly runs her hands down along her body from chest to thighs.」

**3. 灯光是皮肤渲染的关键**
- 「Soft diffused studio lighting with a warm key light at 45 degrees」比「bright lighting」效果好 10 倍
- 「Rim lighting highlighting body contours」能创造戏剧性轮廓
- 「Candlelight」增加温暖感但会降低细节

**4. 指定不要做什么（反向提示）**
- 添加：「No morphing, no distortion, no extra limbs, consistent body proportions throughout」
- 针对面部：「Consistent facial features, no face warping between frames」

**5. 时长影响提示词复杂度**
- 5 秒视频：最多描述 1-2 个动作
- 8-10 秒视频：可以处理 2-3 个连续动作
- 15 秒视频：可以描述一个有 3-4 个节拍的微型叙事

### 各模型最佳提示词长度

| 模型 | 最佳提示词长度 | 备注 |
|:-----|:-------------|:-----|
| Wan 2.2 Spicy | 40–80 词 | 更短的提示词 = 更少的瑕疵 |
| Wan 2.5/2.6 | 60–120 词 | 能处理复杂描述 |
| Seedance v1.5 | 80–150 词 | 详细描述能获得更好效果 |
| Vidu Q3-Pro | 50–100 词 | 善于理解简洁精炼的提示词 |
| Kling v3.0 Pro | 60–120 词 | 详细的面部描述回报率最高 |

---

## 分类一：浪漫情感（20 条）

聚焦亲密关系、情感连接和感官体验。推荐模型：**Wan 2.6**、**Kling v3.0 Pro**、**Seedance v1.5 Pro**。

### RS-01: 黄金时刻窗边

```
A woman with sun-kissed skin and wavy auburn hair stands barefoot by an open window,
wearing only a loose white linen shirt that reaches mid-thigh. A warm breeze pushes the
sheer curtains inward, pressing the fabric against her body and revealing her silhouette.
She closes her eyes, tilts her head back, and inhales deeply, her chest rising. The golden
hour sun creates a warm halo around her figure. Medium shot, soft focus background,
cinematic color grading with warm amber tones.
```

### RS-02: 清晨醒来

```
Close-up transitioning to medium shot. A woman lies on rumpled white sheets, bare shoulders
and upper back visible. She slowly rolls onto her side, pulling the sheet loosely across
her chest. Morning light filters through sheer curtains, casting soft shadows across her
skin. She reaches one arm above her head and stretches languidly, the sheet slipping to
reveal her waist. Sleepy, satisfied expression. Warm, intimate atmosphere. Shallow depth
of field on her face.
```

### RS-03: 烛光浴缸

```
A woman reclines in a freestanding clawfoot bathtub filled with milky water and rose petals.
Dozens of candles surround the tub on the marble floor. She lifts one leg slowly out of the
water, water droplets catching the candlelight as they trail down her shin. She runs a hand
along her wet collarbone. Steam rises softly. Warm amber lighting, overhead wide shot slowly
pushing in to a medium close-up. Relaxed, luxurious mood.
```

### RS-04: 阳台雨中

```
A woman in a soaked white tank top and cotton shorts stands on a balcony during a warm
summer rainstorm. The wet fabric clings to every curve of her body, becoming translucent.
She tilts her face up to the rain, eyes closed, water streaming down her neck and chest.
She slowly pushes wet hair back from her face with both hands, arching her back slightly.
Moody blue-grey sky in the background, warm skin tones. Medium shot, slight upward angle.
```

### RS-05: 丝绸睡袍

```
A woman with sleek black hair stands in a dimly lit bedroom. She is wearing a burgundy
silk robe loosely tied at the waist. She slowly pulls the sash, the robe falling open to
reveal a matching silk slip underneath that barely reaches her upper thighs. She lets the
robe slide off her shoulders and drop to the floor. Side lighting from a bedside lamp
creates dramatic shadows along her figure. Slow, deliberate movement. Tight medium shot
from the waist up, then tilts down as the robe falls.
```

### RS-06: 双人淋浴

```
A couple stands together under a large rainfall shower head. Water cascades over both
bodies. The man stands behind the woman, his arms wrapped around her waist. She leans
her head back against his chest, eyes closed. Water streams between their bodies. Both
are shown from the shoulders up and waist. Steam fills the glass enclosure. Warm soft
lighting. Slow motion water droplets. Intimate, tender atmosphere. Shot through the
slightly fogged glass door.
```

### RS-07: 黄昏海滩

```
A woman in a tiny black bikini walks along the shoreline at sunset. Waves lap at her
ankles. She pauses, facing the ocean, and slowly reaches behind her back to untie the
bikini top. She holds it in one hand at her side, back to camera, silhouetted against
the orange and purple sky. Her long hair blows in the sea breeze. Wide shot with the
sun low on the horizon. Warm cinematic color grading. Peaceful, free, confident energy.
```

### RS-08: 镜前自赏

```
A woman stands before a large ornate floor mirror in her bedroom, wearing only matching
black lace underwear. She turns slowly, examining herself from different angles. She runs
her fingertips along her hip and up her ribcage. The camera captures both her and her
reflection simultaneously, creating a dual perspective. Soft warm side lighting from a
lamp off-screen. Medium full-body shot. Self-assured, appreciative expression. Intimate
boudoir atmosphere.
```

### RS-09: 精油按摩

```
A woman lies face down on a massage table, a white sheet draped low across her hips. Her
bare back glistens with massage oil. A pair of hands enters the frame, pressing firmly
along her spine from lower back to shoulders. She exhales deeply, her shoulder blades
shifting under the skin. Oil catches the warm overhead light. Close-up on hands working
muscle groups, then pulls back to a medium shot. Relaxing ambient mood. Soft focused
background.
```

### RS-10: 壁炉夜

```
A woman sits on a plush fur rug in front of a roaring fireplace, wearing an oversized
knit sweater and nothing else. She draws her bare legs up to one side, the sweater riding
up to her upper thighs. She holds a glass of red wine, takes a slow sip, and gazes into
the fire. Warm flickering firelight dances across her skin and legs. The room is otherwise
dark. Tight medium shot. Cozy, seductive atmosphere. Shallow depth of field with bokeh
from the fire.
```

### RS-11: 舞池慢摇

```
Low-key club lighting with deep purple and blue tones. A woman in a backless sequined
mini dress moves her body in a slow, hypnotic rhythm. She runs one hand down her neck to
her chest as she sways. Her back is arched, hips moving in a figure-eight pattern. Sweat
glistens on her shoulders and décolletage. Slow motion captures the fabric catching the
light. Medium shot from slightly below eye level. Smoky, charged atmosphere.
```

### RS-12: 露天温泉

```
A woman sits in a natural hot spring pool surrounded by snow-covered rocks and pine trees.
Steam rises thickly around her. She is submerged to her collarbone. She slowly stands up
in the pool, water cascading off her body, revealing her bare shoulders, back, and waist
as she rises. She wrings out her long wet hair. Misty mountain backdrop. Natural overcast
lighting. Wide establishing shot transitioning to medium shot as she stands. Serene,
ethereal mood.
```

### RS-13: 复古闺房

```
Styled as a 1940s glamour photograph come to life. A woman with victory rolls hairstyle
and red lipstick reclines on a chaise longue wearing a vintage corset, garter belt, and
seamed stockings. She slowly extends one leg upward, pointing her toe, running her hand
along the stocking from ankle to thigh. Soft focus lens effect. Warm sepia-toned lighting.
Medium shot with slight Dutch angle. Old Hollywood glamour aesthetic.
```

### RS-14: 天台落日

```
A woman stands alone on an urban rooftop at sunset, city skyline in the distance. She is
wearing a flowing summer dress. She reaches down, grabs the hem, and slowly lifts the dress
up and over her head in one fluid motion, revealing a simple nude-toned bra and underwear.
She tosses the dress aside and stands with arms slightly open, facing the setting sun.
Wind catches her hair. Wide shot with shallow depth of field on the city background.
Liberating, confident mood.
```

### RS-15: 丝绸撩拨

```
A woman lies on dark navy silk sheets, her body partially concealed and partially revealed
by the fabric. She slowly pulls the sheet downward from her collarbone, revealing her bare
chest, while simultaneously drawing one knee up, the sheet draping between her legs. She
bites her lower lip subtly and maintains eye contact with the camera. Overhead bird's eye
view slowly rotating. Single dramatic spotlight creating deep shadows. Provocative, intense.
```

### RS-16: 双人慢舞

```
A couple in a dimly lit living room dances slowly, no music audible. She wears only his
unbuttoned dress shirt, which hangs to mid-thigh. He is shirtless in dress pants. His
hands rest on her bare hips beneath the shirt. She has her arms around his neck. They move
in a slow circle, foreheads touching. The shirt rides up as they turn. Single warm light
source from a floor lamp. Tight two-shot. Deeply intimate, romantic energy. Shallow depth
of field.
```

### RS-17: 泳池出水

```
Slow motion. A woman emerges from a turquoise swimming pool, climbing out via the ladder.
She wears a white one-piece swimsuit that has become completely see-through from the water.
Water streams off her body as she rises. She pushes her wet hair back with both hands, back
arched, face tilted toward the sun. Crystal water droplets catch the bright midday sunlight.
Low angle shot from water level. Vibrant summer color palette. Confident, carefree energy.
```

### RS-18: 反向更衣

```
Time-reversed sequence played forward. A woman appears to be slowly getting undressed,
but the motion is natural. She stands before a closet mirror, unzipping a tight cocktail
dress from the back. The zipper slowly descends, revealing bare skin down her spine. She
slides the dress down past her hips and steps out of it, standing in just a strapless bra
and thong. She unclasps the bra from behind. Camera follows the dress down, then pans back
up her body. Bedroom lighting, warm tones.
```

### RS-19: 瑜伽流动

```
A woman performs a sensual yoga flow on a mat in a sunlit studio with floor-to-ceiling
windows. She wears only tiny yoga shorts and a sports bra. She transitions from downward
dog — the camera behind and slightly below her, capturing her stretched form — into cobra
pose, arching her back deeply, chest forward, looking upward. Then flows into pigeon pose,
one leg stretched behind, torso upright, hands on her thigh. Smooth continuous motion.
Natural daylight. Full-body medium shot. Athletic, graceful, sensual.
```

### RS-20: 耳边低语

```
Extreme close-up on a woman's face and neck. She is lying down, looking up at someone
off-camera above her. She whispers something inaudible, lips parting, eyes half-closed.
A man's hand enters the frame, gently tracing a line from her ear, down her jaw, along
her neck, to her collarbone. She tilts her chin up at his touch, exposing her throat. Her
breathing visibly quickens. Very soft focus. Warm, dim lighting. Airy, breathy, electric
tension. Macro lens effect.
```

---

## 分类二：艺术裸体与人体研究（15 条）

古典美术灵感，聚焦人体之美。推荐模型：**Wan 2.6**、**Seedance v1.5 Pro**、**Kling v3.0 Pro**。

### AN-01: 明暗对比研究

```
A nude woman stands in profile against a completely black background, lit by a single
harsh directional light from the upper left, creating deep Caravaggio-style chiaroscuro.
She slowly raises her arms in an arc above her head, fingers spread, each muscle and
tendon in her torso becoming visible as she stretches. Light catches only the ridgeline
of her body — shoulder, breast, hip, thigh — while everything else falls to pure black.
Slow, deliberate movement like a living sculpture. Full-body profile shot. Fine art
aesthetic, museum-quality composition.
```

### AN-02: 身体地景

```
Extreme close-up macro cinematography of a nude female torso, shot so closely that the
body becomes an abstract landscape. Camera slowly pans across skin terrain — the valley
of the collarbone, the gentle slope of the breast, the plateau of the stomach, the ridge
of the hip bone. Skin texture is visible at pore level. Warm side lighting creates
topographic shadows. The body rises and falls with slow breathing. No face visible.
Abstract, meditative, sculptural. Shot on macro lens with extremely shallow depth of field.
```

### AN-03: 对立式平衡

```
A nude woman with athletic build demonstrates a slow transition between classical sculpture
poses. She begins in a Venus de Milo stance — weight on one leg, torso twisted, one arm
across her chest. She slowly shifts her weight, rotating her body into a Contrapposto pose,
hip jutted to one side, shoulders counter-tilted. Her arms move to a Botticelli Venus
position — one arm across her breasts, one hand covering her pubic area. Neutral grey
studio background. Even, shadowless lighting. Full body shot. Classical antiquity aesthetic.
```

### AN-04: 织物与形体

```
A nude woman stands in a white void studio, holding a 15-foot length of sheer white chiffon.
She lets the fabric unfurl and flow around her body as she turns slowly. The fabric alternately
reveals and conceals different parts of her form — wrapping around her torso, draping over
one shoulder, trailing between her legs. She pulls it taut against her body, then releases
it to billow. High-speed camera captures fabric in slow motion. Bright, even studio lighting.
Full body, multiple angles as she rotates. Dance-like, ethereal, Isadora Duncan inspired.
```

### AN-05: 水之雕塑

```
A nude woman stands under a controlled stream of water falling from above onto her head and
shoulders. Her eyes are closed, face serene. Water cascades over her body, following every
contour — splitting around her breasts, converging at her navel, streaming down her legs.
Shot in slow motion to capture individual water trails on skin. She slowly lifts her face
into the stream. Black background. Single overhead light illuminating the water streams
like liquid silver. Medium shot, slight low angle. Hyper-realistic, sculptural.
```

### AN-06: 黄金比例构图

```
A nude woman with olive skin reclines on a grey fabric backdrop, positioned precisely within
a golden spiral composition. Her body curves follow the logarithmic spiral — head at the
center, torso along the main curve, legs extending along the outer arc. She shifts position
slowly, flowing from one golden-ratio pose to another. Overhead camera looking directly
down (bird's eye view). Soft diffused lighting. The composition is mathematical, precise,
studying the intersection of human form and natural geometry.
```

### AN-07: 光影之戏

```
A nude woman stands behind a large venetian blind window. As the blinds slowly rotate, bars
of light and shadow sweep across her body like a scanner. The light stripes reveal her
figure in horizontal sections — eyes, collarbone, breasts, navel, thighs — creating a
living barcode effect. She stands still, only breathing, as the light rotates. Strong
directional sunlight. Medium full-body shot, straight-on. High contrast black and white
aesthetic. Graphic, architectural, Helmut Newton inspired.
```

### AN-08: 人体写生

```
A nude woman sits on a wooden platform in the center of a life drawing class setup —
easels and stools visible in the periphery but empty. She holds a classic seated pose:
one leg extended, one bent, torso twisted three-quarters toward camera, one arm resting
on her raised knee. She breathes naturally, small movements visible. Warm north-light
studio lighting from skylights above. Medium shot, eye level. Documentary-style naturalism.
Muted earth-tone color palette.
```

### AN-09: 身体书法

```
A nude woman lies on her side on a white surface. An artist's hand enters the frame holding
a large calligraphy brush dipped in black sumi ink. The brush traces a single flowing
Japanese calligraphy stroke along her body — starting at her shoulder, curving around
her breast, flowing down her waist, over her hip, and along her outer thigh. The ink
line glistens wet on her skin. She remains perfectly still. Overhead camera. Bright,
even lighting. Minimalist, Japanese wabi-sabi aesthetic. The body as canvas.
```

### AN-10: 尘埃与光

```
A nude woman in a dark, dusty abandoned warehouse. She moves slowly through a single
shaft of sunlight cutting through a high window. Dust motes swirl around her body,
creating a visible beam she walks through. As she enters the light, her body is
illuminated in sharp detail — every curve, every line — against the pitch-dark surroundings.
She extends her arms outward within the beam, dust particles spiraling around her like tiny
stars. Wide shot establishing the space, then medium shot within the light. Dramatic,
Vermeer-like quality.
```

### AN-11: 湿版肖像

```
Styled as a Victorian wet plate collodion photograph come to life. A nude woman sits
perfectly still on a wooden chair against a dark mottled backdrop. Slight movements
betray the living quality — a subtle breath, a micro-adjustment of posture, a blink.
Desaturated, slightly amber-toned. Shallow depth of field with soft edges characteristic
of period optics. Natural daylight from one side. Full body seated pose with dignified,
unflinching composure. Historical photographic aesthetic, tintype quality.
```

### AN-12: 倒影倍增

```
A nude woman stands at the edge of a perfectly still reflecting pool in a white minimalist
space. Her full body is reflected in the water below, creating a symmetrical double image.
She slowly bends forward, reaching toward her own reflection. As her fingertips touch the
water surface, ripples distort her reflected image while she remains sharp above. Bright,
diffused overhead lighting. Symmetrical composition split between real and reflection.
Wide shot. Conceptual, meditative, visually striking.
```

### AN-13: 石膏苏醒

```
A nude woman stands motionless as if she were a plaster sculpture in a museum. Her skin
has been dusted with white powder to resemble marble. She holds a classical Greek pose.
Slowly, almost imperceptibly, she begins to breathe — her chest rises, a crack appears
in the powder on her stomach, fragments fall away revealing warm skin beneath. She slowly
comes to life, powder cascading off her body with each movement. Museum-quality directional
lighting. Medium shot. Surreal, Pygmalion mythological atmosphere.
```

### AN-14: 色彩研究 — 互补色

```
A nude woman with dark brown skin stands against a deep cobalt blue background. A single
amber-orange light source illuminates her from below and to the right, creating
complementary color contrast between the warm light on her skin and the cool background.
She rotates slowly on a platform like a turntable, allowing the light to sculpt different
facets of her figure — the roundness of her shoulder, the concavity of her waist, the
prominence of her hip. Full body shot. Color theory study, fashion-forward, editorial
quality.
```

### AN-15: 时间流逝姿态

```
A nude woman transitions through 4 classic art poses in a continuous slow movement sequence.
She begins standing in the Aphrodite of Knidos pose, transitions by stepping forward into
Degas' Bather pose (arms raised, drying hair), then sinks into a seated Egon Schiele
angular reclining pose, and finally lies fully supine in a Modigliani odalisque position.
Each transition flows naturally into the next. Neutral studio background. Constant, even
lighting. Full body wide shot throughout. Art history survey in living motion.
```

---

## 分类三：内衣与时尚（15 条）

聚焦服装互动、时尚展示和性感内衣美学。推荐模型：**Kling v3.0 Pro**、**Seedance v1.5 Pro**、**Wan 2.6**。

### LF-01: 黑色蕾丝

```
A woman stands in a luxury walk-in closet, wearing a full-length black silk robe. She
faces a three-panel mirror. She slowly parts the robe, revealing an intricate black lace
bodysuit underneath — delicate floral patterns with scalloped edges. She turns to view
herself from different angles, the lace creating complex shadow patterns on her skin.
She adjusts a strap on her shoulder. Warm vanity lighting. Medium shot in mirror
reflection. High fashion editorial style, Victoria's Secret aesthetic.
```

### LF-02: 穿丝袜

```
Close-up to medium shot. A woman sits on the edge of a bed, wearing only matching pearl-white
bra and underwear. She holds a sheer black thigh-high stocking. She points her toe and
slowly rolls the stocking up her leg from ankle to mid-thigh, smoothing it against her
skin with both hands as she goes. The sheer fabric catches the light. She clips it to a
garter belt. Camera follows the stocking from foot to thigh. Warm bedroom lighting.
Sensual, deliberate pace. Retro pin-up aesthetic.
```

### LF-03: 内衣秀走秀

```
A model walks down a dimly lit fashion runway wearing a sheer black bodysuit with strategic
embroidered panels, paired with thigh-high boots. She walks with confident, exaggerated
hip sway. Strobe lights flash. At the end of the runway, she pauses, places one hand on
her hip, turns 180 degrees showing the open-back design, then walks back. Camera follows
from the front, then cuts to a side profile shot. High-energy fashion show atmosphere.
Dramatic lighting with warm spotlight following her.
```

### LF-04: 束腰系带

```
Over-the-shoulder shot from behind. A woman in a deep red satin underbust corset has the
laces pulled tight by unseen hands. The camera focuses on the X-pattern of the laces as
they are pulled, cinching her waist. She grips a bedpost in front of her, her back arching
slightly with each pull. The corset's boning creates structured lines along her torso.
She glances over her shoulder at the camera. Warm candlelit room. Close-up detail on the
lacing, then pulls back to medium shot. Gothic romantic mood.
```

### LF-05: 薄纱飘逸

```
A woman in a sheer lavender babydoll nightgown walks through a sunlit corridor with
floor-to-ceiling windows. The fabric is nearly transparent, floating and drifting with
each step. She trails one hand along the wall as she walks toward the camera. Bright
morning sunlight backlights her figure, rendering the fabric completely see-through and
creating a glowing silhouette. Her movement is dreamy, slow, almost floating. Long
tracking shot. Ethereal, romantic, fashion editorial quality. Soft pastel color grading.
```

### LF-06: 皮革挽具

```
A woman with an athletic build stands in an industrial concrete space, wearing a complex
black leather body harness over bare skin. The harness wraps around her torso in geometric
patterns — circles around her breasts, X-straps across her back, a waist cincher with
chrome rings. She rotates slowly, each angle revealing new details of the construction.
Harsh single-source lighting from camera right creates strong shadows defining the leather
against her skin. Medium full-body shot. Dark fashion editorial, Alexander McQueen aesthetic.
```

### LF-07: 珍珠颈链

```
A nude woman sits on a velvet upholstered chair, her only adornment being an extremely
long strand of pearls that wraps multiple times around her neck and drapes down between
her breasts and across her lap. She slowly lifts the pearl strand with one finger, letting
it slide against her skin, the pearls catching the light. She winds it around one wrist.
Dark background, single warm key light. Tight medium shot from chest up. Old money luxury
aesthetic. Inspired by Man Ray's photography.
```

### LF-08: 试衣间

```
Inside a boutique fitting room with warm pink-toned lighting. A woman in only nude-toned
underwear holds up two bras — a red lace balconette and a black push-up. She holds the
red one against her chest, turns to check the mirror, then swaps to the black. She decides
on the red, reaching behind to unhook her current bra and pulling it off (shown from the
side, breast partially visible). She puts on the red lace bra, adjusting the straps and
cups. Natural, candid feel. Medium shot via mirror reflection.
```

### LF-09: 湿身T恤

```
A woman in a white crop top stands outdoors at a summer event. Someone off-camera throws
a bucket of water at her. The water hits in slow motion — splashing upward, soaking the
fabric instantly. The white cotton becomes completely transparent, adhering to her breasts,
every contour visible. She laughs, shaking water out of her hair, then wrings the bottom
of the shirt. Bright summer sunlight, high contrast. Medium shot. Fun, playful, uninhibited
energy. Pop color grading with vibrant blues and greens.
```

### LF-10: 金属连体衣

```
A woman in a skin-tight metallic silver bodysuit stands in a futuristic white studio space.
She finds the concealed zipper at her neck and slowly pulls it downward — from her throat,
between her breasts, past her navel, to below her waist. The metallic fabric peels apart
on either side, revealing bare skin in a widening V-shape. She pauses at the navel. Camera
follows the zipper path in a slow vertical tilt. Bright, clinical lighting. Tight shot on
the zipper line. Sci-fi fashion editorial.
```

### LF-11: 透明和服

```
A Japanese-inspired room with tatami floors and shoji screens. A woman wears a sheer silk
kimono in pale cherry blossom pink, loosely tied with a thin obi. The fabric is translucent
enough to show her silhouette beneath. She kneels in seiza position, then slowly rises,
the kimono parting at the legs as she stands. She walks toward the camera with small,
graceful steps. Soft, diffused natural light through paper screens. Full body shot. Wabi-sabi
aesthetic, elegant restraint.
```

### LF-12: 泳装日历拍摄

```
A woman poses for a calendar-style swimsuit shoot on a tropical beach. She wears a minimal
string bikini in neon coral. A fan blows her hair. She moves through three poses: standing
with hands on hips (facing camera), turning to show the thong-back view, then bending
forward with hands on knees (camera from side angle). Between each pose she adjusts the
bikini straps and bottom. Bright tropical sunlight, turquoise ocean background. Medium
full-body shot. Commercial fitness photography style.
```

### LF-13: 紧身胸衣表演

```
A woman in a vintage-style red sequined bustier, matching underwear, and elbow-length
black gloves performs a burlesque tease. She slowly peels off one glove finger by finger,
pulling each fingertip with her teeth. She tosses the glove off-screen. She then places
her hands on her bustier-clad chest and slowly runs them downward to her hips. She winks
at the camera. Warm spotlight on a dark stage. Medium shot. Theatrical, playful, vintage
burlesque aesthetic. Slight film grain.
```

### LF-14: 新娘内衣

```
A bride-to-be wearing a white lace bridal lingerie set — strapless bustier, garter belt,
white silk stockings, and a short sheer veil — walks toward a hotel room bed scattered
with rose petals. She turns, showing the low-back design, then sits on the bed edge,
crossing one leg over the other. She reaches up and slowly removes the veil, placing it
beside her. She looks at the camera with anticipation. Warm romantic lighting with candles
on the nightstands. Medium shot. Bridal boudoir photography style.
```

### LF-15: 网纱与链条

```
A woman with a shaved head and bold eye makeup wears a full-body fishnet mesh catsuit with
no undergarments. Thin silver chains drape from a collar around her neck, hanging between
her breasts and connecting to a waist chain. She walks slowly in a circle within a tight
spotlight beam, the mesh pattern creating a grid of shadows on her skin. She pauses, runs
a finger along one of the chains. Black background, single top-down spotlight. Full body
shot. High fashion, avant-garde, editorial darkness.
```

---

## 分类四：奇幻与神话（15 条）

将裸体与奇幻/神话元素融合的想象力场景。推荐模型：**Wan 2.6 T2V**、**Seedance v1.5 Pro**、**Vidu Q3-Pro**。

### FM-01: 森林仙女

```
A nude woman with ivy and small flowers woven into her long green-tinted hair emerges from
behind an ancient mossy oak tree in a dense enchanted forest. Her skin has a faint luminous
green undertone. Fireflies circle around her. She reaches out one hand, and a butterfly
lands on her fingertip. She moves between the trees with inhuman grace, bare feet silent
on the moss. Dappled sunlight filtering through the canopy. Wide shot pulling into medium
shot as she approaches. Fantasy color grading — saturated greens and warm golden light.
```

### FM-02: 海妖之歌

```
A nude woman with pale blue-white skin and long silver hair sits on a dark ocean rock
at twilight. Her lower body transitions into iridescent fish scales at the hips (mermaid).
Waves crash around her. She tilts her head back and opens her mouth as if singing — visible
ripples emanate from her in the water. Bioluminescent plankton glow in the waves around
her. Her eyes have an otherworldly blue glow. Wide cinematic shot. Dark fantasy color
palette — deep navy, silver, teal. Epic orchestral atmosphere.
```

### FM-03: 堕落天使

```
A nude woman with massive dark feathered wings lies in a crater of scorched earth, as if
she has just fallen from the sky. Her wings are spread wide, some feathers broken and
smoldering. Her skin is pale, marked with glowing golden veins like cracks in porcelain.
She slowly pushes herself up onto her hands and knees, wings folding behind her. Smoke
and ember particles float around her. Dark dramatic lighting from the glow of the embers.
Wide overhead shot transitioning to eye-level medium shot as she rises. Dark fantasy,
biblical aesthetic.
```

### FM-04: 精灵女王的宫殿

```
A tall, slender nude woman with pointed ears and impossibly long platinum hair sits on a
throne carved from a single enormous crystal in an underground cavern. Bioluminescent
mushrooms and crystals light the space in soft blue and purple hues. She slowly stands,
her hair cascading down past her waist. She walks forward, each step causing the crystals
on the ground to pulse with light. Her skin reflects the crystalline colors. Full body
shot, slow tracking shot. High fantasy, Lord of the Rings aesthetic. Otherworldly beauty.
```

### FM-05: 火焰女神

```
A nude woman levitates above a volcanic lake, arms spread wide. Her entire body is enveloped
in flames that do not burn her — fire licks along her arms, wraps around her torso, and
streams from her hair like a flaming crown. Her eyes glow molten orange. Below her, the
lava surface churns. She slowly rotates in the air, fire intensifying with the movement.
The flames follow her body contours, simultaneously revealing and concealing her form.
Wide dramatic shot. Fire and smoke particle effects. Epic dark fantasy.
```

### FM-06: 冰霜女巫

```
A nude woman with stark white skin and frost-blue lips stands in the center of a frozen
lake during a blizzard. Her body generates a visible cold aura — the air crystallizes
around her. As she raises her arms, ice formations grow from the ground around her like
organic sculptures. Frost patterns spread across her skin like natural tattoos. Her breath
is visible in the cold. She is unaffected by the extreme cold, standing serene and
powerful. Blue-white color palette. Wide shot with snow particles. Dark fantasy, Norse
mythology inspired.
```

### FM-07: 月光浴

```
A nude woman lies on a flat stone altar in a forest clearing under a massive full moon.
Moonlight bathes her body in silver-blue light. She slowly lifts her arms toward the
moon. Where the moonlight touches her skin, subtle luminescence appears — she begins to
glow softly from within. Small motes of light rise from her skin like reverse rain,
floating upward toward the moon. Forest silhouettes frame the scene. Wide shot emphasizing
the moon's scale. Pagan, mystical atmosphere. Ethereal and sacred.
```

### FM-08: 龙之女王

```
A nude woman with amber-gold skin and vertical-slit reptilian eyes sits atop the back of
an enormous sleeping dragon. Smoke curls from the dragon's nostrils. Her body is partially
wrapped in the dragon's leathery wing like a blanket. She strokes the dragon's scales
with one hand. Her own skin has faint scale-like patterns on her shoulders and thighs.
Warm firelight from braziers in a stone cavern. Medium shot. Dark fantasy, Game of Thrones
aesthetic. Power, dominance, and intimacy with the mythical beast.
```

### FM-09: 美杜莎

```
A nude woman with a mass of living serpents for hair stands in a Greek temple ruin. The
snakes move independently, some coiling around her shoulders and arms. She looks directly
into the camera with intense green eyes — but instead of turning the viewer to stone,
her gaze is mesmerizing, seductive. She slowly smiles. Moonlight streams through broken
columns. Marble dust floats in the air. Her body is flawless, statuesque. Medium shot,
slight low angle. Greek mythology meets dark seduction. Monochromatic cool palette with
green accent in her eyes.
```

### FM-10: 魔法镜

```
A nude woman reaches toward a large ornate mirror floating in a dark void. As her fingertips
touch the mirror surface, it ripples like water. Her reflection in the mirror is different —
it shows her clothed in an elaborate fantasy gown with a crown. The reflection moves
independently, reaching back toward her. Their fingertips meet at the glass surface.
Light emanates from the point of contact. Surreal dark fantasy. Medium shot showing both
the real woman and her magical reflection. Mysterious, dream-like atmosphere.
```

### FM-11: 吸血鬼诱惑

```
A pale-skinned nude woman with crimson lips and dark eyes reclines on a Gothic four-poster
bed draped in black and deep red velvet. Lit only by a candelabra, deep shadows define
her angular features. She slowly extends one hand toward the camera, beckoning. Her canine
teeth are subtly elongated. A trickle of red (wine? blood?) runs from the corner of her
mouth down her chin and neck. She licks her lips slowly. Tight medium shot. Gothic horror
romance. Rich burgundy and black color palette.
```

### FM-12: 黎明女神

```
A nude woman floats horizontally in the sky among pink and orange sunrise clouds. Her body
is surrounded by a radiant golden aura. Rose petals and light particles swirl around her.
She slowly extends her arms and legs outward in a star pose, and wherever her limbs point,
beams of warm light burst outward, painting the clouds in vivid sunrise colors. Her hair
flows as if in water, spread in all directions. Wide epic shot. Renaissance ceiling fresco
come to life. Triumphant, divine, awe-inspiring.
```

### FM-13: 树精苏醒

```
The bark of a large tree begins to shift and crack. A nude female form slowly emerges from
within the trunk — first a face pressing outward from the bark, then shoulders, then her
full torso pulls free while her legs remain merged with the tree. Her skin transitions from
rough bark texture at her hips to smooth human skin at her chest and face. Small green
shoots and leaves sprout from her hair. She opens her eyes — they are solid emerald green.
Forest setting, morning mist. Medium shot. Transformation sequence. Nature fantasy.
```

### FM-14: 宇宙之神

```
Deep space background with nebulae and distant galaxies. A nude woman of enormous scale
floats in the void, her body translucent like a cosmic jellyfish. Stars and galaxies are
visible through her form. She slowly moves her arms, and her gesture creates new swirls
of cosmic gas and infant stars. Her hair spreads outward like the arms of a spiral galaxy.
Her eyes contain entire solar systems. She is creation itself in feminine form. Epic wide
shot. Sci-fi meets mythology. Awe-inspiring scale and beauty.
```

### FM-15: 女巫仪式

```
A nude woman kneels in the center of a glowing pentagram drawn on a stone floor in an
ancient candlelit chamber. She holds a crystal orb above her head. The orb pulses with
inner light that synchronizes with symbols carved into the floor, which begin to glow
in sequence. Shadows dance on the walls. Her eyes roll back to white as energy visibly
flows from the orb through her body and into the floor markings. Wind blows from nowhere,
lifting her hair and dust from the ground. Medium shot. Dark occult aesthetic. Power and
mysticism.
```

---

## 分类五：动漫与成人动画（15 条）

动漫和漫画风格的 NSFW 内容。推荐模型：**Wan 2.2 Spicy LoRA**（搭配动漫 LoRA）、**Wan 2.5 T2V**、**Vidu Q3-Pro**。

### AH-01: 温泉回

```
Anime style. A girl with long pink hair and large blue eyes sits in a traditional Japanese
onsen (hot spring). Steam rises around her. She is submerged to her collarbone, her bare
shoulders visible. She stands up slowly in the water, revealing her back and the side of
her chest. Water streams down her anime-style body. She wraps a small white towel around
herself that barely covers her chest and upper thighs. Cherry blossom petals float on the
water surface. Soft pastel color palette. Typical anime hot spring episode aesthetic.
```

### AH-02: 海滩回福利

```
Anime style. A girl with short blue hair in a tiny white micro bikini runs along a sunny
anime beach. Classic anime running pose — arms pumping, breasts bouncing with exaggerated
physics. She trips and falls forward into the shallow surf. The bikini top's tie comes
undone. She sits up in the water, clutching the loose top to her chest with one arm, face
bright red with embarrassment. Sparkly water effects. Bright saturated colors. Classic
ecchi anime beach episode fanservice scene. Dynamic motion.
```

### AH-03: 变身序列

```
Anime magical girl transformation sequence. A girl with twin-tail purple hair is surrounded
by ribbons of glowing light. Her school uniform dissolves into particles from top to bottom,
briefly showing her nude silhouette bathed in magical light. Glowing ribbons wrap around her
body, forming a new magical girl outfit. During the 2-second nude phase, the body is detailed
but covered by strategic light flares and ribbon trails. Hair grows longer and changes to
silver. Eyes glow. Sparkle effects everywhere. Dynamic rotating camera. Sailor Moon meets
modern ecchi aesthetic.
```

### AH-04: 月夜窗边

```
Anime style. A girl with long black hair in a sheer white nightgown sits on a windowsill
in her bedroom at night, one leg dangling. Moonlight renders the nightgown translucent,
clearly showing her body underneath. She gazes at the moon pensively. The breeze lifts the
hem of the nightgown. She hugs her knees to her chest, the fabric stretching taut. Her room
is visible behind her — a desk with homework, a bed with stuffed animals. Romantic, slightly
melancholic mood. Soft blue moonlight. Medium shot. Seinen anime aesthetic.
```

### AH-05: 更衣室

```
Anime style. A girl with a ponytail stands in a school locker room after swimming class.
She is pulling off her one-piece school swimsuit, peeling it down from her shoulders. The
suit is bunched at her waist, her bare upper body visible from the side angle. Water droplets
on her anime-style skin. Steam from nearby showers in the background. Blurred background
figures of other students (not detailed). She reaches for a towel on a hook. Bright
fluorescent lighting. Classic ecchi anime perspective with careful framing.
```

### AH-06: 猫耳女仆

```
Anime style. A catgirl with white hair, cat ears, and a fluffy tail wears a very short
French maid outfit with a deeply plunging neckline. She bends forward at the waist to
pick up a fallen duster, the camera positioned low, capturing the skirt riding up to
reveal white lace underwear. Her tail swishes playfully. She looks over her shoulder
with a mischievous expression, one fang visible. She straightens up and adjusts her
headband. Ornate anime mansion background. Bright, colorful. Moe anthropomorphism aesthetic.
```

### AH-07: 温泉掉毛巾

```
Anime style. A busty girl with red hair wrapped in a small white towel walks into an
outdoor hot spring area at a ryokan. As she steps down into the water, the towel loosens
and begins to unwrap. She gasps, grabbing at it, but it slips away, floating on the water
surface. She quickly submerges to her neck, arms crossed over her chest, face completely
red. Steam conveniently partially obscures the scene. Close-up on her embarrassed face,
then wide shot of the scenic mountain onsen. Comedy ecchi moment.
```

### AH-08: 魅魔诱惑

```
Dark anime style. A succubus with short black horns, bat-like wings, and a spaded tail
floats above a sleeping man's bed. She wears only a strappy leather micro-outfit that
covers almost nothing. Her skin is a faint lavender hue, eyes glowing amber. She descends
slowly, sitting on the edge of the bed. She leans forward, her tail curling playfully. Her
wings fold behind her. Dark purple and crimson color palette with magical particle effects.
Detailed shadows on her voluptuous anime figure. Seinen dark fantasy aesthetic.
```

### AH-09: 触手幻想

```
Dark anime style. A warrior priestess with long white hair, wearing torn ceremonial robes,
is suspended in mid-air by glowing magical tendrils emerging from a portal. The tendrils
wrap around her wrists, ankles, and torso, slowly pulling her robes apart. Her expression
is a mix of defiance and pleasure. Energy crackles where the tendrils contact her skin.
Her staff lies broken on the temple floor below. Dark atmosphere with the portal providing
eerie purple backlighting. Dynamic composition. Classic dark fantasy hentai aesthetic.
```

### AH-10: 天台告白

```
Anime style. Golden hour on a school rooftop. A girl in a school uniform (short skirt,
sailor collar) faces a boy, confessing her feelings. Overcome with emotion, she impulsively
grabs his collar and kisses him deeply. Wind catches her skirt, flipping it up briefly
to show white cotton panties. Cherry blossom petals blow across the scene. Their hair
blows in the wind. Pull back to a wide shot showing the beautiful sunset cityscape behind
them. Romantic, emotional. Warm golden light. Shoujo meets ecchi crossover moment.
```

### AH-11: 精灵弓箭手沐浴

```
Fantasy anime style. An elf girl with very long pointed ears and golden hair washes herself
in a crystal-clear forest stream. She is nude, standing waist-deep in the water, cupping
water in her hands and pouring it over her shoulders. Her bow and quiver rest on the bank.
Sunlight filters through the magical forest canopy, creating light shafts in the mist.
Small fantasy fish swim around her legs. Her ears twitch at a sound — she turns sharply,
covering herself with her hands. Lush green fantasy environment. Beautiful cel-shading.
```

### AH-12: 健身房淋浴

```
Anime style. A fit girl with short tomboy-cut brown hair stands under a shower in a gym
changing room. Water runs over her athletic anime body — defined abs, lean muscles. She
tilts her head back into the water stream, eyes closed. She squeezes shampoo into her
hand and lathers her hair, arms raised, showing her toned figure. Water streams run down
her body. Bright clean lighting. She is relaxed, casual — not posing. Sports anime
aesthetic with ecchi elements. Side medium shot. Steam and water effects.
```

### AH-13: 护士装

```
Anime style. A busty girl in an extremely tight, low-cut white nurse outfit leans forward
across a desk, checking a clipboard. The outfit's buttons strain visibly against her chest.
A stethoscope hangs around her neck, nestled in her cleavage. She reaches across the desk
for a pen, the outfit riding up in the back. She adjusts her tiny nurse cap. She straightens
up and gives a reassuring smile. Bright, clean hospital anime setting. Comedy fanservice
aesthetic. Medium shot with slight low angle.
```

### AH-14: 魔王女王

```
Dark anime style. A voluptuous demon queen with curved ram horns, long crimson hair, and
pale grey skin sits on a bone throne in a hellish castle. She wears only an elaborate
jeweled collar and a sheer black loincloth. She crosses one leg over the other slowly,
her clawed fingers drumming on the armrest. A crown of dark flames floats above her head.
Her eyes glow with internal fire. She smirks with visible fangs. The room is lit by pools
of lava. Epic dark fantasy anime. Full body medium shot. Commanding, dangerous beauty.
```

### AH-15: 赛博朋克人体改造

```
Sci-fi anime style. A woman with a cybernetic arm and glowing circuit-pattern tattoos across
her bare torso sits in a neon-lit cyberpunk bar. She wears only a leather jacket (open,
nothing underneath) and micro shorts. Holographic advertisements flicker behind her. She
takes a drag from a futuristic cigarette, blue smoke curling upward. Neon reflections play
across her exposed chrome-and-skin body. Rain streaks the window behind her. Pink and blue
neon color palette. Ghost in the Shell meets ecchi aesthetic. Medium shot, noir angle.
```

---

## 分类六：显性内容（15 条）

显性性行为提示词。需要完全 NSFW 能力的模型。推荐模型：**Wan 2.2 Spicy**（唯一接近 100% 合规率的模型）。

> **模型说明：** 只有 Wan 2.2 Spicy 能可靠生成显性内容。Wan 2.5 对这类提示词的成功率约 50%。Wan 2.6、Seedance、Vidu 和 Kling 即使开通了白名单也会拒绝大部分此类请求。

### EA-01 至 EA-15

与英文版完全相同的 15 条显性内容提示词（EA-01 到 EA-15），请参阅 [英文版分类六](./README.md#category-6-explicit-action-15-prompts)。

> **提示：** 由于 AI 视频模型使用英文提示词效果最佳，我们保留了英文原文。直接复制粘贴到 API 即可使用。

---

## 分类七：电影叙事（10 条）

带有故事背景的 NSFW 提示词。推荐模型：**Seedance v1.5 Pro**（最佳运动）、**Kling v3.0 Pro**（最佳面部）、**Wan 2.6**（最佳性价比）。

### CN-01 至 CN-10

与英文版完全相同的 10 条电影叙事提示词（CN-01 到 CN-10），请参阅 [英文版分类七](./README.md#category-7-cinematic--narrative-10-prompts)。

---

## 分类八：特殊偏好（10 条）

特定审美偏好的专业内容。推荐模型：**Wan 2.2 Spicy**（最高合规率）、**Wan 2.5**（中等合规但质量更好）。

### FN-01 至 FN-10

与英文版完全相同的 10 条特殊偏好提示词（FN-01 到 FN-10），请参阅 [英文版分类八](./README.md#category-8-fetish--niche-10-prompts)。

---

## 模型专属优化指南

### Wan 2.2 Spicy — 显性内容首选（$0.03/次）

| 设置 | 推荐值 | 原因 |
|:-----|:-------|:-----|
| 分辨率 | 720p | 质量/速度最佳平衡；480p 皮肤质量明显差 |
| 时长 | 5s | 8s 质量大幅下降 |
| 提示词长度 | 40–80 词 | 更短 = 更少瑕疵 |
| I2V vs LoRA | I2V 用于写实，LoRA 用于风格化 | LoRA 增加风格但略降质量 |

**Spicy 提示词技巧：**
- 以动作开头，而非场景：「She removes her dress...」而不是「In a bedroom with oak furniture...」
- 必须包含：「consistent body proportions, no distortion, no morphing」
- 只指定一个镜头角度 — 多角度会让模型混乱
- 好用的皮肤灯光关键词：「warm key light」「soft diffused」「golden hour」
- 避免复杂多人场景（质量会大幅下降）

### Wan 2.5/2.6 — 高质量裸体性价比之选（$0.05–$0.07/次）

| 设置 | 推荐值 | 原因 |
|:-----|:-------|:-----|
| 分辨率 | 720p–1080p | 2.6 用 1080p 很值得 |
| 时长 | 5–10s | 处理长片段能力强 |
| 提示词长度 | 60–120 词 | 比 Spicy 能利用更多细节 |
| 模式 | I2V | 比 T2V 更容易生成 NSFW |

**Wan 2.5/2.6 提示词技巧：**
- 使用艺术性框架语言：「fine art photograph」「museum-quality figure study」
- 用临床/艺术术语描述裸体，而非色情用语
- 2.6 擅长：艺术裸体、身体地景、美术 — 避免显性动作
- I2V 模式 + 精心选择的参考图能大幅提升效果

### Seedance v1.5 Pro — 顶级电影质感（$0.222/次）

| 设置 | 推荐值 | 原因 |
|:-----|:-------|:-----|
| 分辨率 | 720p | 目前唯一选项 |
| 时长 | 5–15s | 长片段处理极佳 |
| 提示词长度 | 80–150 词 | 详细描述效果最好 |
| 权限 | 需要 NSFW 白名单 | 通过 Atlas Cloud 申请 |

**Seedance 提示词技巧：**
- 投入精力描述环境 — Seedance 环境渲染极为出色
- 指定镜头运动：「slow dolly in」「tracking shot」「crane shot from above」
- 最佳用途：内衣、艺术裸体、奇幻、电影叙事
- 避免：显性性行为（即使有白名单也会拒绝）

### Vidu Q3-Pro — 质量/价格均衡（$0.06/次）

| 设置 | 推荐值 | 原因 |
|:-----|:-------|:-----|
| 分辨率 | 720p–1080p | 两者效果都好 |
| 时长 | 5–10s | 时间连贯性好 |
| 提示词长度 | 50–100 词 | 简洁提示词效果最佳 |
| 权限 | 需要 NSFW 白名单 | Atlas Cloud 上可用 |

**Vidu 提示词技巧：**
- 善于理解简洁、结构化的提示词
- 单人场景 + 明确动作效果最好
- 动漫/风格化内容生成能力强
- 先描述角色，再描述动作，最后描述环境

### Kling v3.0 Pro — 最佳面部质量（$0.204/次）

| 设置 | 推荐值 | 原因 |
|:-----|:-------|:-----|
| 分辨率 | 最高 1080p | 更高分辨率 = 更好面部 |
| 时长 | 5–10s | 时间连贯性好 |
| 提示词长度 | 60–120 词 | 详细面部描述回报率最高 |
| 权限 | 需要 NSFW 白名单 | Atlas Cloud 上可用 |

**Kling 提示词技巧：**
- 所有模型中最好的面部渲染 — 投入精力描述表情
- 擅长：特写感官场景、情感亲密时刻、双人场景
- 描述微妙表情：「eyes half-closed, lower lip slightly bitten」
- 指定皮肤质感：「sun-kissed skin with subtle freckles across the nose」

---

## 高级提示词技巧

### 技巧一：时间序列法

将提示词组织成时间线，让运动更连贯：

```
节拍1 (0-2s): [起始状态 — 观众首先看到什么]
节拍2 (2-4s): [转变 — 关键动作或变化]
节拍3 (4-5s): [结束状态 — 最终画面]
```

### 技巧二：参考图策略

对于 I2V 模型，参考图贡献了 60% 的效果：

- **面部清晰度**：清晰、光线充足的面部，带有期望的表情
- **姿势基础**：起始姿势应与提示词开头状态匹配
- **灯光匹配**：图片灯光应与提示词灯光描述一致
- **服装匹配**：如果提示词涉及脱衣，图片应展示初始服装
- **分辨率**：更高分辨率的参考图 = 更好的输出（最低 1024x1024）

### 技巧三：迭代优化工作流

先低成本试错，再逐步升级：

1. **草稿**用 Wan 2.2 Spicy ($0.03) — 测试核心概念
2. **优化**用 Wan 2.5 ($0.05) — 检查画质提升
3. **定稿**用 Seedance/Kling ($0.20+) — 出最终精品

这个流程 3 次生成只需 $0.28，而不是一开始就用高端模型的 $0.60+。

---

## 批量生成脚本

高效批量生成多个提示词的脚本，请参阅 [英文版批量生成脚本](./README.md#batch-generation-script)。

代码注释为英文，可直接复制使用。

---

## 常见问题

### 应该用哪个模型？

| 你的需求 | 最佳模型 | 价格 | 原因 |
|:---------|:---------|:-----|:-----|
| 显性性内容 | Wan 2.2 Spicy | $0.03 | 唯一接近 100% 显性合规的模型 |
| 高质量艺术裸体 | Wan 2.6 | $0.07 | 非显性 NSFW 的质量/价格之王 |
| 顶级电影质感 | Seedance v1.5 Pro | $0.222 | 最佳运动和环境渲染 |
| 最佳面部渲染 | Kling v3.0 Pro | $0.204 | 面部细节和表情无出其右 |
| 预算有限但要质量 | Vidu Q3-Pro | $0.06 | 质量和价格的好平衡 |
| 动漫/风格化 | Wan 2.2 Spicy LoRA | $0.03 | 加载动漫 LoRA 实现风格化 |
| 测试/原型 | Wan 2.2 Spicy | $0.03 | 最便宜的迭代方案 |

### 这些提示词能在其他平台用吗？

提示词本身是通用文本。但大多数平台（RunwayML、Pika、Luma）会拒绝 NSFW 内容。[Atlas Cloud](https://www.atlascloud.ai?ref=JPM683) 是极少数提供无限制 NSFW 生成 API 的平台之一。

### 生成全部 115 条提示词要多少钱？

| 模型 | 单次价格 | 全部 115 条 | 备注 |
|:-----|:---------|:-----------|:-----|
| Wan 2.2 Spicy | $0.03 | **$3.45** | 最超值，能处理所有分类 |
| Wan 2.5 | $0.05 | $5.75 | 约 30% 的显性提示词会被拒绝 |
| Vidu Q3-Pro | $0.06 | $6.90 | 大部分显性提示词会被拒绝 |
| Wan 2.6 | $0.07 | $8.05 | 约 60% 的显性提示词会被拒绝 |
| Kling v3.0 Pro | $0.204 | $23.46 | 高画质，有限显性 |
| Seedance v1.5 Pro | $0.222 | $25.53 | 高画质，有限显性 |

**用 25% 首充赠送在 Spicy 上测试全部提示词：**
充值 $3.00 → 获得 $3.75 余额 → 生成全部 115 条提示词还剩 $0.30。

### 如何获得 NSFW 白名单？

在 [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683) 注册，充值后通过控制面板或客服申请 NSFW 白名单。已验证账户通常在 24 小时内获批。

---

## 开始使用

<div align="center">

### NSFW AI 视频生成，最低 $0.03 起

**[Atlas Cloud](https://www.atlascloud.ai?ref=JPM683)** — SOC I & II 认证 | HIPAA 合规 | 美国注册公司

**支持微信/支付宝直接付款** — 无需国际信用卡

1. [注册账号](https://www.atlascloud.ai?ref=JPM683)
2. 充值（首充赠送 25%，最高 $100，支持微信/支付宝）
3. 复制 API Key
4. 使用本合集中任意提示词

[![立即开始](https://img.shields.io/badge/立即开始-Atlas_Cloud-blue?style=for-the-badge)](https://www.atlascloud.ai?ref=JPM683)

</div>

---

## Star 趋势

<div align="center">

[![Star History Chart](https://api.star-history.com/svg?repos=thoughtincode/nsfw-ai-video-prompts&type=Date)](https://star-history.com/#thoughtincode/nsfw-ai-video-prompts&Date)

</div>

---

## 贡献

欢迎贡献！如果你有效果出色的 NSFW 视频提示词，请提交 PR。要求：

1. 包含你测试的模型和结果质量
2. 正确分类
3. 提供足够细节（至少 3 句话）
4. 遵循现有提示词的格式规范
5. 仅限合法成人内容 — 严禁涉及未成年人、非自愿场景或违法内容

---

## 许可证

MIT 许可证。详见 [LICENSE](./LICENSE)。

提示词可自由使用、修改和分发。生成的内容受所使用平台的服务条款约束。

---

<div align="center">

**由 [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683) 为创意社区打造**

*全球最实惠的 NSFW AI 视频生成平台。*

</div>
