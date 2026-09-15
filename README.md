# .github

Default community health files, workflow templates, and repository standards for @scottdensmore.

## Workflow Templates

Starter workflows in `workflow-templates/` enforce GitHub Actions storage best practices:
- **3-day retention** on all artifact uploads (`retention-days: 3`) to prevent exhausting GitHub Actions storage quotas on private repositories.
- Use `if: always()` or `if: failure()` appropriately to avoid uploading unnecessarily on passing runs.
