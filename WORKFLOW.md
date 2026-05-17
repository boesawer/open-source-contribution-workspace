# Contribution Workflow

## 1. Read First

- Read the issue, comments, linked pull requests, and contribution guidelines.
- Confirm the issue is still open and not already covered by another pull request.
- Identify the smallest useful change that would address the request.

## 2. Inspect Locally

- Clone or fork the repository.
- Read the relevant files before editing.
- Check package manager, scripts, and setup notes.
- Reproduce the issue when practical.

## 3. Keep the Change Focused

- Match the project style.
- Avoid unrelated refactors.
- Prefer one clear fix per pull request.
- Add or update tests when the project structure makes that practical.

## 4. Verify

- Run the most relevant check available.
- For UI changes, verify the affected screen where possible.
- If a full repo check fails because of existing unrelated issues, mention that clearly in the pull request.

## 5. Open the Pull Request

PR template:

```md
## Summary
- ...

## Testing
- ...

Fixes #ISSUE_NUMBER
```

## 6. Respond to Feedback

- Respond clearly and politely.
- Keep follow-up commits focused on maintainer feedback.
- Do not expand scope unless the maintainer asks for it.
