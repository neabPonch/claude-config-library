---
name: ngxtm__devkit__skill
source: https://github.com/ngxtm/devkit/blob/9439f27ce3fa7fe53ff9278a1ee9a44bffa70eba/rules/golang/grpc/SKILL.md
repo: ngxtm/devkit
kind: skill
stars: 7
last_pushed: 2026-02-28T04:39:21Z
license: mit
score: 9
domains: [backend-api, golang]
tags: [grpc, go, protobuf]
curated: 2026-06-16
curated_by: config-scout
---

# ngxtm/devkit — skill

**Why it's worth keeping:** The metadata triggers allow an AI to automatically apply these patterns when encountering .proto files; the examples include essential production-ready details like interceptor chaining and status-based error handling.

**Summary:** Provides comprehensive implementation standards for Go gRPC, covering proto definitions, server/client logic, interceptors, and error handling.

**Source credibility:** Niche tool with a specialized multi-agent focus, though relatively low star count.

**Recency:** Highly relevant as gRPC/Go standards are stable and current.

**Source:** [ngxtm/devkit/rules/golang/grpc/SKILL.md](https://github.com/ngxtm/devkit/blob/9439f27ce3fa7fe53ff9278a1ee9a44bffa70eba/rules/golang/grpc/SKILL.md) · 7★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: Go gRPC
description: High-performance RPC framework with Protocol Buffers.
metadata:
  labels: [golang, grpc, protobuf, rpc]
  triggers:
    files: ['**/*.proto', '**/*_grpc.pb.go']
    keywords: [grpc, proto, RegisterServer, NewClient]
---

# Go gRPC Standards

## Proto Definition

```protobuf
// proto/user.proto
syntax = "proto3";
package user;
option go_package = "myapp/gen/user";

service UserService {
    rpc GetUser (GetUserRequest) returns (User);
    rpc ListUsers (ListUsersRequest) returns (stream User);
    rpc CreateUsers (stream CreateUserRequest) returns (CreateUsersResponse);
    rpc Chat (stream Message) returns (stream Message);
}

message User {
    int64 id = 1;
    string name = 2;
    string email = 3;
}

message GetUserRequest {
    int64 id = 1;
}

message ListUsersRequest {
    int32 page_size = 1;
    string page_token = 2;
}
```

## Code Generation

```bash
# Install
go install google.golang.org/protobuf/cmd/protoc-gen-go@latest
go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@latest

# Generate
protoc --go_out=. --go-grpc_out=. proto/user.proto
```

## Server Implementation

```go
type userServer struct {
    pb.UnimplementedUserServiceSe
```

</details>
