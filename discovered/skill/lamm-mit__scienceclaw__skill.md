---
name: lamm-mit__scienceclaw__skill
source: https://github.com/lamm-mit/scienceclaw/blob/f4a628669d1bcf9702cf29d068716c02f1c9268f/skills/motif-clustering/SKILL.md
repo: lamm-mit/scienceclaw
kind: skill
stars: 221
last_pushed: 2026-05-29T14:26:16Z
license: apache-2.0
score: 7
domains: [data-science, musicology, cli-tools]
tags: [clustering, scikit-learn, statistical-analysis]
curated: 2026-06-15
curated_by: config-scout
---

# lamm-mit/scienceclaw — skill

**Why it's worth keeping:** Demonstrates an excellent pattern of defining specific CLI arguments and returning highly structured, statistically enriched JSON outputs that are easy for an agent to parse.

**Summary:** Provides a scientific tool for clustering melodic motifs using statistical methods like KMeans or hierarchical clustering.

**Source credibility:** Strong; comes from a specialized research-oriented repository (lamm-mit).

**Recency:** Current; utilizes modern scikit-learn and music21 workflows.

**Source:** [lamm-mit/scienceclaw/skills/motif-clustering/SKILL.md](https://github.com/lamm-mit/scienceclaw/blob/f4a628669d1bcf9702cf29d068716c02f1c9268f/skills/motif-clustering/SKILL.md) · 221★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# motif-clustering

Clusters melodic motifs using scikit-learn (KMeans or hierarchical clustering) with optional UMAP projection. Takes motif JSON (from motif-detection) and groups them by interval similarity.

## Usage

```bash
python3 skills/motif-clustering/scripts/motif_clustering.py --query "bach motifs" --n-clusters 8 --method kmeans
python3 skills/motif-clustering/scripts/motif_clustering.py --query "bach motifs" --method hierarchical
```

## Output

```json
{
  "method": "kmeans",
  "n_clusters": 8,
  "clusters": [
    {
      "cluster_id": 0,
      "n_members": 12,
      "centroid_intervals": [2, -1, 2],
      "genre_distribution": {"baroque": 8, "folk": 4},
      "top_motifs": ["m_0001", "m_0012"]
    }
  ],
  "silhouette_score": 0.47,
  "inertia": 234.5
}
```

## Dependencies

- scikit-learn
- music21
```

</details>
