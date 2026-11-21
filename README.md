# EC-018 · ECE-006 — Wi-Fi Hotspot Voucher and Session Accounting Engine

A Python 3.10+ command-file-driven engine for prepaid Wi-Fi hotspot vouchers, device sessions, TIME/DATA accounting, idle timeouts, and end-of-day reports.

## Team

| Member | Role | Ownership |
|---|---|---|
| Sravan N (Member 1) | Core engine | Timeline, sessions, voucher lifecycle, billing |
| Devananda Ajith (Member 2) | Supporting modules | Parser, validation, registry, reporting, integration |

Team EC-018 currently has two active members. The project handoff records the team change from three members to two; Johans Prajval Zakkam is no longer an active team member.

## Technology

- Python 3.10+
- pytest
- `decimal.Decimal` for usage quantities and other decimal-sensitive accounting
- Deterministic priority-queue event processing

## Project status

**Week 1 design — pending team review and mentor approval.** No production application code should be started until the design is approved. The official Week 2 command-file and expected-output specification has not yet been supplied; parser and reporter formats must not be guessed.

## Planned structure

See [docs/design.md](docs/design.md) for the domain model, event ordering, business rules, edge cases, ownership, interface proposal, and review checklist.

## Git workflow

- Work on focused feature branches; do not commit directly to `main`.
- Submit changes through pull requests and obtain at least one approval.
- Include the relevant business-rule ID in commit messages.
- Both members must review the shared `src/models.py` interface and understand the full system.

## Repository naming

The required repository name is `EC-018-ECE-006`. The current GitHub repository name includes a leading hyphen (`-EC-018-ECE-006`); repository rename remains pending because the connected GitHub actions do not expose a rename operation.
