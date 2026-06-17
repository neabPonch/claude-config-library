---
name: catchpig__kmvvm
source: https://github.com/catchpig/kmvvm/blob/c23753fab181661e3359f4b8c19dc7d3c24ff09f/CLAUDE.md
repo: catchpig/kmvvm
kind: claude-md
stars: 117
last_pushed: 2026-05-25T13:20:43Z
license: apache-2.0
score: 9
domains: [android, kotlin, mobile-development]
tags: [mvvm, ksp, kotlin-flow, android]
curated: 2026-06-14
curated_by: config-scout
---

# catchpig/kmvvm — claude-md

**Why it's worth keeping:** The file provides exact code signatures for Flow extensions and critical warnings about KSP build requirements that would prevent common AI-generated build errors.

**Summary:** Defines strict architectural patterns for an Android MVVM framework including ViewModel/View lifecycle interactions and KSP annotation usage.

**Source credibility:** A specialized Android framework with significant community interest (117 stars).

**Recency:** Extremely current, leveraging modern standards like KSP and Version Catalogs.

**Source:** [catchpig/kmvvm/CLAUDE.md](https://github.com/catchpig/kmvvm/blob/c23753fab181661e3359f4b8c19dc7d3c24ff09f/CLAUDE.md) · 117★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 项目概述

kmvvm 是一个 Android Kotlin MVVM 架构框架，最低兼容 API 21。核心模块：

- **app**: 演示应用 (`com.catchpig.kmvvm`)
- **mvvm**: 核心框架库（BaseActivity/BaseVMActivity、BaseViewModel、Flow 扩展、网络封装）
- **annotation**: 注解定义（Title、ServiceApi、GlobalConfig、FlowError、Prefs 等）
- **compiler**: KSP 注解处理器
- **download**: 文件下载能力库
- **utils**: 通用扩展与工具

## 构建命令

```bash
# 编译 Debug 版本
./gradlew assembleDebug

# 编译 Release 版本
./gradlew assembleRelease

# 清理并重新编译（修改注解或 KSP 配置后必须用这个）
./gradlew clean assembleDebug

# 运行单元测试
./gradlew test

# 查看依赖树
./gradlew :app:dependencies
```

## 架构约定

### ViewModel 规范

- 继承 `com.catchpig.mvvm.base.viewmodel.BaseViewModel`
- 暴露数据用 `Flow<T>`，通过 `lifecycle*` 扩展收集
- Loading 状态通过 `BaseViewModel` 的 LiveData（`loadingDialogLiveData`、`loadingViewLiveData`）由 Activity/Fragment 统一处理，不直接持有 View/Context

```kotlin
fun queryBanners(): Flow<MutableList<Banner>> = repository.getBanners()
```

### Activity / Fragment 规范

- 有 ViewModel：`BaseVMActivity<VB, VM>` 或 `BaseVMFragment<VB, VM>`（泛型顺序：ViewBinding、ViewModel）
- 无 ViewModel：`BaseActivity<VB>` 或 `BaseFragment<VB>`
- 必须实现：`initParam()`、
```

</details>
