# Taskify Security Remediation Changelog

This changelog documents all security fixes and improvements made to the Taskify application as part of the security education portfolio project.

## Format
Each entry follows this structure:
- **Date**: YYYY-MM-DD
- **Issue**: Brief description of the vulnerability or task
- **Changes**: What was modified
- **Pull Request**: Link to the Pull Request

---

## Changelog Entries

### [2026-03-16] - Initial Changelog Setup
**Issue**: Create project changelog to track all security remediation work
**Changes**: Added CHANGELOG.md to document all security fixes and improvements
**Pull Request**: [https://github.com/MelEUsher/Security_Task-Manager/pull/3]

---

### [2026-03-16] - Fixed SQL Injection in Project Search
**Issue**: Project search vulnerable to SQL injection allowing unauthorized data access
**Changes**: Replaced raw SQL (`$queryRawUnsafe`) with Prisma parameterized queries in `lib/services.ts`. Added user ID enforcement via Prisma's `where` clause to prevent unauthorized project access.
**Pull Request**: [https://github.com/MelEUsher/Security_Task-Manager/pull/8]

---
