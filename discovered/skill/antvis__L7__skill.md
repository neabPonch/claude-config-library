---
name: antvis__L7__skill
source: https://github.com/antvis/L7/blob/ab05df605bd0e5d0d2a938461945405374d9381c/skills/l7/SKILL.md
repo: antvis/L7
kind: skill
stars: 4021
last_pushed: 2026-06-03T15:13:11Z
license: mit
score: 9
domains: [web-frontend, data-visualization, geospatial]
tags: [documentation-navigator, intent-mapping, map-api]
curated: 2026-06-15
curated_by: config-scout
---

# antvis/L7 — skill

**Why it's worth keeping:** Employs 'Intent-to-Documentation' mapping tables and 'Skill Combination Modes' which are elite patterns for teaching agents how to navigate large, multi-layered APIs.

**Summary:** A highly structured master index that maps user intents and complex workflows to specific documentation sub-modules.

**Source credibility:** High; AntV is a well-established visualization engine with significant GitHub traction.

**Recency:** Current; demonstrates modern knowledge-mapping techniques optimized for agentic workflows.

**Source:** [antvis/L7/skills/l7/SKILL.md](https://github.com/antvis/L7/blob/ab05df605bd0e5d0d2a938461945405374d9381c/skills/l7/SKILL.md) · 4021★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: antv-l7
description: |
  Comprehensive guide for AntV L7 geospatial visualization library. Use when users need to:
  (1) Create interactive maps with WebGL rendering
  (2) Visualize geographic data (points, lines, polygons, heatmaps)
  (3) Build location-based data dashboards
  (4) Add map layers, interactions, or animations
  (5) Process and display GeoJSON, CSV, or other spatial data
  (6) Integrate maps with AMap (GaodeMap), Mapbox, Maplibre, or standalone L7 Map
  (7) Optimize performance for large-scale geographic datasets
license: MIT
---

# AntV L7 Geospatial Visualization

AntV L7 是基于 WebGL 的大规模地理空间数据可视化引擎，支持多种地图底图和丰富的可视化图层类型。

## Quick Start

创建最简单的 L7 地图应用：

```javascript
import { Scene, PointLayer } from '@antv/l7';
import { GaodeMap } from '@antv/l7-maps';

// 1. 初始化场景
const scene = new Scene({
  id: 'map',
  map: new GaodeMap({
    center: [120.19, 30.26],
    zoom: 10,
    style: 'light',
  }),
});

// 2. 添加图层
scene.on('loaded', () => {
  const pointLayer = new PointLayer()
    .source(data, {
      parser: { type: 'json', x: 'lng', y: 'lat' },
    })
    .shape('circle')
    .size(10)
    .color('#5B8FF9');

  scene.addLayer(pointLayer);
});
```

## Core Wo
```

</details>
