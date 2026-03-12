<div align="center">

```
 _   _  ______        ______        ___    ___   __     __ _     _
| \ | |/ ___\ \      / /  __|      / _ \  |_ _|  \ \   / /(_) __| | ___  ___
|  \| |\___ \\ \ /\ / /| |_       / /_\ \  | |    \ \ / / | |/ _` |/ _ \/ _ \
| |\  | ___) |\ V  V / |  _|     / _____ \ | |     \ V /  | | (_| |  __/ (_) |
|_| \_||____/  \_/\_/  |_|      /_/     \_\|___|    \_/   |_|\__,_|\___|\___/

 프롬프트 라이브러리 — 100개 이상의 바로 사용 가능한 NSFW AI 비디오 프롬프트
```

# NSFW AI 비디오 프롬프트 라이브러리 — 100개 이상의 상세 프롬프트, 카테고리별 정리

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![프롬프트 수](https://img.shields.io/badge/프롬프트-100개_이상-blue)]()
[![지원 모델](https://img.shields.io/badge/지원_모델-5개_무검열-red)]()
[![최종 업데이트](https://img.shields.io/badge/업데이트-2026년_3월-green)]()
[![플랫폼](https://img.shields.io/badge/플랫폼-Atlas%20Cloud-purple)](https://www.atlascloud.ai?ref=JPM683)

**최대 규모의 오픈소스 NSFW AI 비디오 프롬프트 컬렉션. 모든 프롬프트 실제 테스트 완료, 카테고리별 정리, 각 모델별 최적화.**

**[English](./README.md)** | **[简体中文](./README_zh-CN.md)** | **[日本語](./README_ja.md)** | **[한국어](./README_ko.md)**

---

> **면책 조항:** 이 리포지토리는 합법적인 성인 콘텐츠 제작만을 목적으로 합니다. 모든 프롬프트는 성인(18세 이상)이 해당 콘텐츠가 합법인 지역에서 사용하도록 설계되었습니다. 미성년자, 비합의 시나리오 또는 기타 불법 콘텐츠와 관련된 어떠한 제작에도 엄격히 반대합니다. 사용자는 현지 법률 준수를 스스로 확인할 책임이 있습니다.

</div>

---

## 목차

- [지원 모델 및 가격](#지원-모델-및-가격)
- [가격 비교: Atlas Cloud vs fal.ai](#가격-비교-atlas-cloud-vs-falai)
- [빠른 시작 (API)](#빠른-시작-api)
- [프롬프트 엔지니어링 기초](#프롬프트-엔지니어링-기초)
- [카테고리 1: 로맨틱 & 센슈얼 (20개)](#카테고리-1-로맨틱--센슈얼-20개)
- [카테고리 2: 아티스틱 누드 & 인체 연구 (15개)](#카테고리-2-아티스틱-누드--인체-연구-15개)
- [카테고리 3: 란제리 & 패션 (15개)](#카테고리-3-란제리--패션-15개)
- [카테고리 4: 판타지 & 신화 (15개)](#카테고리-4-판타지--신화-15개)
- [카테고리 5: 애니메이션 & 헨타이 (15개)](#카테고리-5-애니메이션--헨타이-15개)
- [카테고리 6: 익스플리시트 액션 (15개)](#카테고리-6-익스플리시트-액션-15개)
- [카테고리 7: 시네마틱 & 내러티브 (10개)](#카테고리-7-시네마틱--내러티브-10개)
- [카테고리 8: 페티쉬 & 니치 (10개)](#카테고리-8-페티쉬--니치-10개)
- [모델별 최적화 가이드](#모델별-최적화-가이드)
- [고급 프롬프트 기법](#고급-프롬프트-기법)
- [배치 생성 스크립트](#배치-생성-스크립트)
- [자주 묻는 질문](#자주-묻는-질문)
- [시작하기](#시작하기)
- [Star 히스토리](#star-히스토리)
- [라이선스](#라이선스)

---

## 지원 모델 및 가격

아래 모델은 모두 [Atlas Cloud API](https://www.atlascloud.ai?ref=JPM683)를 통해 사용 가능하며, NSFW 콘텐츠 생성이 활성화되어 있습니다.

| 모델 | 타입 | 가격 | 해상도 | 길이 | NSFW 수준 | 최적 용도 |
|:-----|:-----|:-----|:-------|:-----|:----------|:---------|
| **Wan 2.2 Spicy** | I2V / I2V-LoRA | **$0.03**/초부터 | 480p, 720p | 5초, 8초 | 완전 무제한 | 저비용 익스플리시트 콘텐츠 |
| **Wan 2.5** | I2V / T2V | ~$0.05/초부터 | 720p, 1080p | 5초, 10초 | 누드 + 중간 수준 익스플리시트 | 중간 품질 |
| **Wan 2.6** | I2V / T2V | $0.07/초부터 | 최대 1080p | 5–15초 | 누드 (제한적 익스플리시트) | 고품질 아티스틱 누드 |
| **Seedance v1.5 Pro** | T2V / I2V | **$0.044**/초부터 | 720p | 5–15초 | 화이트리스트 NSFW | 프리미엄 시네마틱 품질 |
| **Vidu Q3-Pro** | T2V / I2V | **$0.06**/초부터 | 720p, 1080p | 5–10초 | 화이트리스트 NSFW | 품질/가격 균형 |
| **Kling v3.0 Pro** | T2V / I2V | **$0.204**/초부터 | 최대 1080p | 5–10초 | 화이트리스트 NSFW | 모션 품질, 얼굴 |

> **가격 안내:** 동영상 모델 가격은 생성된 동영상 1초당 가격입니다. 실제 비용은 선택한 해상도와 길이에 따라 달라집니다.
>
> **화이트리스트**는 Atlas Cloud에서 승인을 받은 후 NSFW 콘텐츠를 생성할 수 있음을 의미합니다. Vidu 시리즈도 화이트리스트 NSFW 콘텐츠 생성을 지원합니다.

### 신뢰 및 보안

- **SOC I & II 인증** — 엔터프라이즈급 보안 규정 준수
- **HIPAA 준수** — 의료 수준의 데이터 보호
- **미국 법인** — 미국 데이터 보호법 적용
- **첫 충전 시 25% 보너스** (최대 $100) — [지금 가입하기](https://www.atlascloud.ai?ref=JPM683)

---

## 가격 비교: Atlas Cloud vs fal.ai

fal.ai를 사용하고 계신다면, 다음은 초과 지불하고 있는 금액입니다:

### Wan 모델 (5초 동영상)

| 플랫폼 | 과금 방식 | 5초 동영상 비용 | 100개 비용 |
|:-------|:---------|:-------------|:----------|
| **Atlas Cloud** | 요청당 과금 | **$0.05** | **$5.00** |
| fal.ai | 초당 과금 ($0.05/초) | $0.25 | $25.00 |
| **절감** | | **80%** | **$20.00** |

### Kling 모델 (5초 동영상)

| 플랫폼 | 과금 방식 | 5초 동영상 비용 | 100개 비용 |
|:-------|:---------|:-------------|:----------|
| **Atlas Cloud** | 요청당 과금 | **$0.204** | **$20.40** |
| fal.ai | 초당 과금 ($0.224/초) | $1.12 | $112.00 |
| **절감** | | **82%** | **$91.60** |

### Wan 2.2 Spicy (Atlas Cloud 독점)

| 플랫폼 | 5초 동영상 비용 | 100개 비용 | 1,000개 비용 |
|:-------|:-------------|:----------|:------------|
| **Atlas Cloud** | **$0.03** | **$3.00** | **$30.00** |
| fal.ai | 제공하지 않음 | 제공하지 않음 | 제공하지 않음 |

> fal.ai는 무검열/NSFW 모델을 제공하지 않습니다. Atlas Cloud는 완전한 무제한 NSFW 비디오 생성 API를 제공하는 몇 안 되는 플랫폼 중 하나입니다.

---

## 빠른 시작 (API)

### 사전 요구사항

1. [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683)에서 계정 생성
2. 크레딧 충전 (첫 충전 시 25% 보너스, 최대 $100)
3. 대시보드에서 API 키 복사

### Python — 전체 워크플로

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

    if image_url:
        payload["input"]["image"] = image_url

    response = requests.post(
        f"{BASE_URL}/predictions",
        headers=HEADERS,
        json=payload
    )
    response.raise_for_status()
    prediction_id = response.json()["id"]
    print(f"Submitted: {prediction_id}")

    for _ in range(120):
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

### cURL — 빠른 테스트

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

# Poll result (PREDICTION_ID를 반환된 ID로 교체하세요)
curl -s "https://api.atlascloud.ai/v1/predictions/PREDICTION_ID" \
  -H "Authorization: Bearer $ATLAS_API_KEY"
```

---

## 프롬프트 엔지니어링 기초

프롬프트 라이브러리를 사용하기 전에, 다음 핵심 원칙을 이해하면 생성 품질이 비약적으로 향상됩니다.

### 6요소 NSFW 비디오 프롬프트 공식

고품질 NSFW 비디오 프롬프트에는 다음 6개 요소가 순서대로 포함되어야 합니다:

```
[피사체] + [동작/움직임] + [배경/환경] + [조명] + [카메라] + [스타일/분위기]
```

| 요소 | 역할 | 예시 |
|:-----|:-----|:-----|
| **피사체** | 화면에 누가 있는지 | "A tall woman with long dark hair and olive skin" |
| **동작/움직임** | 무엇이 일어나는지 (비디오의 핵심) | "slowly removes her dress, letting it fall to the floor" |
| **배경/환경** | 어디에서 일어나는지 | "in a minimalist loft apartment with exposed brick walls" |
| **조명** | 피부 렌더링과 분위기에 영향 | "warm golden hour light streaming through venetian blinds" |
| **카메라** | 어떻게 촬영하는지 | "medium shot, slight low angle, shallow depth of field" |
| **스타일/분위기** | 전반적인 시각 및 감정 톤 | "cinematic, sensual, intimate atmosphere" |

### NSFW 전용 팁

**1. 필요시 신체 디테일을 명확히 기술**
- 나쁜 예: 「She takes off her clothes」
- 좋은 예: 「She slowly unbuttons her blouse from top to bottom, revealing a black lace bralette underneath. The fabric parts to show her midriff and décolletage.」

**2. 시간 순서대로 동작을 기술**
- 나쁜 예: 「She dances seductively」
- 좋은 예: 「She sways her hips left and right in a slow rhythm, raises her arms above her head, then slowly runs her hands down along her body from chest to thighs.」

**3. 조명은 피부 렌더링의 핵심**
- 「Soft diffused studio lighting with a warm key light at 45 degrees」가 「bright lighting」보다 10배 좋은 결과
- 「Rim lighting highlighting body contours」는 드라마틱한 실루엣을 생성
- 「Candlelight」는 따뜻함을 추가하지만 디테일은 감소

**4. 하지 말아야 할 것을 지정 (네거티브 프롬프트)**
- 추가: 「No morphing, no distortion, no extra limbs, consistent body proportions throughout」
- 얼굴: 「Consistent facial features, no face warping between frames」

**5. 재생 시간이 프롬프트 복잡도에 영향**
- 5초 동영상: 최대 1-2개 동작
- 8-10초 동영상: 2-3개 연속 동작 가능
- 15초 동영상: 3-4개 비트의 미니 내러티브 가능

### 각 모델 최적 프롬프트 길이

| 모델 | 최적 프롬프트 길이 | 비고 |
|:-----|:-----------------|:-----|
| Wan 2.2 Spicy | 40–80 단어 | 짧을수록 = 아티팩트 적음 |
| Wan 2.5/2.6 | 60–120 단어 | 복잡한 기술에 대응 |
| Seedance v1.5 | 80–150 단어 | 상세한 기술에서 최상의 결과 |
| Vidu Q3-Pro | 50–100 단어 | 간결한 프롬프트가 최적 |
| Kling v3.0 Pro | 60–120 단어 | 상세한 얼굴 기술이 가장 효과적 |

---

## 카테고리 1: 로맨틱 & 센슈얼 (20개)

친밀함, 감정적 연결, 관능미에 초점. 추천 모델: **Wan 2.6**, **Kling v3.0 Pro**, **Seedance v1.5 Pro**.

### RS-01: 골든아워 창가

```
A woman with sun-kissed skin and wavy auburn hair stands barefoot by an open window,
wearing only a loose white linen shirt that reaches mid-thigh. A warm breeze pushes the
sheer curtains inward, pressing the fabric against her body and revealing her silhouette.
She closes her eyes, tilts her head back, and inhales deeply, her chest rising. The golden
hour sun creates a warm halo around her figure. Medium shot, soft focus background,
cinematic color grading with warm amber tones.
```

### RS-02: 아침의 여운

```
Close-up transitioning to medium shot. A woman lies on rumpled white sheets, bare shoulders
and upper back visible. She slowly rolls onto her side, pulling the sheet loosely across
her chest. Morning light filters through sheer curtains, casting soft shadows across her
skin. She reaches one arm above her head and stretches languidly, the sheet slipping to
reveal her waist. Sleepy, satisfied expression. Warm, intimate atmosphere. Shallow depth
of field on her face.
```

### RS-03: 캔들라이트 목욕

```
A woman reclines in a freestanding clawfoot bathtub filled with milky water and rose petals.
Dozens of candles surround the tub on the marble floor. She lifts one leg slowly out of the
water, water droplets catching the candlelight as they trail down her shin. She runs a hand
along her wet collarbone. Steam rises softly. Warm amber lighting, overhead wide shot slowly
pushing in to a medium close-up. Relaxed, luxurious mood.
```

### RS-04: 발코니의 비

```
A woman in a soaked white tank top and cotton shorts stands on a balcony during a warm
summer rainstorm. The wet fabric clings to every curve of her body, becoming translucent.
She tilts her face up to the rain, eyes closed, water streaming down her neck and chest.
She slowly pushes wet hair back from her face with both hands, arching her back slightly.
Moody blue-grey sky in the background, warm skin tones. Medium shot, slight upward angle.
```

### RS-05: 실크 로브 드롭

```
A woman with sleek black hair stands in a dimly lit bedroom. She is wearing a burgundy
silk robe loosely tied at the waist. She slowly pulls the sash, the robe falling open to
reveal a matching silk slip underneath that barely reaches her upper thighs. She lets the
robe slide off her shoulders and drop to the floor. Side lighting from a bedside lamp
creates dramatic shadows along her figure. Slow, deliberate movement. Tight medium shot
from the waist up, then tilts down as the robe falls.
```

### RS-06: 커플 샤워

```
A couple stands together under a large rainfall shower head. Water cascades over both
bodies. The man stands behind the woman, his arms wrapped around her waist. She leans
her head back against his chest, eyes closed. Water streams between their bodies. Both
are shown from the shoulders up and waist. Steam fills the glass enclosure. Warm soft
lighting. Slow motion water droplets. Intimate, tender atmosphere. Shot through the
slightly fogged glass door.
```

### RS-07: 황혼의 해변

```
A woman in a tiny black bikini walks along the shoreline at sunset. Waves lap at her
ankles. She pauses, facing the ocean, and slowly reaches behind her back to untie the
bikini top. She holds it in one hand at her side, back to camera, silhouetted against
the orange and purple sky. Her long hair blows in the sea breeze. Wide shot with the
sun low on the horizon. Warm cinematic color grading. Peaceful, free, confident energy.
```

### RS-08: 거울 앞에서

```
A woman stands before a large ornate floor mirror in her bedroom, wearing only matching
black lace underwear. She turns slowly, examining herself from different angles. She runs
her fingertips along her hip and up her ribcage. The camera captures both her and her
reflection simultaneously, creating a dual perspective. Soft warm side lighting from a
lamp off-screen. Medium full-body shot. Self-assured, appreciative expression. Intimate
boudoir atmosphere.
```

### RS-09: 오일 마사지

```
A woman lies face down on a massage table, a white sheet draped low across her hips. Her
bare back glistens with massage oil. A pair of hands enters the frame, pressing firmly
along her spine from lower back to shoulders. She exhales deeply, her shoulder blades
shifting under the skin. Oil catches the warm overhead light. Close-up on hands working
muscle groups, then pulls back to a medium shot. Relaxing ambient mood. Soft focused
background.
```

### RS-10: 벽난로의 밤

```
A woman sits on a plush fur rug in front of a roaring fireplace, wearing an oversized
knit sweater and nothing else. She draws her bare legs up to one side, the sweater riding
up to her upper thighs. She holds a glass of red wine, takes a slow sip, and gazes into
the fire. Warm flickering firelight dances across her skin and legs. The room is otherwise
dark. Tight medium shot. Cozy, seductive atmosphere. Shallow depth of field with bokeh
from the fire.
```

### RS-11: 댄스플로어

```
Low-key club lighting with deep purple and blue tones. A woman in a backless sequined
mini dress moves her body in a slow, hypnotic rhythm. She runs one hand down her neck to
her chest as she sways. Her back is arched, hips moving in a figure-eight pattern. Sweat
glistens on her shoulders and décolletage. Slow motion captures the fabric catching the
light. Medium shot from slightly below eye level. Smoky, charged atmosphere.
```

### RS-12: 노천 온천

```
A woman sits in a natural hot spring pool surrounded by snow-covered rocks and pine trees.
Steam rises thickly around her. She is submerged to her collarbone. She slowly stands up
in the pool, water cascading off her body, revealing her bare shoulders, back, and waist
as she rises. She wrings out her long wet hair. Misty mountain backdrop. Natural overcast
lighting. Wide establishing shot transitioning to medium shot as she stands. Serene,
ethereal mood.
```

### RS-13: 빈티지 부두아르

```
Styled as a 1940s glamour photograph come to life. A woman with victory rolls hairstyle
and red lipstick reclines on a chaise longue wearing a vintage corset, garter belt, and
seamed stockings. She slowly extends one leg upward, pointing her toe, running her hand
along the stocking from ankle to thigh. Soft focus lens effect. Warm sepia-toned lighting.
Medium shot with slight Dutch angle. Old Hollywood glamour aesthetic.
```

### RS-14: 옥상의 석양

```
A woman stands alone on an urban rooftop at sunset, city skyline in the distance. She is
wearing a flowing summer dress. She reaches down, grabs the hem, and slowly lifts the dress
up and over her head in one fluid motion, revealing a simple nude-toned bra and underwear.
She tosses the dress aside and stands with arms slightly open, facing the setting sun.
Wind catches her hair. Wide shot with shallow depth of field on the city background.
Liberating, confident mood.
```

### RS-15: 실크 시트 티즈

```
A woman lies on dark navy silk sheets, her body partially concealed and partially revealed
by the fabric. She slowly pulls the sheet downward from her collarbone, revealing her bare
chest, while simultaneously drawing one knee up, the sheet draping between her legs. She
bites her lower lip subtly and maintains eye contact with the camera. Overhead bird's eye
view slowly rotating. Single dramatic spotlight creating deep shadows. Provocative, intense.
```

### RS-16: 커플 슬로우 댄스

```
A couple in a dimly lit living room dances slowly, no music audible. She wears only his
unbuttoned dress shirt, which hangs to mid-thigh. He is shirtless in dress pants. His
hands rest on her bare hips beneath the shirt. She has her arms around his neck. They move
in a slow circle, foreheads touching. The shirt rides up as they turn. Single warm light
source from a floor lamp. Tight two-shot. Deeply intimate, romantic energy. Shallow depth
of field.
```

### RS-17: 풀 출수

```
Slow motion. A woman emerges from a turquoise swimming pool, climbing out via the ladder.
She wears a white one-piece swimsuit that has become completely see-through from the water.
Water streams off her body as she rises. She pushes her wet hair back with both hands, back
arched, face tilted toward the sun. Crystal water droplets catch the bright midday sunlight.
Low angle shot from water level. Vibrant summer color palette. Confident, carefree energy.
```

### RS-18: 역재생 착의

```
Time-reversed sequence played forward. A woman appears to be slowly getting undressed,
but the motion is natural. She stands before a closet mirror, unzipping a tight cocktail
dress from the back. The zipper slowly descends, revealing bare skin down her spine. She
slides the dress down past her hips and steps out of it, standing in just a strapless bra
and thong. She unclasps the bra from behind. Camera follows the dress down, then pans back
up her body. Bedroom lighting, warm tones.
```

### RS-19: 요가 플로우

```
A woman performs a sensual yoga flow on a mat in a sunlit studio with floor-to-ceiling
windows. She wears only tiny yoga shorts and a sports bra. She transitions from downward
dog — the camera behind and slightly below her, capturing her stretched form — into cobra
pose, arching her back deeply, chest forward, looking upward. Then flows into pigeon pose,
one leg stretched behind, torso upright, hands on her thigh. Smooth continuous motion.
Natural daylight. Full-body medium shot. Athletic, graceful, sensual.
```

### RS-20: 귓속말

```
Extreme close-up on a woman's face and neck. She is lying down, looking up at someone
off-camera above her. She whispers something inaudible, lips parting, eyes half-closed.
A man's hand enters the frame, gently tracing a line from her ear, down her jaw, along
her neck, to her collarbone. She tilts her chin up at his touch, exposing her throat. Her
breathing visibly quickens. Very soft focus. Warm, dim lighting. Airy, breathy, electric
tension. Macro lens effect.
```

---

## 카테고리 2: 아티스틱 누드 & 인체 연구 (15개)

고전 미술에서 영감을 받은, 인체의 아름다움에 초점을 맞춘 프롬프트. 추천 모델: **Wan 2.6**, **Seedance v1.5 Pro**, **Kling v3.0 Pro**.

### AN-01: 키아로스쿠로 연구

```
A nude woman stands in profile against a completely black background, lit by a single
harsh directional light from the upper left, creating deep Caravaggio-style chiaroscuro.
She slowly raises her arms in an arc above her head, fingers spread, each muscle and
tendon in her torso becoming visible as she stretches. Light catches only the ridgeline
of her body — shoulder, breast, hip, thigh — while everything else falls to pure black.
Slow, deliberate movement like a living sculpture. Full-body profile shot. Fine art
aesthetic, museum-quality composition.
```

### AN-02: 바디 랜드스케이프

```
Extreme close-up macro cinematography of a nude female torso, shot so closely that the
body becomes an abstract landscape. Camera slowly pans across skin terrain — the valley
of the collarbone, the gentle slope of the breast, the plateau of the stomach, the ridge
of the hip bone. Skin texture is visible at pore level. Warm side lighting creates
topographic shadows. The body rises and falls with slow breathing. No face visible.
Abstract, meditative, sculptural. Shot on macro lens with extremely shallow depth of field.
```

### AN-03 ~ AN-15

영어 버전과 동일한 프롬프트 (AN-03부터 AN-15). [영어 버전 카테고리 2](./README.md#category-2-artistic-nude--figure-study-15-prompts)를 참조하세요.

> **팁:** AI 비디오 모델은 영어 프롬프트에서 최상의 결과를 생성하므로 영어 원문을 유지합니다. API에 그대로 복사하여 사용하세요.

---

## 카테고리 3: 란제리 & 패션 (15개)

의류 인터랙션, 패션 프레젠테이션, 섹시한 란제리의 미학에 초점. 추천 모델: **Kling v3.0 Pro**, **Seedance v1.5 Pro**, **Wan 2.6**.

### LF-01: 블랙 레이스

```
A woman stands in a luxury walk-in closet, wearing a full-length black silk robe. She
faces a three-panel mirror. She slowly parts the robe, revealing an intricate black lace
bodysuit underneath — delicate floral patterns with scalloped edges. She turns to view
herself from different angles, the lace creating complex shadow patterns on her skin.
She adjusts a strap on her shoulder. Warm vanity lighting. Medium shot in mirror
reflection. High fashion editorial style, Victoria's Secret aesthetic.
```

### LF-02: 스타킹 착용

```
Close-up to medium shot. A woman sits on the edge of a bed, wearing only matching pearl-white
bra and underwear. She holds a sheer black thigh-high stocking. She points her toe and
slowly rolls the stocking up her leg from ankle to mid-thigh, smoothing it against her
skin with both hands as she goes. The sheer fabric catches the light. She clips it to a
garter belt. Camera follows the stocking from foot to thigh. Warm bedroom lighting.
Sensual, deliberate pace. Retro pin-up aesthetic.
```

### LF-03 ~ LF-15

영어 버전과 동일한 프롬프트. [영어 버전 카테고리 3](./README.md#category-3-lingerie--fashion-15-prompts)을 참조하세요.

---

## 카테고리 4: 판타지 & 신화 (15개)

누드와 판타지/신화적 요소를 결합한 상상력 넘치는 장면. 추천 모델: **Wan 2.6 T2V**, **Seedance v1.5 Pro**, **Vidu Q3-Pro**.

### FM-01: 숲의 요정

```
A nude woman with ivy and small flowers woven into her long green-tinted hair emerges from
behind an ancient mossy oak tree in a dense enchanted forest. Her skin has a faint luminous
green undertone. Fireflies circle around her. She reaches out one hand, and a butterfly
lands on her fingertip. She moves between the trees with inhuman grace, bare feet silent
on the moss. Dappled sunlight filtering through the canopy. Wide shot pulling into medium
shot as she approaches. Fantasy color grading — saturated greens and warm golden light.
```

### FM-02: 세이렌의 노래

```
A nude woman with pale blue-white skin and long silver hair sits on a dark ocean rock
at twilight. Her lower body transitions into iridescent fish scales at the hips (mermaid).
Waves crash around her. She tilts her head back and opens her mouth as if singing — visible
ripples emanate from her in the water. Bioluminescent plankton glow in the waves around
her. Her eyes have an otherworldly blue glow. Wide cinematic shot. Dark fantasy color
palette — deep navy, silver, teal. Epic orchestral atmosphere.
```

### FM-03 ~ FM-15

영어 버전과 동일한 프롬프트. [영어 버전 카테고리 4](./README.md#category-4-fantasy--mythology-15-prompts)를 참조하세요.

---

## 카테고리 5: 애니메이션 & 헨타이 (15개)

애니메이션 및 만화 스타일의 NSFW 콘텐츠. 추천 모델: **Wan 2.2 Spicy LoRA** (애니메이션 LoRA 사용), **Wan 2.5 T2V**, **Vidu Q3-Pro**.

### AH-01: 온천 에피소드

```
Anime style. A girl with long pink hair and large blue eyes sits in a traditional Japanese
onsen (hot spring). Steam rises around her. She is submerged to her collarbone, her bare
shoulders visible. She stands up slowly in the water, revealing her back and the side of
her chest. Water streams down her anime-style body. She wraps a small white towel around
herself that barely covers her chest and upper thighs. Cherry blossom petals float on the
water surface. Soft pastel color palette. Typical anime hot spring episode aesthetic.
```

### AH-02: 해변 에피소드 팬서비스

```
Anime style. A girl with short blue hair in a tiny white micro bikini runs along a sunny
anime beach. Classic anime running pose — arms pumping, breasts bouncing with exaggerated
physics. She trips and falls forward into the shallow surf. The bikini top's tie comes
undone. She sits up in the water, clutching the loose top to her chest with one arm, face
bright red with embarrassment. Sparkly water effects. Bright saturated colors. Classic
ecchi anime beach episode fanservice scene. Dynamic motion.
```

### AH-03: 변신 시퀀스

```
Anime magical girl transformation sequence. A girl with twin-tail purple hair is surrounded
by ribbons of glowing light. Her school uniform dissolves into particles from top to bottom,
briefly showing her nude silhouette bathed in magical light. Glowing ribbons wrap around her
body, forming a new magical girl outfit. During the 2-second nude phase, the body is detailed
but covered by strategic light flares and ribbon trails. Hair grows longer and changes to
silver. Eyes glow. Sparkle effects everywhere. Dynamic rotating camera. Sailor Moon meets
modern ecchi aesthetic.
```

### AH-04: 달빛 창가

```
Anime style. A girl with long black hair in a sheer white nightgown sits on a windowsill
in her bedroom at night, one leg dangling. Moonlight renders the nightgown translucent,
clearly showing her body underneath. She gazes at the moon pensively. The breeze lifts the
hem of the nightgown. She hugs her knees to her chest, the fabric stretching taut. Her room
is visible behind her — a desk with homework, a bed with stuffed animals. Romantic, slightly
melancholic mood. Soft blue moonlight. Medium shot. Seinen anime aesthetic.
```

### AH-05: 탈의실

```
Anime style. A girl with a ponytail stands in a school locker room after swimming class.
She is pulling off her one-piece school swimsuit, peeling it down from her shoulders. The
suit is bunched at her waist, her bare upper body visible from the side angle. Water droplets
on her anime-style skin. Steam from nearby showers in the background. Blurred background
figures of other students (not detailed). She reaches for a towel on a hook. Bright
fluorescent lighting. Classic ecchi anime perspective with careful framing.
```

### AH-06: 고양이귀 메이드

```
Anime style. A catgirl with white hair, cat ears, and a fluffy tail wears a very short
French maid outfit with a deeply plunging neckline. She bends forward at the waist to
pick up a fallen duster, the camera positioned low, capturing the skirt riding up to
reveal white lace underwear. Her tail swishes playfully. She looks over her shoulder
with a mischievous expression, one fang visible. She straightens up and adjusts her
headband. Ornate anime mansion background. Bright, colorful. Moe anthropomorphism aesthetic.
```

### AH-07: 온천 타올 드롭

```
Anime style. A busty girl with red hair wrapped in a small white towel walks into an
outdoor hot spring area at a ryokan. As she steps down into the water, the towel loosens
and begins to unwrap. She gasps, grabbing at it, but it slips away, floating on the water
surface. She quickly submerges to her neck, arms crossed over her chest, face completely
red. Steam conveniently partially obscures the scene. Close-up on her embarrassed face,
then wide shot of the scenic mountain onsen. Comedy ecchi moment.
```

### AH-08: 서큐버스의 유혹

```
Dark anime style. A succubus with short black horns, bat-like wings, and a spaded tail
floats above a sleeping man's bed. She wears only a strappy leather micro-outfit that
covers almost nothing. Her skin is a faint lavender hue, eyes glowing amber. She descends
slowly, sitting on the edge of the bed. She leans forward, her tail curling playfully. Her
wings fold behind her. Dark purple and crimson color palette with magical particle effects.
Detailed shadows on her voluptuous anime figure. Seinen dark fantasy aesthetic.
```

### AH-09 ~ AH-15

영어 버전과 동일한 프롬프트. [영어 버전 카테고리 5](./README.md#category-5-anime--hentai-15-prompts)를 참조하세요.

---

## 카테고리 6: 익스플리시트 액션 (15개)

익스플리시트 성적 콘텐츠 프롬프트. 완전한 NSFW 기능을 가진 모델이 필요합니다. 추천 모델: **Wan 2.2 Spicy** (거의 100% 준수율의 유일한 모델).

> **모델 참고:** Wan 2.2 Spicy만이 익스플리시트 액션 콘텐츠를 안정적으로 생성합니다. Wan 2.5의 성공률은 약 50%입니다. Wan 2.6, Seedance, Vidu, Kling은 NSFW 화이트리스트가 있어도 이러한 프롬프트의 대부분을 거부합니다.

### EA-01 ~ EA-15

영어 버전과 동일한 15개 익스플리시트 콘텐츠 프롬프트. [영어 버전 카테고리 6](./README.md#category-6-explicit-action-15-prompts)을 참조하세요.

---

## 카테고리 7: 시네마틱 & 내러티브 (10개)

스토리가 있는 NSFW 프롬프트. 추천 모델: **Seedance v1.5 Pro**, **Kling v3.0 Pro**, **Wan 2.6**.

### CN-01 ~ CN-10

영어 버전과 동일한 10개 시네마틱 내러티브 프롬프트. [영어 버전 카테고리 7](./README.md#category-7-cinematic--narrative-10-prompts)을 참조하세요.

---

## 카테고리 8: 페티쉬 & 니치 (10개)

특정 미적 취향에 특화된 콘텐츠. 추천 모델: **Wan 2.2 Spicy**, **Wan 2.5**.

### FN-01 ~ FN-10

영어 버전과 동일한 10개 페티쉬 프롬프트. [영어 버전 카테고리 8](./README.md#category-8-fetish--niche-10-prompts)을 참조하세요.

---

## 모델별 최적화 가이드

### Wan 2.2 Spicy — 익스플리시트 콘텐츠 최적 ($0.03/초부터)

| 설정 | 추천값 | 이유 |
|:-----|:-------|:-----|
| 해상도 | 720p | 품질/속도 최적 균형 |
| 길이 | 5초 | 8초에서는 품질이 크게 저하 |
| 프롬프트 길이 | 40–80 단어 | 짧을수록 = 아티팩트 적음 |
| I2V vs LoRA | 사실적이면 I2V, 스타일화는 LoRA | LoRA는 스타일 추가하지만 품질 약간 감소 |

**Spicy 프롬프트 팁:**
- 액션으로 시작, 배경이 아닌: 「She removes her dress...」, 「In a bedroom with oak furniture...」가 아닌
- 반드시 포함: 「consistent body proportions, no distortion, no morphing」
- 카메라 앵글은 하나만 지정 — 여러 앵글은 모델을 혼란시킴
- 효과적인 피부 조명 키워드: 「warm key light」「soft diffused」「golden hour」
- 복잡한 다인 장면은 피하기 (품질이 크게 떨어짐)

### Wan 2.5/2.6 — 고품질 누드의 가성비 최강 ($0.05–$0.07/초부터)

| 설정 | 추천값 | 이유 |
|:-----|:-------|:-----|
| 해상도 | 720p–1080p | 2.6에서는 1080p 가치 있음 |
| 길이 | 5–10초 | 긴 클립 처리 능력 우수 |
| 프롬프트 길이 | 60–120 단어 | Spicy보다 더 많은 디테일 활용 |
| 모드 | I2V | T2V보다 NSFW 준수율 높음 |

**Wan 2.5/2.6 팁:**
- 예술적 프레이밍 언어 사용: 「fine art photograph」「museum-quality figure study」
- 포르노그래피 용어 대신 임상적/예술적 용어로 누드 기술
- 2.6 강점: 아티스틱 누드, 바디 랜드스케이프, 미술

### Seedance v1.5 Pro — 프리미엄 시네마틱 품질 ($0.044/초부터)

| 설정 | 추천값 | 이유 |
|:-----|:-------|:-----|
| 해상도 | 720p | 현재 유일한 옵션 |
| 길이 | 5–15초 | 긴 클립 처리 탁월 |
| 프롬프트 길이 | 80–150 단어 | 상세한 기술에서 최상의 결과 |
| 접근 | NSFW 화이트리스트 필요 | Atlas Cloud에서 신청 |

**Seedance 팁:**
- 환경의 상세한 기술에 투자 — Seedance는 환경 렌더링이 매우 뛰어남
- 카메라 무브먼트 지정: 「slow dolly in」「tracking shot」「crane shot from above」
- 최적 용도: 란제리, 아티스틱 누드, 판타지, 시네마틱 내러티브

### Vidu Q3-Pro — 품질/가격 균형 ($0.06/초부터)

| 설정 | 추천값 | 이유 |
|:-----|:-------|:-----|
| 해상도 | 720p–1080p | 둘 다 좋은 결과 |
| 길이 | 5–10초 | 시간적 일관성 양호 |
| 프롬프트 길이 | 50–100 단어 | 간결한 프롬프트가 최적 |
| 접근 | NSFW 화이트리스트 필요 | Atlas Cloud에서 이용 가능 |

### Kling v3.0 Pro — 최고의 얼굴 품질 ($0.204/초부터)

| 설정 | 추천값 | 이유 |
|:-----|:-------|:-----|
| 해상도 | 최대 1080p | 높은 해상도 = 더 나은 얼굴 |
| 길이 | 5–10초 | 시간적 일관성 양호 |
| 프롬프트 길이 | 60–120 단어 | 상세한 얼굴 기술이 가장 효과적 |
| 접근 | NSFW 화이트리스트 필요 | Atlas Cloud에서 이용 가능 |

---

## 고급 프롬프트 기법

### 기법 1: 시간 시퀀싱

프롬프트를 타임라인으로 구조화하여 더 일관된 모션을 달성:

```
비트 1 (0-2초): [시작 상태 — 시청자가 처음 보는 것]
비트 2 (2-4초): [전환 — 핵심 동작 또는 변화]
비트 3 (4-5초): [종료 상태 — 마지막 프레임]
```

### 기법 2: 참조 이미지 전략

I2V 모델에서 참조 이미지는 결과의 60%를 결정합니다:

- **얼굴 선명도**: 명확하고 충분한 조명, 원하는 표정
- **포즈 기반**: 시작 포즈가 프롬프트의 시작 상태와 일치해야 함
- **조명 일치**: 이미지 조명이 프롬프트의 조명 기술과 일치해야 함
- **의상 일치**: 탈의를 포함하는 프롬프트는 이미지에 시작 의상을 표시
- **해상도**: 높은 해상도의 참조 이미지 = 더 나은 출력 (최소 1024x1024)

### 기법 3: 반복적 개선 워크플로

저비용으로 테스트하고 단계적으로 스케일업:

1. **초안**: Wan 2.2 Spicy ($0.03) — 핵심 컨셉 테스트
2. **개선**: Wan 2.5 ($0.05) — 시각 품질 향상 확인
3. **최종**: Seedance/Kling ($0.20+) — 완성된 최종 버전 제작

이 워크플로는 3회 생성에 $0.28, 프리미엄 모델부터 시작할 경우의 $0.60+에 비해 대폭 절약.

---

## 배치 생성 스크립트

여러 프롬프트의 효율적인 배치 생성 스크립트는 [영어 버전 배치 생성 스크립트](./README.md#batch-generation-script)를 참조하세요.

코드 코멘트는 영어이며, 그대로 복사하여 사용할 수 있습니다.

---

## 자주 묻는 질문

### 어떤 모델을 사용해야 하나요?

| 필요 | 최적 모델 | 가격 | 이유 |
|:-----|:---------|:-----|:-----|
| 익스플리시트 성적 콘텐츠 | Wan 2.2 Spicy | $0.03 | 거의 100% 익스플리시트 준수의 유일한 모델 |
| 고품질 아티스틱 누드 | Wan 2.6 | $0.07 | 비익스플리시트 NSFW의 품질/가격 왕 |
| 프리미엄 시네마틱 품질 | Seedance v1.5 Pro | $0.222 | 최고의 모션 및 환경 렌더링 |
| 최고의 얼굴 렌더링 | Kling v3.0 Pro | $0.204 | 얼굴 디테일과 표정에서 독보적 |
| 예산 제한이지만 품질 중시 | Vidu Q3-Pro | $0.06 | 품질과 가격의 좋은 균형 |
| 애니메이션/스타일화 | Wan 2.2 Spicy LoRA | $0.03 | 애니메이션 LoRA로 스타일화 출력 |
| 테스트/프로토타입 | Wan 2.2 Spicy | $0.03 | 가장 저렴한 반복 |

### 전체 115개 프롬프트를 생성하면 얼마인가요?

| 모델 | 1회 가격 | 전체 115개 | 비고 |
|:-----|:---------|:----------|:-----|
| Wan 2.2 Spicy | $0.03 | **$3.45** | 가장 경제적, 모든 카테고리 대응 |
| Wan 2.5 | $0.05 | $5.75 | 익스플리시트의 약 30%가 거부됨 |
| Vidu Q3-Pro | $0.06 | $6.90 | 대부분의 익스플리시트가 거부됨 |
| Wan 2.6 | $0.07 | $8.05 | 익스플리시트의 약 60%가 거부됨 |
| Kling v3.0 Pro | $0.204 | $23.46 | 고품질, 제한적 익스플리시트 |
| Seedance v1.5 Pro | $0.222 | $25.53 | 고품질, 제한적 익스플리시트 |

**25% 첫 충전 보너스로 Spicy에서 전체 프롬프트 테스트:**
$3.00 충전 → $3.75 크레딧 획득 → 전체 115개 생성 후 $0.30 잔액.

### NSFW 화이트리스트 접근 방법은?

[Atlas Cloud](https://www.atlascloud.ai?ref=JPM683)에서 가입하고, 크레딧을 충전한 후 대시보드 또는 지원팀을 통해 NSFW 화이트리스트 접근을 신청하세요. 인증된 계정은 보통 24시간 이내에 승인됩니다.

### 이 프롬프트를 다른 플랫폼에서 사용할 수 있나요?

프롬프트 자체는 범용 텍스트입니다. 그러나 대부분의 다른 플랫폼(RunwayML, Pika, Luma)은 NSFW 콘텐츠를 거부합니다. [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683)는 무제한 NSFW 생성 API를 제공하는 몇 안 되는 플랫폼 중 하나입니다.

### 참조 이미지가 필요한가요?

**I2V (이미지-투-비디오)** 모델의 경우 참조 이미지가 필요하며 품질에 큰 영향을 미칩니다. **T2V (텍스트-투-비디오)** 모델의 경우 이미지가 필요하지 않습니다.

**추천:** 익스플리시트 콘텐츠의 경우에도 SFW 또는 약간 자극적인 참조 이미지로 시작하세요. 모델이 프롬프트에서 NSFW 콘텐츠를 생성하면서 이미지를 캐릭터 외모의 시각적 앵커로 사용합니다.

---

## 시작하기

<div align="center">

### NSFW AI 비디오 생성, 최저 $0.03부터

**[Atlas Cloud](https://www.atlascloud.ai?ref=JPM683)** — SOC I & II 인증 | HIPAA 준수 | 미국 법인

1. [계정 생성](https://www.atlascloud.ai?ref=JPM683)
2. 크레딧 충전 (첫 충전 시 25% 보너스, 최대 $100)
3. API 키 복사
4. 이 컬렉션의 아무 프롬프트나 사용

[![시작하기](https://img.shields.io/badge/지금_시작-Atlas_Cloud-blue?style=for-the-badge)](https://www.atlascloud.ai?ref=JPM683)

</div>

---

## Star 히스토리

<div align="center">

[![Star History Chart](https://api.star-history.com/svg?repos=thoughtincode/nsfw-ai-video-prompts&type=Date)](https://star-history.com/#thoughtincode/nsfw-ai-video-prompts&Date)

</div>

---

## 기여하기

기여를 환영합니다! 훌륭한 결과를 생성하는 NSFW 비디오 프롬프트가 있다면 PR을 제출해 주세요. 가이드라인:

1. 테스트한 모델과 결과 품질을 포함
2. 적절히 카테고리 분류
3. 충분한 세부사항 제공 (최소 3문장)
4. 기존 프롬프트의 포맷 패턴을 따르기
5. 합법적인 성인 콘텐츠만 — 미성년자, 비합의 시나리오, 불법 콘텐츠는 절대 금지

---

## 라이선스

MIT 라이선스. 자세한 내용은 [LICENSE](./LICENSE)를 참조하세요.

프롬프트는 자유롭게 사용, 수정, 배포할 수 있습니다. 생성된 콘텐츠는 사용하는 플랫폼의 이용약관을 따릅니다.

---

<div align="center">

**[Atlas Cloud](https://www.atlascloud.ai?ref=JPM683)가 크리에이티브 커뮤니티를 위해 제작**

*세계에서 가장 저렴한 NSFW AI 비디오 생성 플랫폼.*

</div>
