# Task Template

## Meta Information

- **Task ID**: `TASK-002`
- **Title**: Implement User Invitation System
- **Status**: `Not Started`
- **Priority**: `P0`
- **Created**: 2025-06-17
- **Updated**: 2025-06-17
- **Estimated Effort**: 3 Days
- **Actual Effort**: [Hours/Days]

## Related Documents

- **PRD**: docs/product/prd-main.md (FR1: User Management)
- **ADR**: [None yet]
- **Dependencies**: TASK-001

## Description

Deliver a complete user invitation system allowing organization admins to invite users via email, users to accept invitations, and role management. Includes database schema, tRPC procedures, email integration, and full UI.

## Acceptance Criteria

- [ ] Admins can invite users via email from UI
- [ ] Invitation emails are sent with magic links
- [ ] Users can view pending invitations
- [ ] Users can accept/decline invitations
- [ ] Role (Admin/Member) assigned on joining
- [ ] Admins can view all organization members
- [ ] Admins can change user roles
- [ ] Invitation tokens expire after 7 days

## TODOs

### Database Layer
- [ ] Add Invitation model to Prisma schema
- [ ] Add role field to UserOrganization relationship
- [ ] Create and run migration
- [ ] Add indexes for performance

### tRPC Layer
- [ ] Create invitation router procedures
- [ ] Implement inviteUser procedure
- [ ] Implement getInvitations procedure (for user)
- [ ] Implement acceptInvitation procedure
- [ ] Implement getOrganizationMembers procedure
- [ ] Implement updateUserRole procedure
- [ ] Add authorization middleware

### Email Integration
- [ ] Configure email service (Resend/SendGrid)
- [ ] Create invitation email template
- [ ] Implement email sending service
- [ ] Add email tracking/logging

### UI Layer
- [ ] Create invite user form/modal
- [ ] Create invitations page for users
- [ ] Create organization members page
- [ ] Add role management UI
- [ ] Create invitation status indicators
- [ ] Add search/filter for members

### Integration
- [ ] Connect all UI to tRPC procedures
- [ ] Test invitation flow end-to-end
- [ ] Add proper error handling
- [ ] Test role-based access control

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

Consider adding invitation resend functionality. Implement invitation revocation for admins.

---

**Template Version**: 1.0
**Last Updated**: 2025-06-17
