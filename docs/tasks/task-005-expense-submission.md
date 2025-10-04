# Task Template

## Meta Information

- **Task ID**: `TASK-005`
- **Title**: Implement Expense Submission Feature
- **Status**: `Not Started`
- **Priority**: `P1`
- **Created**: 2025-06-17
- **Updated**: 2025-06-17
- **Estimated Effort**: 3 Days
- **Actual Effort**: [Hours/Days]

## Related Documents

- **PRD**: docs/product/prd-main.md (FR6: Expense Submission)
- **ADR**: [None yet]
- **Dependencies**: TASK-001, TASK-003, TASK-004

## Description

Deliver a complete expense submission feature where users can submit expenses that are automatically validated against policies, with auto-approval, auto-rejection, or routing to review based on policy rules.

## Acceptance Criteria

- [ ] Users can submit expenses with date, amount, category, description
- [ ] System automatically validates against applicable policy
- [ ] Expenses over limits are auto-rejected with explanation
- [ ] Eligible expenses are auto-approved based on policy
- [ ] Expenses requiring review are routed to reviewers
- [ ] Users can view all their expenses with status
- [ ] Users can edit expenses before approval
- [ ] Clear feedback on why expense was approved/rejected

## TODOs

### Database Layer
- [ ] Add Expense model to Prisma schema
- [ ] Add ExpenseStatus enum
- [ ] Create and run migration
- [ ] Add indexes for user expense queries

### tRPC Layer
- [ ] Create expense router procedures
- [ ] Implement submitExpense procedure (with policy validation)
- [ ] Implement getUserExpenses procedure
- [ ] Implement updateExpense procedure (before approval)
- [ ] Implement deleteExpense procedure (before approval)
- [ ] Integrate with policy resolution engine
- [ ] Add member-only authorization

### Policy Integration
- [ ] Connect to policy resolution engine
- [ ] Implement auto-approval logic
- [ ] Implement auto-rejection with reasons
- [ ] Create review assignment logic
- [ ] Add policy limit checking

### UI Layer
- [ ] Create expense submission form
- [ ] Create expense listing page
- [ ] Add expense status indicators
- [ ] Create expense edit modal
- [ ] Add policy feedback display
- [ ] Create expense detail view

### Integration
- [ ] Connect all UI to tRPC procedures
- [ ] Test submission flow end-to-end
- [ ] Verify policy validation works
- [ ] Test auto-approval/rejection
- [ ] Add proper error handling

## Progress Updates

### [Date] - [Name]
**Status**: [Current Status]
**Progress**: Description of work completed
**Blockers**: Any issues preventing progress
**Next Steps**: What will be done next

## Completion Checklist

- [ ] All acceptance criteria met
- [ ] Code follows project standards
- [ ] Tests written and passing
- [ ] Documentation updated (if needed)
- [ ] Code review completed

## Notes

Consider adding expense drafts. Implement recurring expenses feature.

---

**Template Version**: 1.0
**Last Updated**: 2025-06-17
