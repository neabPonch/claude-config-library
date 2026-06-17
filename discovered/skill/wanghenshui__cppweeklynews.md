---
name: wanghenshui__cppweeklynews
source: https://github.com/wanghenshui/cppweeklynews/blob/d03119bf191e561ad9a0e3488f0c14bb06ab0212/SKILL.md
repo: wanghenshui/cppweeklynews
kind: skill
stars: 548
last_pushed: 2026-05-23T14:54:46Z
license: cc0-1.0
score: 9
domains: [systems-programming, performance-optimization, cpp]
tags: [modern-cpp, optimization, safety, patterns]
curated: 2026-06-15
curated_by: config-scout
---

# wanghenshui/cppweeklynews — skill

**Why it's worth keeping:** Provides actionable 'bad vs good' code snippets for advanced features like deducing this and std::expected; includes deep low-level optimization strategies regarding TLS and memory layout.

**Summary:** A high-density technical reference for modern C++ development, covering C++20/23 idioms, performance optimization, and UB prevention.

**Source credibility:** High; content is curated from a widely recognized specialized C++ newsletter with strong community engagement.

**Recency:** Extremely current, featuring state-of-the-art C++20 and C++23 standards.

**Source:** [wanghenshui/cppweeklynews/SKILL.md](https://github.com/wanghenshui/cppweeklynews/blob/d03119bf191e561ad9a0e3488f0c14bb06ab0212/SKILL.md) · 548★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# C++ 开发技能指南

> 本文档从 C++ 中文周刊（第1期~第196期）中提炼的编码规范、设计模式、性能优化和避坑指南。
> 适用于日常 C++ 开发参考。

---

## 一、现代 C++ 编码规范

### 1.1 优先使用 range-based for 和 Ranges 库

传统 for 循环"过于灵活"，容易引入 off-by-one、修改错误变量等 bug。编译器无法防止这些问题。

```cpp
// ❌ 经典错误
for (auto i = 0; i <= vec.size(); ++i)   // 应该是 <
  use(vec[i]);

for (auto i = vec.size() - 1; i >= 0; --i)  // 无符号数永远 >= 0，死循环！
  use(vec[i]);

// ✅ 现代写法
for (auto const& rec : records)
  use(rec);

// 反向迭代（C++20）
for (auto const& rec : std::views::reverse(records))
  use(rec);

// 带索引迭代（C++23）
for (auto [i, rec] : std::views::enumerate(records))
  use(i, rec);

// 多序列同时迭代（C++23）
for (auto [name, rec] : std::views::zip(names, records))
  use(name, rec);
```

*来源：第190期*

### 1.2 用 `std::source_location` 替代 `__FILE__` / `__LINE__` 宏

```cpp
// ❌ 传统宏方法
#define ASSERT(cond, msg) Assert(cond, msg, __FUNCTION__, __LINE__)

// ✅ C++20
void Assert(bool condition, std::string_view msg,
            std::source_location loc = std::source_location::current()) {
  if (!condition) {
    std::clog << loc.function_name() << ':' << loc.line() << ": " << msg << '\n';
  }
}
// 调用时不需要宏：
Assert(1 != 2, "Not met");
```

关键：`std::source_location::current()` 作为默认参数，在调用侧求值。

*来源：第190期*
```

</details>
