# Auditory C/D ratio — pseudo-weight prototype

高さ h [cm] に応じて音高を Δp = ±g·h [半音] だけ変える実験用プロトタイプ（f₀ = 440 Hz、正弦波）。

https://eisuke29.github.io/sound-cd-weight/ （`#demo` で自動デモ）

- 手法：カメラ（MediaPipe Hand Landmarker）／置いたスマホ（手の大きさから距離を推定）／センサー（DeviceMotion）／デモ
- g：0.05, 0.1, 0.2, 0.4, 0.8 [st/cm]、方向 ±、発音条件 移動時／常時、ゼロ点設定、ブラインド
- 表示：h, Δp, f の数値、h(t)・Δp(t) の時系列（8 s）、Δp = g·h の写像図
- 試行ログ：h が 5 cm 超 → 2 cm 未満に戻るまでを1試行として自動記録（CSVコピー可）
- キー：← → / 1–5 g、Space ゼロ点、Enter ブラインド、R g乱数（非表示）、A 開示、D 方向、M 発音条件

ファイルは `index.html` 1つのみ。
