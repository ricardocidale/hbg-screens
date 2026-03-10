# HBG Screens & Documentation

All page-level React components and complete project documentation for the Hospitality Business Group portal.

## Screens (79 files)

### Core Pages
| Screen | File | Description |
|--------|------|-------------|
| Dashboard | `Dashboard.tsx` | KPI grid, charts, portfolio overview |
| Portfolio | `Portfolio.tsx` | Property cards grid with filters |
| Property Detail | `PropertyDetail.tsx` | Full property view with financial tabs |
| Property Edit | `PropertyEdit.tsx` | Property form (assumptions, revenue, expenses) |
| Company | `Company.tsx` | Management company financials (4 tabs: Income, Cash Flows, Balance Sheet, Funding) |
| Executive Summary | `ExecutiveSummary.tsx` | High-level investment summary |
| Analysis | `Analysis.tsx` | Sensitivity, Financing, Compare, Timeline tabs |
| Admin | `Admin.tsx` | Full admin panel (10 tabs) |

### Analysis & Research
| Screen | File |
|--------|------|
| Sensitivity | `SensitivityAnalysis.tsx` |
| Financing | `FinancingAnalysis.tsx` |
| Comparison | `ComparisonView.tsx` |
| Timeline | `TimelineView.tsx` |
| Funding | `FundingPredictor.tsx` |
| Research Hub | `ResearchHub.tsx` |
| Property Research | `PropertyMarketResearch.tsx` |
| Company Research | `CompanyResearch.tsx` |
| Global Research | `GlobalResearch.tsx` |

### Tools & Settings
| Screen | File |
|--------|------|
| Property Finder | `PropertyFinder.tsx` |
| Map View | `MapView.tsx` |
| Scenarios | `Scenarios.tsx` |
| Company Assumptions | `CompanyAssumptions.tsx` |
| Settings | `Settings.tsx` |
| Profile | `Profile.tsx` |
| Methodology | `Methodology.tsx` |
| VoiceLab | `VoiceLab.tsx` |
| Login | `Login.tsx` |
| Logos | `Logos.tsx` |

### Documentation Pages
| Screen | Directory |
|--------|-----------|
| User Manual | `user-manual/` (17 sections) |
| Checker Manual | `checker-manual/` (21 sections + formulas) |
| Help | `Help.tsx` |

## Documentation (242 files)

### `.claude/` Structure
```
.claude/
├── claude.md                    # Master project reference (sole source of truth)
├── rules/                       # Invariants & constraints (19 rules)
├── skills/                      # Feature-specific documentation
│   ├── admin/                   # Admin panel (8 sub-docs)
│   ├── architecture/            # API routes, storage, project description
│   ├── charts/                  # Chart library (9 components)
│   ├── codebase-architecture/   # Module boundaries, barrel files
│   ├── design-system/           # Themes, colors, typography
│   ├── marcela-ai/              # AI assistant (6 sub-docs)
│   ├── twilio-telephony/        # Voice & SMS (6 sub-docs)
│   ├── ui/                      # UI patterns (40+ sub-docs)
│   └── ...                      # Additional skills
├── manuals/                     # Manual source content
│   ├── user-manual/             # 16 skill files
│   └── checker-manual/          # 15 skills + 5 formula docs + glossary
└── commands/                    # CLI command references
```

### Key Documentation
| Topic | Path |
|-------|------|
| Master reference | `.claude/claude.md` |
| Financial engine rules | `.claude/rules/financial-engine.md` |
| Architecture rules | `.claude/rules/architecture.md` |
| Design system | `.claude/skills/design-system/SKILL.md` |
| Admin panel | `.claude/skills/admin/SKILL.md` |
| AI assistant | `.claude/skills/marcela-ai/SKILL.md` |
| Chart library | `.claude/skills/charts/SKILL.md` |
| UI patterns | `.claude/skills/ui/*.md` |

## Routing

`client/src/App.tsx` contains the full route configuration mapping URLs to page components.

## Dependencies

These screens depend on:
- **Design System**: `ricardocidale/hbg-design-system` (UI components, themes, icons, charts)
- **ElevenLabs**: `ricardocidale/hbg-elevenlabs` (AI agent components for VoiceLab, Help)
- **Twilio**: `ricardocidale/hbg-twilio-telephony` (telephony admin)
