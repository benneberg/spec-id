# Transmitter Engine — Unified PRD & Architecture



---

# PRD.md — Transmitter Engine

## 1. Product Overview

### Name
**Transmitter Engine**

### One-Line Summary
A local-first routing and composition engine that converts technical projects into venue-native posts, pitches, and handoff packages—enabling builders to externalize ideas, attract the right people, and free mental RAM.

### Position in the Ecosystem
- **Externalizer OS** captures raw ideas and project fragments
- **Spec-ID** structures them into coherent system definitions
- **Transmitter Engine** turns those structured systems into targeted external outputs for validation, contributors, operators, acquirers, or adopters

### Core Thesis
A project is not mentally complete when it works.  
It is complete when it has been clearly framed, routed to the right audience, and released from active cognitive ownership.

The Transmitter Engine exists to create that release.

---

## 2. Problem Statement

High-level architects and rapid prototype builders complete the hardest conceptual work but remain mentally occupied by unfinished transfer:

- The system exists
- The architecture is real
- The value is there
- But it has not been properly exposed to the right people

Without a handoff mechanism, projects remain "paged in" mentally.

**The result:**
- Active RAM leakage
- Context switching overhead
- Unfinished psychological loops
- Repeated re-thinking of already-solved architecture

**Existing tools help with:**
- Note capture
- Spec writing
- Posting drafts
- Launch copy

**But they do NOT solve:**
- Where this should go
- Who should see it
- How it should be framed there
- Whether the draft fits community norms
- Whether the project can be mentally marked "transferred"

---

## 3. Product Vision

The Transmitter Engine is not just a copy generator.  
It is a **distribution decision system** for technical artifacts.

It helps the user answer:

1. What kind of project is this?
2. What outcome am I trying to get?
3. Which specific venues are a good fit?
4. What kind of post is culturally acceptable there?
5. How do I say it without sounding like an AI marketer?
6. Can I now consider this project externalized?

### The Shift
**From:**  
`project → platform → post`

**To:**  
`project → objective → audience → venue → post mode → draft → outcome`

That routing model is the real product.

---

## 4. Primary User

### Persona: The Architect / Inventor
A technical creator who:
- Thinks in systems
- Prototypes quickly
- Solves architecture and logic problems
- Is less interested in long-tail execution, operations, GTM, or packaging
- Accumulates active projects faster than they can be transferred

### Their Desired Outcomes
- Validate ideas without overselling
- Find collaborators or maintainers
- Find operators or acquirers
- Release projects into open source
- Package systems for integration or licensing
- **Feel psychological closure after doing so**

---

## 5. Jobs to Be Done

**When I finish a prototype or system design,**  
I want to quickly understand where it belongs and how to present it,  
so I can attract the right people and stop carrying it in my head.

**When I decide I'm done with a project,**  
I want to generate a clean handoff package and post,  
so someone else can execute, operate, maintain, or acquire it.

**When I want validation,**  
I want the system to suggest communities that accept technical critique,  
so I get signal instead of vague praise.

---

## 6. Product Goals

### Primary Goal
Enable **closure through routed exposure**:
- A project is externalized
- The user feels a reduction in mental load
- The output reaches a venue where the ask is culturally appropriate

### Secondary Goals
- Improve venue fit
- Improve post authenticity
- Attract the intended responder type
- Reduce off-topic or spammy drafts
- Create reusable handoff artifacts

### Success Criteria
- Users trust venue recommendations
- Generated drafts feel native to the venue
- Replies come from the intended persona
- Users mark projects externalized with confidence
- Users report "mental decoupling" and reduced cognitive load

---

## 7. Non-Goals

The product is **NOT** intended to:
- Auto-post everywhere
- Maximize reach at all costs
- Generate spammy growth hacks
- Replace human judgment
- Do large-scale cross-posting
- Become a CRM or social scheduler
- Fabricate traction or proof

**The goal is high-fit exposure, not mass distribution.**

---

## 8. Core Product Model

### The Complete Flow
```
Project Fingerprint
    ↓
Objective (Closure Path)
    ↓
Audience Inference
    ↓
Venue Recommendation
    ↓
Post Mode Selection
    ↓
Strategy Generation
    ↓
Draft Composition
    ↓
Compliance Check
    ↓
Handoff Package
    ↓
Externalization
    ↓
Outcome Memory
```

### Key Definitions

**Project Fingerprint**  
A structured representation of what the project is, what stage it's in, what evidence exists, and what kind of transfer is desired.

**Closure Path (Objective)**  
The desired external outcome that allows the creator to mentally release the project.

**Venue**  
A specific community or distribution surface with known cultural norms:
- `Show HN`
- `r/selfhosted`
- `c/selfhosted@lemmy.world`
- `LinkedIn / Operators`
- `Indie Hackers / Feedback`
- `Mastodon / #hashtag cluster`

**Post Mode**  
The culturally valid form of expression for that venue.

**Externalization**  
A deliberate state change indicating that the project has been packaged and released to the outside world.

---

## 9. Supported Closure Paths

1. **Validation** — "Is this architecture useful/correct?"
2. **Adoption** — "People can use this now"
3. **Contributors** — "Looking for collaborators or maintainers"
4. **Open Source** — "I'm releasing this for the community"
5. **Design Partners** — "Looking for teams with this problem"
6. **Handoff** — "Looking for an operator/founder to run this"
7. **Acquisition** — "Looking for a buyer"
8. **Licensing/Integration** — "This can plug into an existing workflow/product"

---

## 10. Supported Post Modes

- **Show** — "Here's what I built"
- **Ask** — "Is this the right approach?"
- **Launch** — "This is now available"
- **OSS Intro** — "Releasing this open source"
- **Technical Write-up** — Deep architectural explanation
- **Design Partner Request** — "Looking for early users with X problem"
- **Handoff** — "Looking for someone to take this over"
- **Integration Pitch** — "This solves Y for teams doing Z"

**A venue match is incomplete unless the post mode is also correct.**

---

## 11. MVP Scope

### Must Have

#### 1. Ingest Project Data
From System Cards / Spec-ID:
- Title
- Problem/solution
- Tech stack
- Links/assets
- Notes
- Handoff readiness

#### 2. Generate Project Fingerprint
Infer or collect:
- Project type
- Maturity stage
- Target audiences
- Commercial intent
- Domain tags
- Evidence/proof available
- Primary ask/objective
- Sensitivity/compliance flags

#### 3. Venue Registry
A curated local registry with metadata:
- Platform
- Venue/community name
- Audience
- Topic tags
- Allowed post modes
- Tone norms
- Self-promo tolerance
- Proof requirements
- Title/body expectations
- Anti-patterns

#### 4. Routing Engine
Recommend top venues with:
- Fit score (0-100)
- Rationale
- Warnings
- Suggested post mode

#### 5. Draft Generation
Generate venue-native drafts:
- **AI OFF:** Deterministic templates
- **AI ON:** Groq strategy + writing passes

#### 6. Handoff Package
Generate:
- Title
- Full body
- Short version
- Lower-self-promo alternative
- Adoption/operator profile
- "The catch" / missing work
- Optional Spec-ID summary attachment

#### 7. Compliance / Culture Check
Before final output, detect:
- Over-promotion
- Missing proof
- Tone mismatch
- Bad CTA strength
- Venue anti-patterns

#### 8. Externalization Flow
Allow user to:
- Copy draft
- Export package
- Mark project externalized
- Visually archive or lock the card

#### 9. Outcome Memory
Capture:
- Recommended venue
- Selected venue
- Post mode
- Copied/exported status
- Externalized timestamp
- Optional later response quality

---

## 12. Starter Venue Set for MVP

Don't attempt to support everything. Start with venues with clear norms:

- **Hacker News** / Show HN
- **Hacker News** / Ask HN
- **Reddit** / r/selfhosted
- **Reddit** / r/SideProject
- **Reddit** / r/programming
- **Indie Hackers** / Feedback
- **Indie Hackers** / Launch
- **LinkedIn** / Operators
- **Product Hunt**
- **Lemmy** / selfhosted or programming community
- **Mastodon** / hashtag cluster
- **GitHub** / release or repo intro

---

## 13. User Workflow

### Main Flow
1. User opens a System Card
2. Clicks **Start Handoff**
3. Selects a closure path/objective
4. System generates or refines the project fingerprint
5. System shows top-ranked venue recommendations
6. User selects a venue
7. User selects or confirms a post mode
8. System generates 2-3 draft variants
9. System runs compliance/culture check
10. User copies or exports the package
11. User marks the project **Externalized**
12. Card enters read-only/archived state
13. User may later log response quality

### Emotional UX Goal
The flow should feel like:
- Organizing
- Packaging
- Releasing
- Closing the loop

**Not like:**
- Content marketing
- Social scheduling
- Self-promo automation

---

## 14. UX Principles

### 1. Venue Before Draft
Don't ask the user to choose a platform first.  
Recommend venues based on fit.

### 2. Specificity Over Genericity
Prefer:
- `r/selfhosted`
- `Show HN`
- `LinkedIn / Operators`

Over:
- Reddit
- HN
- LinkedIn

### 3. The "Tired, Brilliant Engineer" Tone
Generated text should sound:
- Direct
- Precise
- Practical
- Slightly tired but credible
- Honest about what is incomplete

### 4. Proof Matters
Encourage users to include:
- Demo
- Repo
- Screenshot
- Benchmark
- Architecture note

where relevant.

### 5. Closure is a Product Feature
Marking a card "Externalized" is not cosmetic.  
**It is part of the product's core value.**

---

## 15. Success Metrics

### Product Success
- % of projects successfully fingerprinted
- % of sessions where a venue is selected
- % of sessions where a draft is copied/exported
- % of sessions where a card is marked externalized

### Quality Metrics
- Venue recommendation acceptance rate
- Draft edit distance before copy
- User-rated relevance of recommendations
- User-rated authenticity of generated drafts

### Outcome Metrics
- Response quality score
- Response type distribution:
  - Builders
  - Contributors
  - Operators
  - Buyers
  - Noise

### Psychological Metric
**Self-reported "mental RAM freed" score after externalization**

---

## 16. Risks

1. **Wrong Venue Fit** — Technically plausible but culturally wrong recommendations reduce trust
2. **AI Tone Drift** — Drafts may sound synthetic or over-produced
3. **Overfitting to Templates** — Too much determinism produces rigid posts
4. **Missing Proof** — Some venues require repo/demo/screenshots; absence should reduce confidence
5. **Secret Storage Concerns** — Local-first key handling is practical but not perfect

---

## 17. Design Principles

- Local-first
- User-controlled
- Venue-aware
- Anti-hype
- Proof-sensitive
- Honest about incompleteness
- Optimized for signal, not reach
- **Optimized for closure, not content output**

---

## 18. Launch Definition of Done

The MVP is successful when a user can:

1. Open a project card
2. Choose an objective
3. Receive relevant venue recommendations
4. Generate a venue-native draft
5. Copy/export it
6. Mark the project externalized
7. **Feel the project has been "handed off" enough to leave active mindspace**

---

# ARCHITECTURE.md — Transmitter Engine

## 1. Architecture Summary

The Transmitter Engine is a local-first client-side system that:

1. Reads project data from System Cards / Spec-ID
2. Builds a structured Project Fingerprint
3. Scores the project against a curated Venue Registry
4. Recommends ranked venues and post modes
5. Generates a strategy and draft package
6. Validates the draft against venue norms
7. Stores externalization state and optional outcome memory

**Supports both:**
- **AI OFF:** Deterministic routing + templated composition
- **AI ON:** Deterministic routing + AI strategy + AI writing + optional AI critique

---

## 2. Design Principles

### Local-First
User data, cards, routing, and registry work locally.

### Deterministic Core, AI-Enhanced Edges
Routing and validation remain explainable.  
AI helps with:
- Inference
- Phrasing
- Summarization
- Strategy refinement

### Venue-Aware, Not Platform-Aware
The routing unit is the **venue/community**, not the platform.

### Cultural Fit Over Maximum Exposure
Prefer fewer, higher-fit recommendations.

### Human Review Required
The system assists with distribution but does not autonomously post.

---

## 3. High-Level Data Flow

```
System Card / Spec-ID
        ↓
Project Fingerprinter
        ↓
ProjectFingerprint
        ↓
Routing Engine + Venue Registry
        ↓
Ranked Venue Matches
        ↓
User selects venue + objective + post mode
        ↓
Strategy Generator (AI optional)
        ↓
Composer (AI or template)
        ↓
Compliance / Culture Filter
        ↓
Draft Package
        ↓
Copy / Export / Externalize
        ↓
Outcome Memory
```

---

## 4. Core Modules

### 4.1 Project Fingerprinter
Converts project data into a structured fingerprint.

**Inputs:**
- Title
- Description/problem/solution
- Tech stack
- Links
- Status
- Handoff readiness
- Notes from Spec-ID

**Outputs:**
- Typed fields for routing and generation
- Tags inferred from content
- Evidence inventory
- Intended audience/objective

**Modes:**
- Deterministic extraction
- Optional AI-assisted inference for tags, audience, and project type

---

### 4.2 Venue Registry
A curated dataset of specific communities/venues.

**Responsibilities:**
- Define topic and audience fit
- Define accepted post modes
- Define tone norms
- Define self-promo tolerance
- Define proof expectations
- Define formatting constraints
- Define anti-patterns

**Storage:**  
Static bundled JSON or TS file in MVP.

---

### 4.3 Routing Engine
Scores each venue against the project fingerprint and selected objective.

**Responsibilities:**
- Compute fit score
- Explain fit
- Attach warnings
- Recommend post mode
- Rank top matches

**Design:**  
Deterministic and explainable.

---

### 4.4 Strategy Generator
Produces a venue-aware drafting plan.

**Responsibilities:**
- Recommend opening angle
- Recommend CTA
- Specify proof to highlight
- Specify what to avoid
- Choose emphasis based on venue culture

**Note:**  
Only runs when AI is enabled.

---

### 4.5 Composer
Generates actual output variants.

**Output Package:**
- Title
- Body
- Short version
- Softer/lower-promo variant
- Handoff/adoption profile where relevant
- Optional handoff summary

**Modes:**
- AI OFF → Templates
- AI ON → LLM-generated drafts

---

### 4.6 Compliance / Culture Filter
Validates generated output before user copy/export.

**Deterministic Checks:**
- Missing required proof
- Banned phrases
- Title/body length
- Mismatch between venue and post mode
- Excessive CTA intensity
- Likely over-promo

**Optional AI Critique Pass:**
- Would this feel off-topic here?
- Is the tone too promotional?
- Is the opening wrong for this venue?
- Is the proof sufficient?

---

### 4.7 Externalization Engine
Handles state transition from active project to externally packaged project.

**Responsibilities:**
- Record copy/export
- Mark project as externalized
- Store selected venue/objective
- Archive or lock card
- Trigger closure UI treatment

---

### 4.8 Outcome Memory
Stores post-selection and later user feedback.

**Responsibilities:**
- Record which venue was chosen
- Record generated mode and draft type
- Track whether it was copied/exported
- Optionally track whether it was posted
- Optionally log response quality and responder type

---

## 5. Core Domain Model

### 5.1 Enums / Primitive Types

```typescript
export type ProjectType =
  | 'devtool'
  | 'oss_library'
  | 'consumer_app'
  | 'b2b_saas'
  | 'workflow_automation'
  | 'protocol'
  | 'research_artifact'
  | 'internal_tool'
  | 'media_pipeline'
  | 'other';

export type MaturityStage =
  | 'idea'
  | 'prototype'
  | 'working_demo'
  | 'beta'
  | 'launched'
  | 'production_ready'
  | 'oss_live';

export type ClosurePath =
  | 'validation'
  | 'adoption'
  | 'contributors'
  | 'open_source'
  | 'design_partners'
  | 'handoff'
  | 'acquisition'
  | 'licensing_integration';

export type PostMode =
  | 'show'
  | 'ask'
  | 'launch'
  | 'oss_intro'
  | 'technical_writeup'
  | 'design_partner_request'
  | 'handoff'
  | 'integration_pitch';

export type AudienceTag =
  | 'developers'
  | 'founders'
  | 'operators'
  | 'buyers'
  | 'self_hosters'
  | 'researchers'
  | 'creators'
  | 'maintainers'
  | 'sysadmins'
  | 'early_adopters';

export type EvidenceType =
  | 'repo'
  | 'demo'
  | 'screenshots'
  | 'benchmarks'
  | 'users'
  | 'revenue'
  | 'testimonials'
  | 'writeup'
  | 'none';

export type PreferredTone =
  | 'technical'
  | 'pragmatic'
  | 'founder'
  | 'casual'
  | 'academic';

export type Platform =
  | 'reddit'
  | 'hackernews'
  | 'indiehackers'
  | 'linkedin'
  | 'producthunt'
  | 'lemmy'
  | 'mastodon'
  | 'devto'
  | 'github'
  | 'direct';
```

---

### 5.2 ProjectFingerprint

```typescript
export interface ProjectFingerprint {
  projectId: string;

  title: string;
  oneLiner?: string;

  problem: string;
  solution?: string;
  specSummary?: string;

  techStack: string[];
  domainTags: string[];

  projectType: ProjectType;
  maturityStage: MaturityStage;

  closurePath: ClosurePath;
  handoffReadiness?: number; // 1-10

  targetAudiences: AudienceTag[];
  commercialIntent: boolean;

  evidence: EvidenceType[];
  links?: {
    repo?: string;
    demo?: string;
    docs?: string;
    screenshots?: string[];
    listing?: string;
  };

  needsTechnicalContext: boolean;
  complianceFlags?: string[];
  sensitivityFlags?: string[];

  missingPieces?: string[];
  adoptionProfile?: string[];
  creatorRoleAfterTransfer?: string;

  sourceCardId?: string;
  updatedAt: number;
}
```

---

### 5.3 VenueProfile

```typescript
export interface VenueProfile {
  id: string;
  platform: Platform;
  name: string; // e.g., "Show HN", "r/selfhosted"
  description?: string;

  topicTags: string[];
  audienceTags: AudienceTag[];

  allowedPostModes: PostMode[];
  preferredTone: PreferredTone;

  selfPromoTolerance: 0 | 1 | 2 | 3 | 4 | 5;

  requiresProof: EvidenceType[];
  recommendedProof?: EvidenceType[];

  titleStyle: string;
  charLimits?: {
    title?: number;
    body?: number;
  };

  norms: string[];
  forbiddenPatterns: string[];

  stageFit?: MaturityStage[];
  closurePathFit?: ClosurePath[];

  notes?: string[];
}
```

---

### 5.4 RouteMatch

```typescript
export interface RouteMatch {
  venueId: string;
  venueName: string;

  score: number; // 0-100
  suggestedMode: PostMode;

  reasons: string[];
  warnings: string[];

  dimensionScores: {
    topicFit: number;
    audienceFit: number;
    objectiveFit: number;
    modeFit: number;
    stageFit: number;
    proofFit: number;
    toneFit: number;
    promoFit: number;
  };
}
```

---

### 5.5 DraftStrategy

```typescript
export interface DraftStrategy {
  venueId: string;
  postMode: PostMode;
  openingAngle: string;
  keyProofToMention: string[];
  primaryCTA: string;
  avoid: string[];
  theCatch: string; // What's unfinished/missing
  adoptionProfile?: string[]; // Skills next owner needs
  confidence: number; // 0-100
}
```

---

### 5.6 DraftPackage

```typescript
export interface DraftPackage {
  projectId: string;
  venueId: string;
  closurePath: ClosurePath;
  postMode: PostMode;

  title: string;
  body: string;
  shortVersion?: string;
  lowPromoVariant?: string;

  adoptionProfile?: {
    idealNextOwner?: string[];
    missingWork?: string[];
    creatorRoleAfterTransfer?: string;
  };

  compliance: {
    passed: boolean;
    warnings: string[];
    suggestions: string[];
  };

  generatedBy: {
    aiEnabled: boolean;
    strategyModel?: string;
    writingModel?: string;
    version: string;
  };

  createdAt: number;
}
```

---

### 5.7 TransmissionOutcome

```typescript
export interface TransmissionOutcome {
  projectId: string;
  venueId: string;
  postMode: PostMode;
  closurePath: ClosurePath;

  copiedAt?: number;
  exportedAt?: number;
  externalizedAt?: number;

  posted?: boolean;

  responseQuality?: 1 | 2 | 3 | 4 | 5;
  responseTypes?: Array<
    'builders' | 'contributors' | 'operators' | 'buyers' | 'maintainers' | 'noise'
  >;

  mentalRamFreed?: number; // 0-100 self-reported

  notes?: string;
}
```

---

## 6. Routing Model

### 6.1 Core Formula

Venue scoring combines multiple dimensions.

**Suggested weighted scoring:**

- Topic fit: **25%**
- Audience fit: **20%**
- Closure path fit: **20%**
- Post mode fit: **10%**
- Maturity/stage fit: **10%**
- Proof fit: **10%**
- Tone/culture fit: **5%**

**Penalties:**
- Low self-promo tolerance + strong commercial framing
- Missing expected proof
- Mismatched stage
- Mismatched venue culture
- Sensitivity/compliance mismatch

---

### 6.2 Routing Pseudocode

```typescript
function scoreVenue(
  project: ProjectFingerprint,
  venue: VenueProfile,
  inferredMode: PostMode
): RouteMatch {
  const reasons: string[] = [];
  const warnings: string[] = [];

  const topicFit = overlap(project.domainTags, venue.topicTags);
  const audienceFit = overlap(project.targetAudiences, venue.audienceTags);
  const objectiveFit = venue.closurePathFit?.includes(project.closurePath) ? 1 : 0.4;
  const modeFit = venue.allowedPostModes.includes(inferredMode) ? 1 : 0;
  const stageFit = venue.stageFit?.includes(project.maturityStage) ? 1 : 0.5;
  const proofFit = satisfiesProof(project.evidence, venue.requiresProof) ? 1 : 0;
  const toneFit = inferToneFit(project, venue);
  const promoFit = inferPromoFit(project, venue);

  let score =
    topicFit * 25 +
    audienceFit * 20 +
    objectiveFit * 20 +
    modeFit * 10 +
    stageFit * 10 +
    proofFit * 10 +
    toneFit * 5;

  if (project.commercialIntent && venue.selfPromoTolerance < 2) {
    score -= 10;
    warnings.push('Commercial framing may be poorly received here.');
  }

  if (!proofFit && venue.requiresProof.length > 0) {
    warnings.push('Expected proof is missing for this venue.');
  }

  if (topicFit > 0.6) reasons.push('Strong topic alignment.');
  if (audienceFit > 0.6) reasons.push('Audience fit is strong.');
  if (modeFit) reasons.push(`Supports ${inferredMode} posts.`);
  if (proofFit) reasons.push('Available proof matches venue expectations.');

  return {
    venueId: venue.id,
    venueName: venue.name,
    score: Math.max(0, Math.min(100, Math.round(score))),
    suggestedMode: inferredMode,
    reasons,
    warnings,
    dimensionScores: {
      topicFit,
      audienceFit,
      objectiveFit,
      modeFit,
      stageFit,
      proofFit,
      toneFit,
      promoFit
    }
  };
}
```

---

### 6.3 Post Mode Inference

```typescript
function inferPostMode(path: ClosurePath, stage: MaturityStage): PostMode {
  switch (path) {
    case 'validation':
      return 'ask';
    case 'adoption':
      return stage === 'launched' || stage === 'beta' ? 'launch' : 'show';
    case 'contributors':
      return 'oss_intro';
    case 'open_source':
      return 'oss_intro';
    case 'design_partners':
      return 'design_partner_request';
    case 'handoff':
      return 'handoff';
    case 'acquisition':
      return 'handoff';
    case 'licensing_integration':
      return 'integration_pitch';
    default:
      return 'show';
  }
}
```

---

## 7. AI Generation Pipeline

### 7.1 AI OFF Path
Use deterministic templates based on:
- Closure path
- Venue tone
- Post mode
- Available proof

**Good for:**
- Reliability
- Privacy-sensitive use
- Fast drafts
- Fallback when API unavailable

---

### 7.2 AI ON Path
Use a **3-step pipeline:**

#### Step 1 — Strategy
Generate:
- Best opening angle
- Evidence to emphasize
- Explicit CTA
- What to avoid
- "The catch" (what's unfinished)
- Adoption profile
- Confidence

#### Step 2 — Writing
Generate:
- Title
- Body
- Short version
- Low-promo alternative
- Adoption profile if applicable

#### Step 3 — Critique
Validate:
- Venue fit
- Tone fit
- Proof sufficiency
- Self-promo intensity
- Title clarity

---

### 7.3 Prompt Design

#### Shared System Prompt
```typescript
const systemPrompt = `
You are a senior systems architect handing off or exposing a real technical project.

Voice:
- Direct
- Specific
- Practical
- Humble
- Mildly tired, never theatrical

Strict rules:
- NO marketing jargon
- NO hype words like "revolutionary", "game-changing", "unlock", "seamless", "delve"
- State what the project is in plain language
- State what is already solved
- State what is still missing
- Make the ask explicit
- Match the venue culture exactly
`;
```

#### Strategy Prompt
```typescript
const strategyPrompt = `
Given:
- A ProjectFingerprint
- A VenueProfile
- A ClosurePath
- An inferred PostMode

Return JSON:
{
  "best_angle": "How to frame the project for this specific venue",
  "the_catch": "What is unfinished or missing that needs to be disclosed",
  "adoption_profile": ["Skill 1", "Skill 2", "Skill 3"] // What the next owner needs
  "recommended_cta": "The exact call to action based on the closure path",
  "avoid": ["Thing 1", "Thing 2"]
}

Optimize for community fit and authenticity.
`;
```

#### Writing Prompt
```typescript
const writingPrompt = `
Write a post for ${venue.name}.

Constraints:
- Post mode: ${postMode}
- Closure path: ${closurePath}
- Preferred tone: ${venue.preferredTone}
- Norms: ${venue.norms.join('; ')}
- Avoid: ${venue.forbiddenPatterns.join('; ')}

Strategy:
${JSON.stringify(strategy, null, 2)}

STRUCTURE REQUIRED:
1. The Core Utility (What it does and why you built it)
2. The Architecture (Brief tech overview)
3. The Catch (Explicitly state: ${strategy.the_catch})
4. The Handoff/Adoption Profile (Who you're looking for: ${strategy.adoption_profile})
5. CTA: ${strategy.recommended_cta}

Return:
- title
- full body
- short version
- lower-self-promo variant

The draft must sound like a tired, brilliant engineer talking to a peer—NOT a marketer.
`;
```

#### Critique Prompt
```typescript
const critiquePrompt = `
Review this draft for venue fit.

Venue: ${venue.name}
Venue norms: ${venue.norms.join('; ')}
Forbidden patterns: ${venue.forbiddenPatterns.join('; ')}

Draft:
${draft}

Check:
- Does it sound too promotional?
- Is it too vague?
- Is the CTA too strong for this venue?
- Is expected proof missing?
- Would the audience understand the first sentence?
- Does it fit the selected post mode?

Return JSON:
{
  "passed": true/false,
  "warnings": ["Warning 1", "Warning 2"],
  "suggestions": ["Suggestion 1", "Suggestion 2"]
}
`;
```

---

## 8. Compliance / Culture Filter Rules

### 8.1 Deterministic Checks
- Banned phrase list by venue
- Title too long / too vague
- No repo/demo when venue expects proof
- Mismatch between venue and post mode
- Business jargon in technical venue
- Overly technical first sentence in operator venue
- Missing explicit CTA
- Missing "what's unfinished" in handoff flow

### 8.2 Example Banned Phrase Set

**Global default:**
- revolutionary
- game-changing
- unlock
- seamless
- delve
- next-gen
- world-class
- disruptive
- cutting-edge
- leverage (as a verb in marketing context)

**Venue-specific bans can be appended.**

---

## 9. Storage Model

### 9.1 IndexedDB
Recommended for:
- System cards
- Project fingerprints
- Generated drafts
- Outcomes
- Externalization state

### 9.2 localStorage
Used in MVP for:
- Groq API key
- Lightweight settings
- User preferences

**Note:**  
localStorage is acceptable for a local-first MVP, but future options may include:
- Session-only storage
- Encrypted local storage
- User-supplied environment injection

### 9.3 Static Assets
- `venues.json`
- `templates.ts`
- Prompt presets
- Banned phrase rules

---

## 10. Suggested File Structure

```
/src
  /components
    TransmitterPanel.tsx
    VenueRecommendations.tsx
    DraftPreview.tsx
    ComplianceWarnings.tsx
    ExternalizeDialog.tsx
    ClosureAnimation.tsx

  /core
    fingerprint.ts
    routing.ts
    postMode.ts
    compliance.ts
    templates.ts
    scoring.ts

  /ai
    groq.ts
    prompts.ts
    strategy.ts
    compose.ts
    critique.ts

  /data
    venues.json
    defaults.ts
    bannedPhrases.ts

  /storage
    cards.ts
    settings.ts
    outcomes.ts
    drafts.ts

  /types
    transmitter.ts
```

---

## 11. UI State Machine

```
ACTIVE
  ↓
FINGERPRINTED
  ↓
ROUTED
  ↓
DRAFTED
  ↓
COPIED / EXPORTED
  ↓
EXTERNALIZED
  ↓
ARCHIVED / READ_ONLY
```

### State Notes
- A project can be drafted without being externalized
- Externalization should require explicit confirmation
- Archive state should preserve generated package and selected venue
- **The visual treatment of externalized cards is a core UX feature**

---

## 12. UX Outputs

### 12.1 Recommendation View
Show:
- Top 3 venues
- Score
- Suggested post mode
- Reasons
- Warnings

**Example:**
```
Show HN — 87
✓ Strong topic fit
✓ Working demo available
✓ Best mode: Show
⚠ Avoid operator/acquisition framing
```

### 12.2 Draft Package View
Show:
- Title
- Body
- Short version
- Lower-promo version
- Compliance warnings
- Adoption profile
- Missing proof suggestions

### 12.3 Closure View
After externalization:
- Venue used
- Objective used
- Date externalized
- Exported assets
- **"Mental RAM Freed: 15%" badge**
- Optional vault-locking or paper-airplane animation

---

## 13. Starter Venue Registry Examples

```typescript
export const venues: VenueProfile[] = [
  {
    id: 'hn_show',
    platform: 'hackernews',
    name: 'Show HN',
    topicTags: ['devtools', 'systems', 'ai', 'oss', 'automation'],
    audienceTags: ['developers', 'founders', 'early_adopters'],
    allowedPostModes: ['show', 'oss_intro', 'technical_writeup'],
    preferredTone: 'technical',
    selfPromoTolerance: 3,
    requiresProof: ['demo'],
    recommendedProof: ['repo', 'writeup'],
    titleStyle: 'Show HN: {name} – {plain description}',
    norms: ['Be direct', 'Explain why you built it', 'Avoid hype'],
    forbiddenPatterns: ['revolutionary', 'game-changing', 'vague launch copy'],
    stageFit: ['working_demo', 'beta', 'launched', 'oss_live'],
    closurePathFit: ['validation', 'adoption', 'open_source']
  },
  {
    id: 'reddit_selfhosted',
    platform: 'reddit',
    name: 'r/selfhosted',
    topicTags: ['self-hosting', 'privacy', 'automation', 'infra'],
    audienceTags: ['developers', 'sysadmins', 'self_hosters'],
    allowedPostModes: ['show', 'ask', 'oss_intro'],
    preferredTone: 'technical',
    selfPromoTolerance: 2,
    requiresProof: ['repo'],
    recommendedProof: ['screenshots', 'demo'],
    titleStyle: 'State clearly what it does',
    norms: [
      'Lead with utility',
      'Be transparent that you built it',
      'Setup details help'
    ],
    forbiddenPatterns: ['business jargon', 'vague pitch'],
    stageFit: ['prototype', 'working_demo', 'oss_live', 'beta'],
    closurePathFit: ['validation', 'open_source', 'contributors', 'adoption']
  },
  {
    id: 'linkedin_operators',
    platform: 'linkedin',
    name: 'LinkedIn / Operators',
    topicTags: ['workflow', 'automation', 'b2b', 'operations'],
    audienceTags: ['operators', 'founders', 'buyers'],
    allowedPostModes: ['handoff', 'launch', 'design_partner_request', 'integration_pitch'],
    preferredTone: 'pragmatic',
    selfPromoTolerance: 4,
    requiresProof: ['none'],
    recommendedProof: ['writeup', 'demo'],
    titleStyle: 'Lead with business outcome',
    norms: [
      'Translate technical depth into leverage',
      'Keep first sentence non-technical',
      'Use a clear CTA'
    ],
    forbiddenPatterns: ['overly academic opening'],
    stageFit: ['prototype', 'working_demo', 'beta', 'launched', 'production_ready'],
    closurePathFit: ['handoff', 'design_partners', 'licensing_integration', 'acquisition']
  },
  {
    id: 'ih_feedback',
    platform: 'indiehackers',
    name: 'Indie Hackers / Feedback',
    topicTags: ['saas', 'startup', 'bootstrapping', 'mvp'],
    audienceTags: ['founders', 'early_adopters', 'developers'],
    allowedPostModes: ['ask', 'show', 'launch'],
    preferredTone: 'founder',
    selfPromoTolerance: 3,
    requiresProof: ['demo'],
    recommendedProof: ['users', 'revenue'],
    titleStyle: 'Ask a specific question',
    norms: [
      'Be vulnerable about challenges',
      'Share metrics if you have them',
      'Ask specific questions'
    ],
    forbiddenPatterns: ['pure promotion without ask'],
    stageFit: ['prototype', 'working_demo', 'beta', 'launched'],
    closurePathFit: ['validation', 'design_partners', 'adoption']
  }
];
```

---

## 14. Integration with Existing Products

### Externalizer OS
Source of raw ideas and cards.

### Spec-ID
Source of structured problem/solution/system details.

### Transmitter Engine
Consumes those artifacts and produces:
- Venue recommendations
- Handoff packages
- Externalization records

**The three products form a complete idea-to-externalization pipeline.**

---

## 15. Implementation Plan

### Phase 1 — Deterministic MVP
- Define schemas
- Build venue registry
- Build fingerprint extractor
- Build routing engine
- Build templates for AI OFF mode
- Build copy/export/externalize flow

### Phase 2 — AI Strategy + Writing
- Groq integration
- Strategy pass
- Writing pass
- Critique pass

### Phase 3 — Outcome Learning + Polish
- Response logging
- Venue performance summaries
- Personalized recommendation tuning
- Closure animations
- Mental RAM freed metrics

---

## 16. Acceptance Criteria

The architecture is complete enough for MVP when:

1. A card can be converted into a ProjectFingerprint
2. At least 8-12 venues are represented in a registry
3. The app can rank venues with reasons and warnings
4. The app can generate at least one usable draft in AI OFF mode
5. The app can generate improved drafts in AI ON mode
6. The app can validate draft fit before copy/export
7. The user can mark a project externalized
8. The app stores outcome metadata locally
9. **The externalization feels psychologically satisfying**

---

## 17. Future Extensions

- Custom private buyer/operator lists
- More advanced learning from outcomes
- Team mode / shared registries
- External repo analysis for proof extraction
- Screenshot and asset attachment suggestions
- Per-venue title optimization
- Region/language-specific venue packs
- "Should I post this yet?" readiness scoring
- Integration with direct messaging for private handoffs
- Buyer/acquirer database integration

---

## 18. Final Architectural Position

The Transmitter Engine is best understood as:

- A **fingerprinting system**
- A **routing system**
- A **cultural adaptation system**
- A **handoff package generator**
- A **closure mechanism**

**It is not a generic AI writer.**

**That distinction is the product.**

---

## Summary of Improvements

This merged version incorporates:

1. ✅ **Closure philosophy** — "Mental RAM freed" is a core metric
2. ✅ **Routing model** — Objective → Venue → Post Mode flow
3. ✅ **Venue/community abstraction** — Specific, not generic
4. ✅ **Anti-AI/anti-marketing tone controls** — Banned phrases, "tired engineer" persona
5. ✅ **Adoption/handoff profile** — "The catch" and "next owner skills"
6. ✅ **Compliance + outcome memory** — Pre-flight checks and post-externalization tracking
7. ✅ **Non-goals explicitly stated**
8. ✅ **Starter venue set for MVP**
9. ✅ **Wording shifted from "platform" to "venue"**
10. ✅ **TypeScript schemas included**
11. ✅ **3-step AI pipeline** (Strategy → Writing → Critique)
12. ✅ **Psychological closure as UX feature**

The result is a **complete, actionable specification** ready for implementation.
