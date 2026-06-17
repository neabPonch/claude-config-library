---
name: ttskch__audio2video
source: https://github.com/ttskch/audio2video/blob/7bc00a1ffa0c403fcdfeddb57c23ba86d3e8459e/CLAUDE.md
repo: ttskch/audio2video
kind: claude-md
stars: 6
last_pushed: 2026-02-23T01:14:34Z
license: mit
score: 8
domains: [web-app, media-processing]
tags: [php, symfony, ffmpeg, fullstack]
curated: 2026-06-16
curated_by: config-scout
---

# ttskch/audio2video — claude-md

**Why it's worth keeping:** It explicitly documents critical 'hidden' constraints (e.g., the 140s duration limit) and exact service configurations which are essential for preventing AI-generated logical errors in legacy systems.

**Summary:** A high-density technical blueprint that maps out architecture, dependency injection patterns, and specific business logic flows.

**Source credibility:** Small personal utility project with moderate maintenance history.

**Recency:** The tech stack is aging, but the documentation structure is a gold standard for instructing modern agents on complex/legacy codebases.

**Source:** [ttskch/audio2video/CLAUDE.md](https://github.com/ttskch/audio2video/blob/7bc00a1ffa0c403fcdfeddb57c23ba86d3e8459e/CLAUDE.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# audio2video 開発者ガイド

## プロジェクト概要

音声ファイル（mp3等）を静止画付きの動画ファイル（mp4等）に変換するWebアプリケーション。
Twitter/FacebookなどSNSへの音声投稿ができない問題を解決するためのツール。
本番URL: http://audio2video.me
CLI版: [ttskch/audio2video-cli](https://github.com/ttskch/audio2video-cli)

## 技術スタック

### バックエンド
- **PHP** 7.1.3+
- **Symfony** 4.x（MicroKernelTrait使用のマイクロカーネル構成）
- **SensioFrameworkExtraBundle** 5.x（`@Route`, `@Template` アノテーション）
- **Symfony Form** / **Validator** / **Translation** / **Process**
- **テスト**: PHPUnit（Symfony PHPUnit Bridge経由、`bin/phpunit`）

### フロントエンド
- **Webpack Encore** 0.17（Symfony公式Webpackラッパー）
- **jQuery** 3.x + **Bootstrap** 4 + **Popper.js**
- **Select2**（Bootstrap4テーマ付き: `@ttskch/select2-bootstrap4-theme`）
- **Font Awesome** 4.x
- **is-loading**（フォーム送信時のオーバーレイ表示）
- **SCSS**（node-sass + sass-loader）
- **PostCSS**（autoprefixer）

### 外部ツール（サーバー側）
- **FFmpeg** / **FFprobe**: 音声→動画変換の中核処理
- **ImageMagick** + **Imagick PHP拡張**: ブランク画像の生成

### インフラ
- **Docker**: Alpine Linux ベース（`ttskch/nginx-php-fpm-heroku` イメージ）
- **Nginx** + **PHP-FPM** 構成
- **Heroku**: Container Registry経由のデプロイ
- **GitHub Actions**: mainブランチへのプッシュでDockerイメージをビルド→Herokuへデプロイ

## ディレクトリ構成

```
├── assets/                  # フロントエンドソース
│
```

</details>
