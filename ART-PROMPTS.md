# 星星小游戏 · 美术素材清单（给 GPT / 绘图模型用）

> 主会场（img/scene.jpg）那套已经定调了：**深蓝夜空 + 暖金色灯光 + 奶油白 + 星形点缀 + 微光柔焦**。
> 游戏里所有素材都往这套靠，别换画风，不然接上去会像两个游戏拼起来的。

## 全局画风关键词（每条提示词都带上这段）

```
2D side-scrolling platformer game art, soft hand-painted storybook style,
warm golden rim light, deep indigo night sky, cream and pale blue palette,
star and moonlight motifs, gentle bloom, cozy birthday atmosphere,
clean readable silhouette, no text, no watermark
```

---

## 1. 主角（img/player.png）

透明底 PNG，256×256（游戏里会缩到 28×40 显示），**正面朝右站立**。

```
A tiny cute chibi girl mascot for a platformer, roughly 3 heads tall,
round pale face, two big dark friendly eyes, tiny pink blush,
short fluffy pink-white hair, wearing a soft pink dress/overall,
small rounded feet, simple thick outline, flat cel shading,
full body, standing facing right, slight smile,
transparent background, centered, no shadow, no text
```

- 关键：**轮廓要简单**，缩小到 28px 还要认得出。别加细节、别加道具。
- 想给她换装就改 dress 那句（粉色连衣裙 / 白毛衣 / 深蓝大衣都行）。

---

## 2. 蘑菇怪 · 四种（img/mob-walk.png / mob-hop.png / mob-armor.png / mob-fly.png）

统一：透明底 PNG，256×256，**侧面朝右**，脚下对齐画布底部。

共同前缀：

```
Cute round mushroom creature enemy for a platformer, side view facing right,
single mushroom cap with visible short legs, big friendly-but-mischievous eyes,
thick outline, flat cel shading, game sprite, transparent background,
character sits on the bottom edge of the canvas, no shadow, no text
```

| 文件 | 追加描述 |
|---|---|
| `mob-walk.png` | `red-coral cap with pale cream spots, calm walker, small and harmless looking` |
| `mob-hop.png` | `warm orange cap with cream ring spots, springy legs, looks like it's mid-bounce` |
| `mob-armor.png` | `steel-grey cap with a riveted metal band across it, slightly bigger and heavier, tough looking` |
| `mob-fly.png` | `soft violet cap, two small translucent pale wings on its sides, floating off the ground` |

- 四只**大小要一致**（同一个画布、同一个角色比例），否则摆在一起会怪。
- 铁头菇那只要能看出「踩一下会裂」的气质——金属压条是关键。

---

## 3. 低天花板（img/ceiling.png）

**横向无缝平铺**，高度 40–120px 都行，宽度随意。**不要画刺**（刺是代码画的，会叠在底边）。

```
Seamless horizontal tile of a stone cave ceiling underside, seen from below,
dark slate blue-grey rock, subtle cracks and moss patches,
soft bottom edge with faint shadow, painterly, muted,
left and right edges must tile seamlessly, no spikes, no text
```

---

## 4. 云台（img/cloud.png）

透明底 PNG，横图（比如 512×192）。游戏会横向拉伸到平台宽度（150–440px）。

```
A soft fluffy floating cloud platform, side view, pure white top surface
with pale blue shadow underneath, gentle rounded bumps, dreamy storybook look,
transparent background, isolated object, no ground, no text
```

- 重点是**顶面要平**——它是要站人的，别画成尖顶。

---

## 5. 游戏背景（img/bg-game.jpg）—— 可选，但效果最大

16:9 横图，最小 1920×1080。**不要画地面和角色**，只要天和远景（地面是代码画的）。

```
Horizontal parallax background for a cozy 2D platformer, 16:9,
deep indigo night sky with a crescent moon and scattered stars,
distant rolling hills silhouettes in soft blue-green,
a few warm string lights and tiny distant lanterns glowing,
rolling mist near the horizon, painterly storybook style,
warm golden bloom, no ground, no characters, no text
```

- **底部留出约 1/3 的平坦区域**（会被地面和前景盖住），别把重要内容放那儿。
- 和主会场 scene.jpg 同一个调子——那两张要能连成一个世界。

---

## 放哪儿

全部丢进 `birthday-site/img/`，文件名严格照上表。放好之后跟我说一声，我重新部署一次就会替换（没放的会自动保留现在代码画的版本，不会白屏）。
