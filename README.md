# CICAN

CICAN is an independent educational interface for exploring publicly available and declassified historical intelligence records.

## Experience

The site uses a fictional access-path simulation inspired by real intelligence concepts:

**RECRUIT → ANALYST → CONFIDENTIAL → SECRET → TOP SECRET → COMPARTMENT**

Important: U.S. national-security classification has three formal levels: **Confidential, Secret, and Top Secret**. SCI, SAP, and compartmentation are controlled-access concepts rather than additional classification levels. The CICAN stages use these ideas as gameplay language and do not provide or represent access to classified information.

## CICAN interaction

The original locked CICAN interaction is preserved:

- Start size: 34
- Growth: +0.5
- Maximum size: exactly 180
- Movement interpolation: x += (targetX - x) * 0.10 and y += (targetY - y) * 0.10
- Double-tap window: 350ms
- Split placement: +45
- Merge distance: 20
- FULL + FULL → merge → record access
- FULL + small → merge, no record access
- small + small → merge, no record access

The interaction is the access mechanism, not decoration.

## Source policy

Records shown by the interface must point to real public sources. The primary source is the CIA FOIA Electronic Reading Room:

https://www.cia.gov/readingroom/

The project must never fabricate a CIA document, claim access to current classified information, or imply that the user has received a real security clearance. A direct PDF/file URL is only used when independently verified from the public source; a filename shown by a CIA source page is stored as metadata rather than turned into a guessed URL.

## Current build

- index.html — landing/access briefing
- decode.html — CICAN access-path simulation and public-record gateway
- academy.html — researcher training
- organization.html — public organizational map
- investigation.html — source-verification cases
- network.html — knowledge network
- evidence.html — evidence dossier
- legal.html — legal, independence, source and copyright policy
- privacy.html — privacy and browser-storage notice
- records.json — source-mapped public-record catalog (v1.14; 96 records)\n\nCurrent catalog integrity: 96 unique records, 74 with direct public CIA source pages, and 23 with verified public PDF attachment filenames.\n\nThe catalog distinguishes CIA Reading Room indexes, public collections, and individual public document pages. Where the CIA source page explicitly lists a PDF attachment, CICAN records the verified public attachment filename as metadata; it does not invent or assume a direct PDF URL.

## Legal / independence baseline

CICAN is an independent educational and research project. It is not affiliated with, endorsed by, sponsored by, approved by, or operated by the U.S. Central Intelligence Agency or the U.S. Government. “CIA” is retained only where it is necessary to identify an actual government source, record, collection, or historical fact.

The project does not use the CIA seal as its product identity. Simulated ranks, access stages, compartments, and missions are fictional gameplay elements and do not grant or imply real clearance or government authority.

See **legal.html** and **privacy.html** for the project's current independence, source, privacy, copyright, external-link, storage, and legal-review disclosures.

This is a project-level disclosure baseline, not a jurisdiction-specific legal opinion. Commercial or app-store release should receive a professional legal review before publication.
