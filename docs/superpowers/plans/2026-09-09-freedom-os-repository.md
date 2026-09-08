# Freedom OS Repository Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Codex, Claude, ChatGPT, Hermes가 공통으로 읽을 수 있는 Freedom OS Git 문서 저장소를 만든다.

**Architecture:** 전략·상태·도구 경계를 `docs/`에 두고, 에이전트 행동 규칙은 `agents/`, 데이터 계약은 `schemas/`에 분리한다. 실행 데이터와 장기 지식은 각각 Notion과 Obsidian에 남겨 Git 문서와 중복 관리하지 않는다.

**Tech Stack:** Markdown, Git

**Spec:** `docs/superpowers/specs/2026-09-09-freedom-os-repository-design.md`

## Global Constraints

- 미정 값은 `TBD`로 표시한다.
- 전략·상태·계약 정의는 한 곳에서만 정본으로 관리한다.
- 개인 금융·민감 정보는 초기 커밋에 저장하지 않는다.
- 초기 범위는 문서 Skeleton이며 실제 자동화 구현은 포함하지 않는다.

### Task 1: Repository Documentation Skeleton

**Files:**
- Create: `README.md`
- Create: `docs/*.md`
- Create: `agents/*.md`
- Create: `schemas/*.md`
- Create: `changelog/DECISIONS.md`
- Create: `.gitignore`

- [ ] Create the source-of-truth map and all referenced documents.
- [ ] Link each document to its authoritative parent instead of duplicating definitions.
- [ ] Mark unresolved values as `TBD`.

### Task 2: Structural Verification

**Files:**
- Verify: all Markdown and referenced paths

- [ ] Check every required path exists.
- [ ] Search for unresolved private values and accidental secrets.
- [ ] Check all internal Markdown links resolve.

### Task 3: Git Initialization

**Files:**
- Create: `.git/`

- [ ] Initialize Git in the project root if absent.
- [ ] Stage the new documentation.
- [ ] Create the first commit with a descriptive message.
