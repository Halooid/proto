# Halooid Contracts (Proto)

## Purpose
This repository acts as the single source of truth for all gRPC Protobuf definitions used across the Halooid ecosystem. It ensures backend microservices, gateways, and mobile applications communicate using strictly defined, backward-compatible schemas.

## Responsibilities
- Definitions for all gRPC APIs and message types.
- Ensure strict additive backward compatibility.
- Decouple schema from implementation.

## Tech Stack
- Protocol Buffers (proto3)
- Buf (for linting and module management)

## Dependencies
- None. This is the root dependency for all services.

## How to Run / Build
To lint the definitions, run:
```bash
buf lint
```

> **Note**: Stubs and generated code are intentionally omitted from this repository. All consumer repositories must generate code locally using tools like `buf.gen.yaml`.

## Key Flows
- Defining API boundaries for services.
- Providing standardized representations across web, mobile, and backend nodes.

## Documentation Index
- See `.agents/rules/grpc-proto-guidelines.md` for specific proto change requirements.
