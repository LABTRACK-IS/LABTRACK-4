## Summary

Iteration **v4** of LabTrack, imported from ``labtrack 4`` on 2026-11-20.

Compared against: **labtrack 3**.

## Change overview

| Area | Modified | Added |
|------|----------|-------|
| Backend | **3** | **0** |
| Frontend | **12** | **1** |

Full per-file detail in [CHANGELOG-V4.md](./CHANGELOG-V4.md).

## Backend - notable changes

- backend\LabTrack.CSharp\src\LabTrack.Api\Controllers\AuthController.cs (16886 bytes)
- backend\LabTrack.CSharp\src\LabTrack.Api\Controllers\ProblemReportController.cs (8652 bytes)
- backend\LabTrack.CSharp\src\LabTrack.Api\Services\ProblemReportService.cs (12167 bytes)

### New backend files

- (none)

## Frontend - notable changes

- frontend\src\components\admin\CampusesLabsView.tsx (59208 bytes)
- frontend\src\components\admin\IssueServiceDeskView.tsx (51471 bytes)
- frontend\src\components\auth\AuthLayout.tsx (18590 bytes)
- frontend\src\components\portal\PortalShell.tsx (17598 bytes)
- frontend\src\pages\auth\forgot-password-page.tsx (21894 bytes)
- frontend\src\pages\auth\login-page.tsx (22738 bytes)
- frontend\src\pages\auth\register-page.tsx (12970 bytes)
- frontend\src\pages\landing\AboutPage.tsx (21589 bytes)
- frontend\src\pages\landing\FeaturesPage.tsx (25333 bytes)
- frontend\src\pages\landing\HomePage.tsx (21094 bytes)
- ... and 2 more

### New frontend files

- frontend\src\components\common\SequentialTypewriterBanner.tsx (61 lines, NEW)

## QA checklist

- [ ] dotnet build succeeds on backend
- [ ] tsc --noEmit returns 0 errors on frontend
- [ ] /health/live returns 200
- [ ] No junk files (bak, cleanup) in git tree
- [ ] Diff vs labtrack 3 is intentional
- [ ] Swagger shows all controllers

## How to verify

Backend:

    cd backend/LabTrack.CSharp/src/LabTrack.Api
    dotnet build && dotnet run

Frontend (new terminal):

    cd frontend
    npm install && npm run dev

Expected URLs:

- http://localhost:3000 - frontend
- http://localhost:5000/swagger - API docs
- http://localhost:5000/health/live - 200 OK

---

Auto-generated on 2026-11-20 04:01:21
