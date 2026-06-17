---
name: ZijingWu-MTH__MyEnv
source: https://github.com/ZijingWu-MTH/MyEnv/blob/b351d70f62c1a23a0eda80150b6e21000f303081/CLAUDE.md
repo: ZijingWu-MTH/MyEnv
kind: claude-md
stars: 1
last_pushed: 2026-06-11T06:48:40Z
license: unknown
score: 8
domains: [cpp, dart, cross-platform]
tags: [debugging-protocol, workflow-rules, build-system, error-handling]
curated: 2026-06-15
curated_by: config-scout
---

# ZijingWu-MTH/MyEnv — claude-md

**Why it's worth keeping:** It defines excellent debugging protocols (adding DEBUG tags for human review), architectural constraints (tasklet patterns), and explicit instructions on how the AI should interact with the developer via confirmation loops.

**Summary:** A highly specific technical guide for a C++/Dart cross-platform project covering custom build systems, error handling macros, and memory management. It establishes a strict 'investigation-first' workflow to minimize incorrect code changes.

**Source credibility:** Low star count suggests a private or niche personal repository, but the technical depth is high.

**Recency:** Current; reflects modern workflows involving AI-assisted debugging and custom build scripts.

**Source:** [ZijingWu-MTH/MyEnv/CLAUDE.md](https://github.com/ZijingWu-MTH/MyEnv/blob/b351d70f62c1a23a0eda80150b6e21000f303081/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## 1. Common information
- Our project will generate some header/java/python file in obj folder. The obj folder is in the same level as the project root folder. For example the source folder in ~/source_code/bj-media4 the object root folder can be ~/source_code/mac-obj-media4 for mac platform build. The obj folder structure is much the same as src folder.
- The ${OBJROOT}/xplatform_util-src/xplatform_util/error_handling_template.h contains the error handling common code. In the macro name RTV means return void. RTN means return with an value. RFE means return an error feature. And AL means alarm. AS means assert. 5M/5S means 5 minutes interval or 5 seconds interval for alarm. You should generate code as with CHECK_RESULT_xxxx as much as possible. So error can be easily catched. Especially for the data or logic which will not happen in real environment, most likely will be a bug.
- Please avoid to search the code in thirdparty-src folder, it is public opensource thirdparty code, and the code base is huge and slow for search.
- Read the xplatform_util-src/xplatform_util/async/cancellable.h for how to use FutureRef and CancellableSet.
- Use namespace xu as short alias of namespace xpl
```

</details>
