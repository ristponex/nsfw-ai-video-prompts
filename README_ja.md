<div align="center">

```
 _   _  ______        ______        ___    ___   __     __ _     _
| \ | |/ ___\ \      / /  __|      / _ \  |_ _|  \ \   / /(_) __| | ___  ___
|  \| |\___ \\ \ /\ / /| |_       / /_\ \  | |    \ \ / / | |/ _` |/ _ \/ _ \
| |\  | ___) |\ V  V / |  _|     / _____ \ | |     \ V /  | | (_| |  __/ (_) |
|_| \_||____/  \_/\_/  |_|      /_/     \_\|___|    \_/   |_|\__,_|\___|\___/

 プロンプトライブラリ — 100以上のすぐに使えるNSFW AIビデオプロンプト
```

# NSFW AIビデオプロンプトライブラリ — 100以上の詳細プロンプト、カテゴリ別整理

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![プロンプト数](https://img.shields.io/badge/プロンプト-100以上-blue)]()
[![対応モデル](https://img.shields.io/badge/対応モデル-5つの無検閲-red)]()
[![最終更新](https://img.shields.io/badge/更新日-2026年3月-green)]()
[![プラットフォーム](https://img.shields.io/badge/プラットフォーム-Atlas%20Cloud-purple)](https://www.atlascloud.ai?ref=JPM683)

**最大級のオープンソースNSFW AIビデオプロンプト集。全プロンプト実機テスト済み、カテゴリ別整理、各モデル向け最適化済み。**

**[English](./README.md)** | **[简体中文](./README_zh-CN.md)** | **[日本語](./README_ja.md)** | **[한국어](./README_ko.md)**

---

> **免責事項：** 本リポジトリは合法的な成人コンテンツ制作のみを目的としています。すべてのプロンプトは、成人（18歳以上）が法律で許可された地域で使用することを前提としています。未成年者、非合意シナリオ、その他の違法コンテンツに関わるいかなる制作にも厳しく反対します。ユーザーは現地の法令への準拠を自己責任で確保してください。

</div>

---

## 目次

- [対応モデルと料金](#対応モデルと料金)
- [料金比較：Atlas Cloud vs fal.ai](#料金比較atlas-cloud-vs-falai)
- [クイックスタート（API）](#クイックスタートapi)
- [プロンプトエンジニアリングの基礎](#プロンプトエンジニアリングの基礎)
- [カテゴリ1：ロマンティック＆センシュアル（20本）](#カテゴリ1ロマンティックセンシュアル20本)
- [カテゴリ2：アーティスティックヌード＆人体研究（15本）](#カテゴリ2アーティスティックヌード人体研究15本)
- [カテゴリ3：ランジェリー＆ファッション（15本）](#カテゴリ3ランジェリーファッション15本)
- [カテゴリ4：ファンタジー＆神話（15本）](#カテゴリ4ファンタジー神話15本)
- [カテゴリ5：アニメ＆ヘンタイ（15本）](#カテゴリ5アニメヘンタイ15本)
- [カテゴリ6：エクスプリシットアクション（15本）](#カテゴリ6エクスプリシットアクション15本)
- [カテゴリ7：シネマティック＆ナラティブ（10本）](#カテゴリ7シネマティックナラティブ10本)
- [カテゴリ8：フェティッシュ＆ニッチ（10本）](#カテゴリ8フェティッシュニッチ10本)
- [モデル別最適化ガイド](#モデル別最適化ガイド)
- [高度なプロンプトテクニック](#高度なプロンプトテクニック)
- [バッチ生成スクリプト](#バッチ生成スクリプト)
- [よくある質問](#よくある質問)
- [利用開始](#利用開始)
- [Star履歴](#star履歴)
- [ライセンス](#ライセンス)

---

## 対応モデルと料金

以下のモデルはすべて[Atlas Cloud API](https://www.atlascloud.ai?ref=JPM683)経由でアクセス可能で、NSFWコンテンツ生成が有効化されています。

| モデル | タイプ | 料金 | 解像度 | 再生時間 | NSFWレベル | 最適用途 |
|:-------|:-------|:-----|:-------|:---------|:-----------|:---------|
| **Wan 2.2 Spicy** | I2V / I2V-LoRA | **$0.03**/秒から | 480p, 720p | 5秒, 8秒 | 完全無制限 | 低コストのエクスプリシットコンテンツ |
| **Wan 2.5** | I2V / T2V | ~$0.05/秒から | 720p, 1080p | 5秒, 10秒 | ヌード＋中程度のエクスプリシット | 中品質 |
| **Wan 2.6** | I2V / T2V | $0.07/秒から | 最大1080p | 5–15秒 | ヌード（限定的エクスプリシット） | 高品質アーティスティックヌード |
| **Seedance v1.5 Pro** | T2V / I2V | **$0.044**/秒から | 720p | 5–15秒 | ホワイトリストNSFW | プレミアムシネマティック品質 |
| **Vidu Q3-Pro** | T2V / I2V | **$0.06**/秒から | 720p, 1080p | 5–10秒 | ホワイトリストNSFW | 品質/価格のバランス |
| **Kling v3.0 Pro** | T2V / I2V | **$0.204**/秒から | 最大1080p | 5–10秒 | ホワイトリストNSFW | モーション品質、顔 |

> **料金について：** 動画モデルの料金は生成動画1秒あたりの価格です。実際の料金は選択した解像度と再生時間によって異なります。
>
> **ホワイトリスト**とは、Atlas Cloudで承認を得た後にNSFWコンテンツを生成できることを意味します。ViduシリーズもホワイトリストでのNSFWコンテンツ生成に対応しています。

### 信頼性とセキュリティ

- **SOC I & II認証** — エンタープライズグレードのセキュリティコンプライアンス
- **HIPAA準拠** — 医療レベルのデータ保護
- **米国法人** — 米国データ保護法の適用
- **初回チャージで25%ボーナス**（最大$100）— [今すぐ登録](https://www.atlascloud.ai?ref=JPM683)

---

## 料金比較：Atlas Cloud vs fal.ai

fal.aiをご利用中の方へ、余分にお支払いの金額はこちらです：

### Wanモデル（5秒動画）

| プラットフォーム | 課金方式 | 5秒動画コスト | 100本のコスト |
|:---------------|:---------|:-------------|:-------------|
| **Atlas Cloud** | リクエスト毎 | **$0.05** | **$5.00** |
| fal.ai | 秒課金 ($0.05/秒) | $0.25 | $25.00 |
| **節約額** | | **80%** | **$20.00** |

### Klingモデル（5秒動画）

| プラットフォーム | 課金方式 | 5秒動画コスト | 100本のコスト |
|:---------------|:---------|:-------------|:-------------|
| **Atlas Cloud** | リクエスト毎 | **$0.204** | **$20.40** |
| fal.ai | 秒課金 ($0.224/秒) | $1.12 | $112.00 |
| **節約額** | | **82%** | **$91.60** |

### Wan 2.2 Spicy（Atlas Cloud限定）

| プラットフォーム | 5秒動画コスト | 100本のコスト | 1,000本のコスト |
|:---------------|:-------------|:-------------|:---------------|
| **Atlas Cloud** | **$0.03** | **$3.00** | **$30.00** |
| fal.ai | 提供なし | 提供なし | 提供なし |

> fal.aiは無検閲/NSFWモデルを提供していません。Atlas Cloudは完全無制限のNSFWビデオ生成APIを提供する数少ないプラットフォームの一つです。

---

## クイックスタート（API）

### 前提条件

1. [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683)でアカウントを作成
2. クレジットをチャージ（初回チャージで25%ボーナス、最大$100）
3. ダッシュボードからAPIキーをコピー

### Python — 完全なワークフロー

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

### cURL — クイックテスト

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

# Poll result (PREDICTION_IDを返されたIDに置き換えてください)
curl -s "https://api.atlascloud.ai/v1/predictions/PREDICTION_ID" \
  -H "Authorization: Bearer $ATLAS_API_KEY"
```

---

## プロンプトエンジニアリングの基礎

プロンプトライブラリを使用する前に、以下の原則を理解することで生成品質が劇的に向上します。

### 6要素NSFWビデオプロンプトフォーミュラ

高品質なNSFWビデオプロンプトには以下の6つの要素を含めるべきです：

```
[被写体] + [アクション/動き] + [シーン/環境] + [照明] + [カメラ] + [スタイル/雰囲気]
```

| 要素 | 目的 | 例 |
|:-----|:-----|:---|
| **被写体** | 誰が画面にいるか | "A tall woman with long dark hair and olive skin" |
| **アクション/動き** | 何が起こるか（ビデオの核心） | "slowly removes her dress, letting it fall to the floor" |
| **シーン/環境** | どこで起こるか | "in a minimalist loft apartment with exposed brick walls" |
| **照明** | 肌の描画と雰囲気に影響 | "warm golden hour light streaming through venetian blinds" |
| **カメラ** | どう撮影するか | "medium shot, slight low angle, shallow depth of field" |
| **スタイル/雰囲気** | 全体的な視覚と感情のトーン | "cinematic, sensual, intimate atmosphere" |

### NSFW専用テクニック

**1. 必要に応じて身体の詳細を明確に**
- 悪い例：「She takes off her clothes」
- 良い例：「She slowly unbuttons her blouse from top to bottom, revealing a black lace bralette underneath. The fabric parts to show her midriff and décolletage.」

**2. 時系列で動きを記述する**
- 悪い例：「She dances seductively」
- 良い例：「She sways her hips left and right in a slow rhythm, raises her arms above her head, then slowly runs her hands down along her body from chest to thighs.」

**3. 照明は肌の描画の鍵**
- 「Soft diffused studio lighting with a warm key light at 45 degrees」は「bright lighting」よりも10倍良い結果
- 「Rim lighting highlighting body contours」はドラマチックなシルエットを作成
- 「Candlelight」は温かみを追加するがディテールは低下

**4. やってはいけないことを指定する（ネガティブプロンプト）**
- 追加する：「No morphing, no distortion, no extra limbs, consistent body proportions throughout」
- 顔について：「Consistent facial features, no face warping between frames」

**5. 再生時間がプロンプトの複雑さに影響**
- 5秒動画：最大1-2アクション
- 8-10秒動画：2-3の連続アクションが可能
- 15秒動画：3-4ビートのミニナラティブが可能

### 各モデル最適プロンプト長

| モデル | 最適プロンプト長 | 備考 |
|:-------|:---------------|:-----|
| Wan 2.2 Spicy | 40–80語 | 短い = アーティファクト少ない |
| Wan 2.5/2.6 | 60–120語 | 複雑な記述に対応 |
| Seedance v1.5 | 80–150語 | 詳細な記述で最良の結果 |
| Vidu Q3-Pro | 50–100語 | 簡潔なプロンプトが得意 |
| Kling v3.0 Pro | 60–120語 | 詳細な顔の記述が最も効果的 |

---

## カテゴリ1：ロマンティック＆センシュアル（20本）

親密さ、感情的なつながり、官能性に焦点を当てたプロンプト。推奨モデル：**Wan 2.6**、**Kling v3.0 Pro**、**Seedance v1.5 Pro**。

### RS-01: ゴールデンアワーの窓辺

```
A woman with sun-kissed skin and wavy auburn hair stands barefoot by an open window,
wearing only a loose white linen shirt that reaches mid-thigh. A warm breeze pushes the
sheer curtains inward, pressing the fabric against her body and revealing her silhouette.
She closes her eyes, tilts her head back, and inhales deeply, her chest rising. The golden
hour sun creates a warm halo around her figure. Medium shot, soft focus background,
cinematic color grading with warm amber tones.
```

### RS-02: モーニングアフター

```
Close-up transitioning to medium shot. A woman lies on rumpled white sheets, bare shoulders
and upper back visible. She slowly rolls onto her side, pulling the sheet loosely across
her chest. Morning light filters through sheer curtains, casting soft shadows across her
skin. She reaches one arm above her head and stretches languidly, the sheet slipping to
reveal her waist. Sleepy, satisfied expression. Warm, intimate atmosphere. Shallow depth
of field on her face.
```

### RS-03: キャンドルバス

```
A woman reclines in a freestanding clawfoot bathtub filled with milky water and rose petals.
Dozens of candles surround the tub on the marble floor. She lifts one leg slowly out of the
water, water droplets catching the candlelight as they trail down her shin. She runs a hand
along her wet collarbone. Steam rises softly. Warm amber lighting, overhead wide shot slowly
pushing in to a medium close-up. Relaxed, luxurious mood.
```

### RS-04: バルコニーの雨

```
A woman in a soaked white tank top and cotton shorts stands on a balcony during a warm
summer rainstorm. The wet fabric clings to every curve of her body, becoming translucent.
She tilts her face up to the rain, eyes closed, water streaming down her neck and chest.
She slowly pushes wet hair back from her face with both hands, arching her back slightly.
Moody blue-grey sky in the background, warm skin tones. Medium shot, slight upward angle.
```

### RS-05: シルクローブドロップ

```
A woman with sleek black hair stands in a dimly lit bedroom. She is wearing a burgundy
silk robe loosely tied at the waist. She slowly pulls the sash, the robe falling open to
reveal a matching silk slip underneath that barely reaches her upper thighs. She lets the
robe slide off her shoulders and drop to the floor. Side lighting from a bedside lamp
creates dramatic shadows along her figure. Slow, deliberate movement. Tight medium shot
from the waist up, then tilts down as the robe falls.
```

### RS-06: カップルシャワー

```
A couple stands together under a large rainfall shower head. Water cascades over both
bodies. The man stands behind the woman, his arms wrapped around her waist. She leans
her head back against his chest, eyes closed. Water streams between their bodies. Both
are shown from the shoulders up and waist. Steam fills the glass enclosure. Warm soft
lighting. Slow motion water droplets. Intimate, tender atmosphere. Shot through the
slightly fogged glass door.
```

### RS-07: 夕暮れのビーチ

```
A woman in a tiny black bikini walks along the shoreline at sunset. Waves lap at her
ankles. She pauses, facing the ocean, and slowly reaches behind her back to untie the
bikini top. She holds it in one hand at her side, back to camera, silhouetted against
the orange and purple sky. Her long hair blows in the sea breeze. Wide shot with the
sun low on the horizon. Warm cinematic color grading. Peaceful, free, confident energy.
```

### RS-08: 鏡の前で

```
A woman stands before a large ornate floor mirror in her bedroom, wearing only matching
black lace underwear. She turns slowly, examining herself from different angles. She runs
her fingertips along her hip and up her ribcage. The camera captures both her and her
reflection simultaneously, creating a dual perspective. Soft warm side lighting from a
lamp off-screen. Medium full-body shot. Self-assured, appreciative expression. Intimate
boudoir atmosphere.
```

### RS-09: オイルマッサージ

```
A woman lies face down on a massage table, a white sheet draped low across her hips. Her
bare back glistens with massage oil. A pair of hands enters the frame, pressing firmly
along her spine from lower back to shoulders. She exhales deeply, her shoulder blades
shifting under the skin. Oil catches the warm overhead light. Close-up on hands working
muscle groups, then pulls back to a medium shot. Relaxing ambient mood. Soft focused
background.
```

### RS-10: 暖炉の夜

```
A woman sits on a plush fur rug in front of a roaring fireplace, wearing an oversized
knit sweater and nothing else. She draws her bare legs up to one side, the sweater riding
up to her upper thighs. She holds a glass of red wine, takes a slow sip, and gazes into
the fire. Warm flickering firelight dances across her skin and legs. The room is otherwise
dark. Tight medium shot. Cozy, seductive atmosphere. Shallow depth of field with bokeh
from the fire.
```

### RS-11: ダンスフロア

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

### RS-13: ヴィンテージブドワール

```
Styled as a 1940s glamour photograph come to life. A woman with victory rolls hairstyle
and red lipstick reclines on a chaise longue wearing a vintage corset, garter belt, and
seamed stockings. She slowly extends one leg upward, pointing her toe, running her hand
along the stocking from ankle to thigh. Soft focus lens effect. Warm sepia-toned lighting.
Medium shot with slight Dutch angle. Old Hollywood glamour aesthetic.
```

### RS-14: 屋上のサンセット

```
A woman stands alone on an urban rooftop at sunset, city skyline in the distance. She is
wearing a flowing summer dress. She reaches down, grabs the hem, and slowly lifts the dress
up and over her head in one fluid motion, revealing a simple nude-toned bra and underwear.
She tosses the dress aside and stands with arms slightly open, facing the setting sun.
Wind catches her hair. Wide shot with shallow depth of field on the city background.
Liberating, confident mood.
```

### RS-15: シルクシーツ

```
A woman lies on dark navy silk sheets, her body partially concealed and partially revealed
by the fabric. She slowly pulls the sheet downward from her collarbone, revealing her bare
chest, while simultaneously drawing one knee up, the sheet draping between her legs. She
bites her lower lip subtly and maintains eye contact with the camera. Overhead bird's eye
view slowly rotating. Single dramatic spotlight creating deep shadows. Provocative, intense.
```

### RS-16: カップルスローダンス

```
A couple in a dimly lit living room dances slowly, no music audible. She wears only his
unbuttoned dress shirt, which hangs to mid-thigh. He is shirtless in dress pants. His
hands rest on her bare hips beneath the shirt. She has her arms around his neck. They move
in a slow circle, foreheads touching. The shirt rides up as they turn. Single warm light
source from a floor lamp. Tight two-shot. Deeply intimate, romantic energy. Shallow depth
of field.
```

### RS-17: プール出水

```
Slow motion. A woman emerges from a turquoise swimming pool, climbing out via the ladder.
She wears a white one-piece swimsuit that has become completely see-through from the water.
Water streams off her body as she rises. She pushes her wet hair back with both hands, back
arched, face tilted toward the sun. Crystal water droplets catch the bright midday sunlight.
Low angle shot from water level. Vibrant summer color palette. Confident, carefree energy.
```

### RS-18: 逆再生の着替え

```
Time-reversed sequence played forward. A woman appears to be slowly getting undressed,
but the motion is natural. She stands before a closet mirror, unzipping a tight cocktail
dress from the back. The zipper slowly descends, revealing bare skin down her spine. She
slides the dress down past her hips and steps out of it, standing in just a strapless bra
and thong. She unclasps the bra from behind. Camera follows the dress down, then pans back
up her body. Bedroom lighting, warm tones.
```

### RS-19: ヨガフロー

```
A woman performs a sensual yoga flow on a mat in a sunlit studio with floor-to-ceiling
windows. She wears only tiny yoga shorts and a sports bra. She transitions from downward
dog — the camera behind and slightly below her, capturing her stretched form — into cobra
pose, arching her back deeply, chest forward, looking upward. Then flows into pigeon pose,
one leg stretched behind, torso upright, hands on her thigh. Smooth continuous motion.
Natural daylight. Full-body medium shot. Athletic, graceful, sensual.
```

### RS-20: 耳元の囁き

```
Extreme close-up on a woman's face and neck. She is lying down, looking up at someone
off-camera above her. She whispers something inaudible, lips parting, eyes half-closed.
A man's hand enters the frame, gently tracing a line from her ear, down her jaw, along
her neck, to her collarbone. She tilts her chin up at his touch, exposing her throat. Her
breathing visibly quickens. Very soft focus. Warm, dim lighting. Airy, breathy, electric
tension. Macro lens effect.
```

---

## カテゴリ2：アーティスティックヌード＆人体研究（15本）

古典美術にインスピレーションを得た、人体の美に焦点を当てたプロンプト。推奨モデル：**Wan 2.6**、**Seedance v1.5 Pro**、**Kling v3.0 Pro**。

### AN-01: キアロスクーロ研究

```
A nude woman stands in profile against a completely black background, lit by a single
harsh directional light from the upper left, creating deep Caravaggio-style chiaroscuro.
She slowly raises her arms in an arc above her head, fingers spread, each muscle and
tendon in her torso becoming visible as she stretches. Light catches only the ridgeline
of her body — shoulder, breast, hip, thigh — while everything else falls to pure black.
Slow, deliberate movement like a living sculpture. Full-body profile shot. Fine art
aesthetic, museum-quality composition.
```

### AN-02: ボディランドスケープ

```
Extreme close-up macro cinematography of a nude female torso, shot so closely that the
body becomes an abstract landscape. Camera slowly pans across skin terrain — the valley
of the collarbone, the gentle slope of the breast, the plateau of the stomach, the ridge
of the hip bone. Skin texture is visible at pore level. Warm side lighting creates
topographic shadows. The body rises and falls with slow breathing. No face visible.
Abstract, meditative, sculptural. Shot on macro lens with extremely shallow depth of field.
```

### AN-03 〜 AN-15

英語版と同一のプロンプト（AN-03からAN-15）。[英語版カテゴリ2](./README.md#category-2-artistic-nude--figure-study-15-prompts)をご参照ください。

> **ヒント：** AIビデオモデルは英語プロンプトで最良の結果を生成するため、英語原文を保持しています。APIにそのままコピー＆ペーストしてください。

---

## カテゴリ3：ランジェリー＆ファッション（15本）

衣服のインタラクション、ファッションプレゼンテーション、セクシーなランジェリーの美学に焦点を当てています。推奨モデル：**Kling v3.0 Pro**、**Seedance v1.5 Pro**、**Wan 2.6**。

### LF-01: ブラックレース

```
A woman stands in a luxury walk-in closet, wearing a full-length black silk robe. She
faces a three-panel mirror. She slowly parts the robe, revealing an intricate black lace
bodysuit underneath — delicate floral patterns with scalloped edges. She turns to view
herself from different angles, the lace creating complex shadow patterns on her skin.
She adjusts a strap on her shoulder. Warm vanity lighting. Medium shot in mirror
reflection. High fashion editorial style, Victoria's Secret aesthetic.
```

### LF-02: ストッキング装着

```
Close-up to medium shot. A woman sits on the edge of a bed, wearing only matching pearl-white
bra and underwear. She holds a sheer black thigh-high stocking. She points her toe and
slowly rolls the stocking up her leg from ankle to mid-thigh, smoothing it against her
skin with both hands as she goes. The sheer fabric catches the light. She clips it to a
garter belt. Camera follows the stocking from foot to thigh. Warm bedroom lighting.
Sensual, deliberate pace. Retro pin-up aesthetic.
```

### LF-03 〜 LF-15

英語版と同一のプロンプト。[英語版カテゴリ3](./README.md#category-3-lingerie--fashion-15-prompts)をご参照ください。

---

## カテゴリ4：ファンタジー＆神話（15本）

ヌードとファンタジー/神話要素を融合させた想像力豊かなシーン。推奨モデル：**Wan 2.6 T2V**、**Seedance v1.5 Pro**、**Vidu Q3-Pro**。

### FM-01: 森の精霊

```
A nude woman with ivy and small flowers woven into her long green-tinted hair emerges from
behind an ancient mossy oak tree in a dense enchanted forest. Her skin has a faint luminous
green undertone. Fireflies circle around her. She reaches out one hand, and a butterfly
lands on her fingertip. She moves between the trees with inhuman grace, bare feet silent
on the moss. Dappled sunlight filtering through the canopy. Wide shot pulling into medium
shot as she approaches. Fantasy color grading — saturated greens and warm golden light.
```

### FM-02: セイレーンの歌

```
A nude woman with pale blue-white skin and long silver hair sits on a dark ocean rock
at twilight. Her lower body transitions into iridescent fish scales at the hips (mermaid).
Waves crash around her. She tilts her head back and opens her mouth as if singing — visible
ripples emanate from her in the water. Bioluminescent plankton glow in the waves around
her. Her eyes have an otherworldly blue glow. Wide cinematic shot. Dark fantasy color
palette — deep navy, silver, teal. Epic orchestral atmosphere.
```

### FM-03 〜 FM-15

英語版と同一のプロンプト。[英語版カテゴリ4](./README.md#category-4-fantasy--mythology-15-prompts)をご参照ください。

---

## カテゴリ5：アニメ＆ヘンタイ（15本）

アニメ・マンガスタイルのNSFWコンテンツ。推奨モデル：**Wan 2.2 Spicy LoRA**（アニメLoRA使用）、**Wan 2.5 T2V**、**Vidu Q3-Pro**。

### AH-01: 温泉回

```
Anime style. A girl with long pink hair and large blue eyes sits in a traditional Japanese
onsen (hot spring). Steam rises around her. She is submerged to her collarbone, her bare
shoulders visible. She stands up slowly in the water, revealing her back and the side of
her chest. Water streams down her anime-style body. She wraps a small white towel around
herself that barely covers her chest and upper thighs. Cherry blossom petals float on the
water surface. Soft pastel color palette. Typical anime hot spring episode aesthetic.
```

### AH-02: ビーチ回ファンサービス

```
Anime style. A girl with short blue hair in a tiny white micro bikini runs along a sunny
anime beach. Classic anime running pose — arms pumping, breasts bouncing with exaggerated
physics. She trips and falls forward into the shallow surf. The bikini top's tie comes
undone. She sits up in the water, clutching the loose top to her chest with one arm, face
bright red with embarrassment. Sparkly water effects. Bright saturated colors. Classic
ecchi anime beach episode fanservice scene. Dynamic motion.
```

### AH-03: 変身シーケンス

```
Anime magical girl transformation sequence. A girl with twin-tail purple hair is surrounded
by ribbons of glowing light. Her school uniform dissolves into particles from top to bottom,
briefly showing her nude silhouette bathed in magical light. Glowing ribbons wrap around her
body, forming a new magical girl outfit. During the 2-second nude phase, the body is detailed
but covered by strategic light flares and ribbon trails. Hair grows longer and changes to
silver. Eyes glow. Sparkle effects everywhere. Dynamic rotating camera. Sailor Moon meets
modern ecchi aesthetic.
```

### AH-04: 月夜の窓辺

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

### AH-06: 猫耳メイド

```
Anime style. A catgirl with white hair, cat ears, and a fluffy tail wears a very short
French maid outfit with a deeply plunging neckline. She bends forward at the waist to
pick up a fallen duster, the camera positioned low, capturing the skirt riding up to
reveal white lace underwear. Her tail swishes playfully. She looks over her shoulder
with a mischievous expression, one fang visible. She straightens up and adjusts her
headband. Ornate anime mansion background. Bright, colorful. Moe anthropomorphism aesthetic.
```

### AH-07: 温泉タオル落ち

```
Anime style. A busty girl with red hair wrapped in a small white towel walks into an
outdoor hot spring area at a ryokan. As she steps down into the water, the towel loosens
and begins to unwrap. She gasps, grabbing at it, but it slips away, floating on the water
surface. She quickly submerges to her neck, arms crossed over her chest, face completely
red. Steam conveniently partially obscures the scene. Close-up on her embarrassed face,
then wide shot of the scenic mountain onsen. Comedy ecchi moment.
```

### AH-08: サキュバスの誘惑

```
Dark anime style. A succubus with short black horns, bat-like wings, and a spaded tail
floats above a sleeping man's bed. She wears only a strappy leather micro-outfit that
covers almost nothing. Her skin is a faint lavender hue, eyes glowing amber. She descends
slowly, sitting on the edge of the bed. She leans forward, her tail curling playfully. Her
wings fold behind her. Dark purple and crimson color palette with magical particle effects.
Detailed shadows on her voluptuous anime figure. Seinen dark fantasy aesthetic.
```

### AH-09 〜 AH-15

英語版と同一のプロンプト。[英語版カテゴリ5](./README.md#category-5-anime--hentai-15-prompts)をご参照ください。

---

## カテゴリ6：エクスプリシットアクション（15本）

エクスプリシットな性的コンテンツのプロンプト。完全なNSFW機能を持つモデルが必要です。推奨モデル：**Wan 2.2 Spicy**（唯一ほぼ100%のコンプライアンス率）。

> **モデル注記：** Wan 2.2 Spicyのみがエクスプリシットアクションコンテンツを確実に生成できます。Wan 2.5の成功率は約50%です。Wan 2.6、Seedance、Vidu、KlingはNSFWホワイトリストがあっても、これらのプロンプトのほとんどを拒否します。

### EA-01 〜 EA-15

英語版と同一の15本のエクスプリシットコンテンツプロンプト。[英語版カテゴリ6](./README.md#category-6-explicit-action-15-prompts)をご参照ください。

---

## カテゴリ7：シネマティック＆ナラティブ（10本）

物語性のあるNSFWプロンプト。推奨モデル：**Seedance v1.5 Pro**、**Kling v3.0 Pro**、**Wan 2.6**。

### CN-01 〜 CN-10

英語版と同一の10本の映画的ナラティブプロンプト。[英語版カテゴリ7](./README.md#category-7-cinematic--narrative-10-prompts)をご参照ください。

---

## カテゴリ8：フェティッシュ＆ニッチ（10本）

特定の美的嗜好に特化したコンテンツ。推奨モデル：**Wan 2.2 Spicy**、**Wan 2.5**。

### FN-01 〜 FN-10

英語版と同一の10本のフェティッシュプロンプト。[英語版カテゴリ8](./README.md#category-8-fetish--niche-10-prompts)をご参照ください。

---

## モデル別最適化ガイド

### Wan 2.2 Spicy — エクスプリシットコンテンツに最適（$0.03/秒から）

| 設定 | 推奨値 | 理由 |
|:-----|:-------|:-----|
| 解像度 | 720p | 品質/速度の最適バランス |
| 再生時間 | 5秒 | 8秒では品質が大幅に低下 |
| プロンプト長 | 40–80語 | 短い = アーティファクト少ない |
| I2V vs LoRA | リアル系はI2V、スタイライズはLoRA | LoRAはスタイルを追加するが品質がわずかに低下 |

**Spicyプロンプトのコツ：**
- アクションから始める、シーンからではない：「She removes her dress...」であり「In a bedroom with oak furniture...」ではない
- 必ず含める：「consistent body proportions, no distortion, no morphing」
- カメラアングルは1つだけ指定 — 複数アングルはモデルを混乱させる
- 効果的な肌の照明キーワード：「warm key light」「soft diffused」「golden hour」

### Wan 2.5/2.6 — 高品質ヌードのコスパ最強（$0.05–$0.07/秒から）

| 設定 | 推奨値 | 理由 |
|:-----|:-------|:-----|
| 解像度 | 720p–1080p | 2.6では1080pの価値あり |
| 再生時間 | 5–10秒 | 長いクリップの処理が得意 |
| プロンプト長 | 60–120語 | Spicyより多くのディテールを活用 |
| モード | I2V | T2VよりNSFWコンプライアンスが高い |

**Wan 2.5/2.6のコツ：**
- 芸術的なフレーミング言語を使用：「fine art photograph」「museum-quality figure study」
- ヌードをポルノグラフィック用語ではなく、臨床的/芸術的用語で記述
- 2.6の得意分野：アーティスティックヌード、ボディランドスケープ、美術

### Seedance v1.5 Pro — プレミアムシネマティック品質（$0.044/秒から）

| 設定 | 推奨値 | 理由 |
|:-----|:-------|:-----|
| 解像度 | 720p | 現在唯一のオプション |
| 再生時間 | 5–15秒 | 長いクリップの処理が卓越 |
| プロンプト長 | 80–150語 | 詳細な記述で最良の結果 |
| アクセス | NSFWホワイトリスト必要 | Atlas Cloudで申請 |

**Seedanceのコツ：**
- 環境の詳細な記述に投資 — Seedanceは環境描画が非常に優秀
- カメラムーブメントを指定：「slow dolly in」「tracking shot」「crane shot from above」
- 最適用途：ランジェリー、アーティスティックヌード、ファンタジー、シネマティックナラティブ

### Vidu Q3-Pro — 品質/価格バランス（$0.06/秒から）

| 設定 | 推奨値 | 理由 |
|:-----|:-------|:-----|
| 解像度 | 720p–1080p | どちらも良好 |
| 再生時間 | 5–10秒 | 時間的一貫性が良好 |
| プロンプト長 | 50–100語 | 簡潔なプロンプトが最適 |
| アクセス | NSFWホワイトリスト必要 | Atlas Cloudで利用可能 |

### Kling v3.0 Pro — 最高の顔品質（$0.204/秒から）

| 設定 | 推奨値 | 理由 |
|:-----|:-------|:-----|
| 解像度 | 最大1080p | 高解像度 = より良い顔 |
| 再生時間 | 5–10秒 | 時間的一貫性が良好 |
| プロンプト長 | 60–120語 | 詳細な顔の記述が最も効果的 |
| アクセス | NSFWホワイトリスト必要 | Atlas Cloudで利用可能 |

---

## 高度なプロンプトテクニック

### テクニック1：時間シーケンシング

プロンプトをタイムラインとして構造化し、より一貫したモーションを実現：

```
ビート1 (0-2秒): [開始状態 — 視聴者が最初に見るもの]
ビート2 (2-4秒): [遷移 — 主要なアクションまたは変化]
ビート3 (4-5秒): [終了状態 — 最終フレーム]
```

### テクニック2：参照画像戦略

I2Vモデルでは、参照画像が結果の60%を決定します：

- **顔のクリアさ**：明確で十分な照明、望ましい表情
- **ポーズの基礎**：開始ポーズはプロンプトの冒頭状態と一致させる
- **照明の一致**：画像の照明はプロンプトの照明記述と一致させる
- **衣装の一致**：脱衣を含むプロンプトは、画像に開始衣装を表示
- **解像度**：高解像度の参照画像 = より良い出力（最低1024x1024）

### テクニック3：反復的な改良ワークフロー

低コストでテストし、段階的にスケールアップ：

1. **ドラフト**：Wan 2.2 Spicy ($0.03) — コアコンセプトをテスト
2. **改良**：Wan 2.5 ($0.05) — 視覚品質の向上を確認
3. **最終版**：Seedance/Kling ($0.20+) — 洗練された最終バージョンを制作

このワークフローでは3回の生成で$0.28、プレミアムモデルから始めた場合の$0.60+と比較して大幅に節約。

---

## バッチ生成スクリプト

複数プロンプトの効率的なバッチ生成スクリプトについては、[英語版バッチ生成スクリプト](./README.md#batch-generation-script)をご参照ください。

コードコメントは英語で、そのままコピーして使用できます。

---

## よくある質問

### どのモデルを使うべきですか？

| ニーズ | 最適モデル | 料金 | 理由 |
|:-------|:---------|:-----|:-----|
| エクスプリシットな性的コンテンツ | Wan 2.2 Spicy | $0.03 | 唯一ほぼ100%のエクスプリシットコンプライアンス |
| 高品質アーティスティックヌード | Wan 2.6 | $0.07 | 非エクスプリシットNSFWの品質/価格の王者 |
| プレミアムシネマティック品質 | Seedance v1.5 Pro | $0.222 | 最高のモーションと環境描画 |
| 最高の顔描画 | Kling v3.0 Pro | $0.204 | 顔のディテールと表情で他を圧倒 |
| 予算限定でも品質重視 | Vidu Q3-Pro | $0.06 | 品質と価格の良いバランス |
| アニメ/スタイライズ | Wan 2.2 Spicy LoRA | $0.03 | アニメLoRAでスタイライズ出力 |
| テスト/プロトタイプ | Wan 2.2 Spicy | $0.03 | 最も安いイテレーション |

### 全115本のプロンプトを生成するといくらですか？

| モデル | 1回の料金 | 全115本 | 備考 |
|:-------|:---------|:--------|:-----|
| Wan 2.2 Spicy | $0.03 | **$3.45** | 最もお得、全カテゴリ対応 |
| Wan 2.5 | $0.05 | $5.75 | エクスプリシットの約30%が拒否 |
| Vidu Q3-Pro | $0.06 | $6.90 | ほとんどのエクスプリシットが拒否 |
| Wan 2.6 | $0.07 | $8.05 | エクスプリシットの約60%が拒否 |
| Kling v3.0 Pro | $0.204 | $23.46 | 高品質、限定的エクスプリシット |
| Seedance v1.5 Pro | $0.222 | $25.53 | 高品質、限定的エクスプリシット |

**25%初回チャージボーナスでSpicyで全プロンプトをテスト：**
$3.00チャージ → $3.75のクレジット取得 → 全115本を生成して$0.30残り。

### NSFWホワイトリストアクセスの取得方法は？

[Atlas Cloud](https://www.atlascloud.ai?ref=JPM683)で登録し、クレジットをチャージ後、ダッシュボードまたはサポートを通じてNSFWホワイトリストアクセスを申請してください。確認済みアカウントは通常24時間以内に承認されます。

---

## 利用開始

<div align="center">

### NSFW AIビデオ生成、最低$0.03から

**[Atlas Cloud](https://www.atlascloud.ai?ref=JPM683)** — SOC I & II認証 | HIPAA準拠 | 米国法人

1. [アカウント作成](https://www.atlascloud.ai?ref=JPM683)
2. クレジットチャージ（初回チャージで25%ボーナス、最大$100）
3. APIキーをコピー
4. 本コレクションの任意のプロンプトを使用

[![利用開始](https://img.shields.io/badge/今すぐ始める-Atlas_Cloud-blue?style=for-the-badge)](https://www.atlascloud.ai?ref=JPM683)

</div>

---

## Star履歴

<div align="center">

[![Star History Chart](https://api.star-history.com/svg?repos=thoughtincode/nsfw-ai-video-prompts&type=Date)](https://star-history.com/#thoughtincode/nsfw-ai-video-prompts&Date)

</div>

---

## コントリビュート

コントリビューション歓迎！優れた結果を生むNSFWビデオプロンプトをお持ちの方は、PRを提出してください。ガイドライン：

1. テストしたモデルと結果の品質を含める
2. 適切にカテゴリ分けする
3. 十分な詳細を提供（最低3文）
4. 既存プロンプトのフォーマットパターンに従う
5. 合法的な成人コンテンツのみ — 未成年者、非合意シナリオ、違法コンテンツは絶対に禁止

---

## ライセンス

MITライセンス。詳細は[LICENSE](./LICENSE)をご覧ください。

プロンプトは自由に使用、変更、配布できます。生成されたコンテンツは使用プラットフォームの利用規約に従います。

---

<div align="center">

**[Atlas Cloud](https://www.atlascloud.ai?ref=JPM683)がクリエイティブコミュニティのために制作**

*世界で最も手頃なNSFW AIビデオ生成プラットフォーム。*

</div>
