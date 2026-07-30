# Hi, I'm Arockia

I'm a cybersecurity engineering student at Anna University, class of 2028. Most of my time goes into secure messaging and applied crypto. I do security R&D at GRMG LLC, where I'm building AION Protocol, a secure peer-to-peer communications platform.

## Things I've built

**[tamperlog](https://github.com/ArockiaRajamanickam/tamperlog)** is a Python library for append-only logs you can actually prove things about. Most tamper-evident log code chains hashes together, which catches an edited row but quietly misses truncation, since deleting the last few entries leaves the chain perfectly self-consistent. tamperlog uses RFC 6962 Merkle proofs instead, so a small checkpoint you published earlier is enough to prove the log still holds what it did before, in the same order, with nothing dropped. No dependencies, fully typed.

**[SAATCHI (சாட்சி)](https://github.com/ArockiaRajamanickam/saatchi-app)** is a wage record system for daily wage workers in India. A worker sends a voice note, the system transcribes it, verifies the speaker's voice print, and seals the record into a hash chain anchored to Bitcoin. If anyone tampers with a record later, the public verification page turns red. Built with my team, Nexus Network, for a national AI competition.

**[SBLC Platform](https://github.com/ArockiaRajamanickam/sblc)** manages Standby Letters of Credit for banks, from issuance through KYC/AML compliance to loan disbursement, with role-based access for every party involved. FastAPI, PostgreSQL and Redis under the hood.

**AION Protocol** is my main work at GRMG. End-to-end encrypted peer-to-peer messaging with a tamper-evident integrity ledger. That repo stays private for now.

**[GRMG's website](https://globalmanagementgroupllc.com)** is one I designed and built end to end in React, then translated into 32 languages, including full right-to-left support.

**[react-vite-starter-mipe](https://github.com/ArockiaRajamanickam/react-vite-starter-mipe)** is the small React + Vite template I clone whenever I start something new.

## Open source

I contribute where I actually use things. Recently that has meant a data-loss fix in Alembic's SQLite batch migrations, where a `TypeDecorator` wrapping `JSON` slipped past an `isinstance` check and every value in the column was cast to `0`, and an OIDC fix in django-oauth-toolkit, where RP-initiated logout was not idempotent so a second relying party got rejected instead of its redirect. I try to send a failing test along with the report.

## What I care about

Systems where you don't have to take anyone's word for it. Hash chains, public verification pages, encryption that still holds up if the server is compromised. I also like shipping the whole thing myself: backend, frontend, deploys.

## Stack

Python and FastAPI on the backend, React and TypeScript on the frontend, PostgreSQL, Redis and Docker for everything else.

## Contact

arockia.lyx@gmail.com
