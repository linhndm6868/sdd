# SDD Project

Repository này được bootstrap theo `github/spec-kit` để phát triển theo hướng Spec-Driven Development (SDD).

## Cấu trúc chính

- `.specify/`: bộ khung SDD (templates, scripts, integration, memory)
- `.specify/memory/constitution.md`: nguyên tắc phát triển của dự án
- `specs/<feature-id>/`: nơi tạo `spec.md`, `plan.md`, `tasks.md` cho từng feature

## Quy trình làm việc

1. `$speckit-constitution`
2. `$speckit-specify`
3. `$speckit-clarify` (nếu cần)
4. `$speckit-plan`
5. `$speckit-tasks`
6. `$speckit-analyze` + `$speckit-checklist`
7. `$speckit-implement`
