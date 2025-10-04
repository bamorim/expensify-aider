# Task Template

## Meta Information

- **Task ID**: `TASK-003`
- **Title**: Implement Expense Categories Management
- **Status**: `Not Started`
- **Priority**: `P1`
- **Created**: 2025-06-17
- **Updated**: 2025-06-17
- **Estimated Effort**: 2 Days
- **Actual Effort**: [Hours/Days]

## Related Documents

- **PRD**: docs/product/prd-main.md (FR3: Expense Categories)
- **ADR**: [None yet]
- **Dependencies**: TASK-001, TASK-002

## Description

Deliver a complete expense categories management feature allowing organization admins to create, edit, and delete expense categories. Includes database schema, tRPC procedures, and full UI with validation and safety checks.

## Acceptance Criteria

- [ ] Admins can create new categories from UI
- [ ] Admins can edit category names and descriptions
- [ ] Admins can delete unused categories
- [ ] Categories are organization-scoped
- [ ] Categories can't be deleted if expenses exist
- [ ] Category listing with search and filter
- [ ] Categories can be reordered
- [ ] Default categories created for new orgs

## TODOs

### Database Layer
- [ ] Add ExpenseCategory model to Prisma schema
- [ ] Add order field for sorting
- [ ] Create and run migration
- [ ] Add unique constraint on name + orgId

### tRPC Layer
- [ ] Create category router procedures
- [ ] Implement createCategory procedure
- [ ] Implement updateCategory procedure
- [ ] Implement deleteCategory procedure (with safety checks)
- [ ] Implement getCategories procedure
- [ ] Implement reorderCategories procedure
- [ ] Add admin-only authorization

### UI Layer
- [ ] Create category management page
- [ ] Create category form (create/edit)
- [ ] Create category list with drag-and-drop
- [ ] Add delete confirmation modal
- [ ] Create category selection dropdown
- [ ] Add search/filter functionality

### Integration
- [ ] Connect UI to all tRPC procedures
- [ ] Test category management flow
- [ ] Add proper error handling
- [ ] Test deletion safety checks
- [ ] Verify organization scoping

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

Consider adding category icons/colors. Implement category usage statistics.

---

**Template Version**: 1.0
**Last Updated**: 2025-06-17
