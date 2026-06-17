---
name: lakehq__sail__pyspark-skill
source: https://github.com/lakehq/sail/blob/7a34be78a9cfac9446fa5459669c449c6be19c73/docs/guide/integrations/_code/pyspark-skill.md
repo: lakehq/sail
kind: skill
stars: 2955
last_pushed: 2026-06-15T03:40:48Z
license: apache-2.0
score: 7
domains: [data-engineering, cli-tools]
tags: [pyspark, sail, distributed-computing]
curated: 2026-06-15
curated_by: config-scout
---

# lakehq/sail — skill

**Why it's worth keeping:** Offers multiple execution patterns (piping, heredocs, and file paths) which are crucial for an agent to know when handling multi-line code snippets via shell.

**Summary:** Provides instruction on executing PySpark scripts through the Sail distributed compute engine using various CLI input methods.

**Source credibility:** High; source repository is well-starred (2955 stars) and actively maintained.

**Recency:** Current; documentation reflects a modern, active project.

**Source:** [lakehq/sail/docs/guide/integrations/_code/pyspark-skill.md](https://github.com/lakehq/sail/blob/7a34be78a9cfac9446fa5459669c449c6be19c73/docs/guide/integrations/_code/pyspark-skill.md) · 2955★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: run-pyspark-script
description: Runs a PySpark script.
---

You can run PySpark scripts via the `sail spark run` command.

Sail is an open-source unified and distributed multimodal computation framework
that can be used as a drop-in replacement for Apache Spark.
By using Sail to run PySpark scripts, you can perform data processing tasks
with the familiar PySpark DataFrame API or Spark SQL while benefiting from
the high performance and low memory overhead of Sail.

The script can refer to the Spark session via the `spark` variable, which
connects to a local Sail server via the Spark Connect protocol.
The Sail server starts instantly when you run the `sail spark run` command,
and it will be automatically stopped after the script finishes.

You can pipe simple PySpark code to the `sail spark run` command directly:

```bash
echo 'spark.sql("SELECT 1 + 1").show()' | sail spark run 2>/dev/null
```

Alternatively, you can use a heredoc for more complex PySpark scripts:

```bash
cat <<EOF | sail spark run 2>/dev/null
import pyspark.sql.functions as F

df = spark.createDataFrame([(1, 2), (2, 3)], ["a", "b"])
df = df.withColumn("sum", F.col("a") + F.col("b"))
df.show()
EOF
```

You
```

</details>
