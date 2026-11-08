# Better Dumangas

Independent community transparency portal for **Dumangas, Iloilo**, maintained by [@zerozepol](https://github.com/zerozepol). Work in Progress. Not an official LGU website and not yet registered with or endorsed by BetterGov.

## Run locally

No package installation is required. Build using `node build.mjs`, then run `python3 -m http.server 4173 --directory dist` and open http://localhost:4173. Node.js 18+ and Python 3 are sufficient.

## Scope

This is an independent repository, with its own initial commit, source, LGU data and build. No dependency on the previous shared portal or another LGU repository. Relative asset paths support both domain-root and subpath hosting.

Six sections follow the [BetterGov LGU guide](https://lgu.bettergov.ph/GUIDE): offices/services, barangays, officials, budget/expenditure sources, project records and ordinance archive. The visual system derives from our earlier Bayan Portal implementation; no third-party template code is included.

## Data

51 sourced listings, including 45 barangay name listings. See `src/data.json` for per-entry sources, review dates and caveats. Contact numbers have not been telephone-tested. Public source information was reviewed 8 November 2026. Barangay listings are names only, not verified contact listings. Historical procurement records do not establish delivery or completion. No current financial dataset or complete recent ordinance archive is claimed.

## Contribute

Open an issue or PR with a public source for corrections. Add the source URL, `reviewed` date, and a note explaining uncertainty. Rebuild and check search, all six sections, dialogs, CSV and mobile before publishing. Review public sources quarterly; no automatic monitoring is configured.

## Deployment

Build output is `dist/`, suitable for static hosting. This repository has no hosting credentials or inherited Sites project ID. Publication is separate from repository creation. See `BETTERGOV-SUBMISSION.md` for a draft registration row. Do not claim Active while the public portal is not live.

## Sources

- https://fdpp.blgs.gov.ph/
- https://iloilo.gov.ph/en/node/113
- https://notices.philgeps.gov.ph/GEPSNONPILOT/Tender/PrintableBidNoticeAbstractUI.aspx?refid=11481024
- https://psa.gov.ph/classification/psgc/barangays/0603018000
- https://www.iloilo.gov.ph/municipal-directory
