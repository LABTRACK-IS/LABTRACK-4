# LabTrack v4 - Iteration 4

Iteration 4 of LabTrack. Imported from labtrack 4 on 2026-11-20.

Compared against: **labtrack 3**.

## Snapshot

- Backend controllers: **29**
- Backend C# files: **459**
- Frontend TS/TSX files: **72**

## Changes in v4 (vs labtrack 3)

### Backend

- **3** files modified
- **0** new files
- Fixed Compile Include directives (CS0101)

### Frontend

- **12** files modified
- **1** new files

## Infrastructure

- Removed stray Compile Include directives from csproj files
- Removed bak and cleanup text artifacts from working tree
- Updated .gitignore to prevent re-commit

## Full details

See [CHANGELOG-V4.md](./CHANGELOG-V4.md) for per-file diff.

## Controllers

- AiAssistant
- Analytics
- Asset
- Audit
- Auth
- ChainOfCustody
- Communication
- Financial
- IdempotencyRecords
- InstructorCommunication
- Laboratories
- Maintenance
- MaintenanceRecord
- MaintenanceRecords
- Network
- NetworkIncident
- NetworkInfo
- Notification
- PcUsage
- ProblemReport
- QrAdmin
- Qr
- QrSession
- RepairTicket
- Replacement
- ReplacementRecord
- Reservation
- Users
- Workstations

## Quick start

Backend:

    cd backend/LabTrack.CSharp/src/LabTrack.Api
    dotnet run

Frontend:

    cd frontend
    npm install
    npm run dev

Endpoints:

- Frontend: http://localhost:3000
- Swagger: http://localhost:5000/swagger
- Health: http://localhost:5000/health/live

---

Generated: 2026-11-20 04:01:21
