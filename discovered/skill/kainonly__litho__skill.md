---
name: kainonly__litho__skill
source: https://github.com/kainonly/litho/blob/e32000eddc5dcc71cf8c3ee1a988925294ff7ef8/.llms/skills/angular/skill.md
repo: kainonly/litho
kind: skill
stars: 20
last_pushed: 2026-04-10T01:37:09Z
license: bsd-3-clause
score: 7
domains: [web-frontend, typescript]
tags: [angular, signals, modern-web]
curated: 2026-06-15
curated_by: config-scout
---

# kainonly/litho — skill

**Why it's worth keeping:** It effectively steers LLMs away from legacy RxJS/class-based patterns by prioritizing Signal-based inputs, outputs, and modern template structures.

**Summary:** Provides high-density technical grounding for Angular 21, specifically emphasizing modern paradigms like Signals and the new control flow syntax.

**Source credibility:** Derived from official Angular documentation (angular.dev).

**Recency:** Highly current; aligns with the latest Angular 21 standards.

**Source:** [kainonly/litho/.llms/skills/angular/skill.md](https://github.com/kainonly/litho/blob/e32000eddc5dcc71cf8c3ee1a988925294ff7ef8/.llms/skills/angular/skill.md) · 20★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Angular 21 LLM 上下文
# 来源: https://angular.dev/llms.txt

## 框架概述
Angular 是一个用于构建现代 Web 应用程序的开发框架，让开发更有信心。
当前版本: Angular 21

## 核心概念

### 组件 (Components)
- 组件是 Angular 应用程序的主要构建块
- 使用独立组件 standalone components（Angular 21 默认）
- 组件装饰器: @Component({ selector, template/templateUrl, styles/styleUrls })
- 使用 input() 函数创建基于信号的输入
- 使用 output() 函数创建基于信号的输出

### 模板 (Templates)
- 使用 Angular 模板语法和插值表达式 {{ }}
- 属性绑定: [property]="value"
- 事件绑定: (event)="handler()"
- 双向绑定: [(ngModel)]="value"
- 控制流: @if, @else, @for, @switch (新的块语法)
- 模板引用变量: #ref

### 指令 (Directives)
- 结构型指令改变 DOM 布局 (@if, @for, @switch)
- 属性型指令改变元素外观/行为
- 使用 @Directive 装饰器创建自定义指令

### 信号 (Signals)
- 用于状态管理的响应式原语
- signal() 创建可写信号
- computed() 创建派生信号
- effect() 创建副作用
- 尽可能使用信号代替 RxJS，实现更简单的响应式

### 依赖注入 (Dependency Injection)
- 分层注入系统
- @Injectable({ providedIn: 'root' }) 用于单例服务
- inject() 函数用于注入依赖
- 注入令牌 (Injection tokens) 用于非类依赖

### HTTP 客户端 (HTTP Client)
- 使用 HttpClient 发起 HTTP 请求
- 使用 withInterceptors() 创建函数式拦截器
- 类型安全的请求/响应处理
- withFetch() 使用原生 fetch API

### 表单 (Forms)
- 响应式表单: FormGroup, FormControl, FormArray
- 模板驱动表单: ngModel
- 使用 Validators 进行表单验证
- 自定义验证器和异步验证器

### 路由 (Routing)
- 独立路由配置
- 路由守卫: CanActivate, CanDeacti
```

</details>
