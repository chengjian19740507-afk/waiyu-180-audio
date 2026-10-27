# waiyu-180-audio

《出境无忧180句》离线发音音频库。

- 13 语种 × 180 句 = 2340 个 mp3
- 引擎：macOS 内置 TTS（`say`），零成本、零 API key
- 格式：mp3 / 48kbps / 22.05kHz 单声道
- 目录：`audio/<lang>/<id>.mp3`，`manifest.json` 为句 ID → 原文映射

## 用途

| 端 | 说明 |
|---|---|
| 网页版 | `waiyu-180-app` 在浏览器 SpeechSynthesis 不可用（微信内置浏览器）时的降级发音 |
| 小程序版 | 待接入（需云开发/备案域名，见主仓 README） |

## 重新生成

```
cd waiyu-180-app && python3 scripts/gen_audio.py --out ../waiyu-180-audio --jobs 8
```

## 许可

音频基于 CC BY-NC 4.0 数据（`LICENSE-DATA`）派生，仅限非商业使用。
