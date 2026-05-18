# Contributions

## Pull Requests

| Date | Repository | Pull Request | Area | Status |
| --- | --- | --- | --- | --- |
| 2026-05-17 | `anurag3407/career-pilot` | [Add profile summary character counter](https://github.com/anurag3407/career-pilot/pull/125) | Frontend | Merged |
| 2026-05-17 | `Canopus-Labs/PrepPilot` | [Add upload file size limit](https://github.com/Canopus-Labs/PrepPilot/pull/7) | Backend | Open |
| 2026-05-18 | `ProKelly/mychart` | [Add lobby room join form](https://github.com/ProKelly/mychart/pull/5) | Django | Open |
| 2026-05-18 | `future-agi/future-agi` | [Add confirmation dialog for eval template deletion](https://github.com/future-agi/future-agi/pull/534) | Frontend | Open |

## Contribution Notes

### `career-pilot`

Added a character counter to a profile summary input in the onboarding flow and included the value in the existing profile payload.

Merged on 2026-05-18.

Checks run:

```text
npx eslint src/pages/fellowship/Onboarding.jsx
npm run build
```

### `PrepPilot`

Added a 5MB upload size limit to the Multer upload middleware while keeping the existing storage and file type validation behavior.

Check run:

```text
node --check backend/middlewares/uploadMiddleware.js
```

### `mychart`

Added a simple lobby join form that passes room and user names into the room view, plus basic Django tests for query parameters and default values.

Checks run:

```text
python manage.py check
python manage.py test
```

### `future-agi`

Added a confirmation dialog before deleting an eval template from the detail page, reusing the existing bulk-delete dialog pattern.

Checks run:

```text
npx eslint src/sections/evals/components/EvalDetailPage.jsx
npx prettier --check src/sections/evals/components/EvalDetailPage.jsx
npx vite build
```
