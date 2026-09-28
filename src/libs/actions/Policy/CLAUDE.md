# Policy actions (src/libs/actions/Policy)

Client-side actions for workspace ("policy") settings: members, approvals and
workflows, categories, tags, distance rates and per diem.

- Member.ts: adding, removing and importing workspace members and their approver settings.
- Actions build optimistic Onyx data and call the backend with API.write; use the onyx skill for patterns.
- Tests: tests/actions/PolicyMemberTest.ts (members), tests/actions/WorkflowTest.ts (workflows),
  tests/ui/ImportedMembersPageTest.tsx (spreadsheet import UI).
- Run one test file: npm test -- <path>
- Keep fixes small, and add a regression test with every bug fix.
