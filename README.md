# testmodeler

**mini-AI v0.3** の GGUF 置き場です（ゼロから学習した超小型日本語チャットモデル）。

## モデル

| 項目 | 値 |
|------|-----|
| ファイル | `mini-ai-v0.3-f16.gguf` |
| サイズ | 約 2.2 MB (f16) |
| パラメータ | ~0.96M |
| アーキテクチャ | Llama (RMSNorm + RoPE + SwiGLU) |
| トークナイザ | 文字レベル |
| context | 128 |

## ダウンロード

ファイルをこのリポジトリの root に置いたあと:

```text
https://github.com/kubobeem/testmodeler/raw/main/mini-ai-v0.3-f16.gguf
```

または Releases から取得してください。

## 使い方

- ブラウザデモ: [kubobeem/groktest](https://github.com/kubobeem/groktest)
- llama.cpp / LM Studio / Ollama でも読み込み可能

## プロンプト形式

```
質問：ねこの鳴き声は？
答え：
```

## アップロード手順（手元の gguf を置く）

```bash
git clone https://github.com/kubobeem/testmodeler.git
cd testmodeler
cp /path/to/mini-ai-v0.3-f16.gguf .
git add mini-ai-v0.3-f16.gguf
git commit -m "Add mini-ai-v0.3-f16.gguf"
git push
```

GitHub Web UI でも「Add file → Upload files」で 2.2MB の GGUF を直接アップロードできます。
