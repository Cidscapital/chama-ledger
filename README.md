# chama-ledger

A full-stack web app that helps **chamas** (savings groups) keep a clear, shared record of contributions, loans and repayments.

![status](https://img.shields.io/badge/status-in%20progress-orange) ![react](https://img.shields.io/badge/frontend-React-61dafb) ![flask](https://img.shields.io/badge/backend-Flask-black) ![license](https://img.shields.io/badge/license-MIT-green)

> 🚧 **In progress.** This README is the plan I'm building against. Features are ticked off as they land.

## Why this project

Millions of Kenyans save and borrow through chamas, but many groups still track money in a notebook or a WhatsApp thread. Records go missing and trust suffers. chama-ledger gives every member the same up-to-date view of where the money is.

## Planned features

- [ ] Sign-up and login with JWT authentication
- [ ] Roles: **chairperson**, **treasurer** and **member**, each with its own permissions
- [ ] Create a group and invite members
- [ ] Record contributions and see each member's running balance
- [ ] Loans with interest, repayment schedules and overdue flags
- [ ] Member statements and a group dashboard (totals, arrears, loan book)
- [ ] Export statements to CSV and PDF
- [ ] Pay contributions by M-Pesa through [mpesa-checkout-api](https://github.com/Cidscapital/mpesa-checkout-api)
- [ ] Tests for the API (pytest) and the UI (Vitest + React Testing Library)

## Data model

`Group` → `Member` → `Contribution`\
`Member` → `Loan` → `Repayment`

Every change to money is recorded as a new entry, never edited in place, so the history can always be audited.

## Tech stack

**Frontend:** React · Vite · React Router\
**Backend:** Python · Flask · SQLAlchemy · PostgreSQL\
**Tooling:** pytest · Vitest · Docker · GitHub Actions

## Roadmap

| Milestone | Scope | Status |
|---|---|---|
| 1 | API skeleton, database schema, authentication | ⏳ |
| 2 | Groups, members and contributions | ⏳ |
| 3 | Loans, repayments and statements | ⏳ |
| 4 | React dashboard, exports, deployment | ⏳ |
| 5 | M-Pesa payments | ⏳ |

## Running locally

Setup instructions will be added with milestone 1.

---

Built by [Jesse Jason Momanyi](https://github.com/Cidscapital) · [LinkedIn](https://www.linkedin.com/in/jesse-jason-m/)
