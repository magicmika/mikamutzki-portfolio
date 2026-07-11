# 13_FOUNDATION_V2_TEST_LOG

## Purpose

Evidence log for hypotheses, controlled variants, findings, accessibility checks and decisions.

## Test template

### TEST-ID — Title

- **Status:** EXPLORATION | CANDIDATE | APPROVED | REJECTED
- **Hypothesis:**
- **Must prove:**
- **Controlled variables:**
- **Assets and source:**
- **Variants:**
- **Evaluation criteria:**
- **Accessibility checks:**
- **Observed result:**
- **Decision:**
- **Learning:**
- **Next gate:**
- **Figma link/node:**

---

## EXP-01 — Abstract colour and typography micro-tests

- **Status:** EXPLORATION
- **Hypothesis:** Strong saturated fields, Switzer and surface switching can express Constructive Poster without muddy neutrality.
- **Variants:** Electric blue, signal orange and a combined-colour exploration.
- **Observed result:** Blue and orange were strong separately; their mixture in one composition felt less coherent.
- **Accessibility:** Black on the tested blue failed for small text; off-white passed. Off-white on the tested orange failed for small text; black passed numerically but still required stronger type for perceptual clarity.
- **Decision:** Colours remain test values. Small text on colour should not use fine weights; exact typography rules remain unapproved.

## EXP-02 — Full Floom screen on colour field

- **Status:** REJECTED
- **Hypothesis:** A complete UX screen can sit directly on a saturated system field.
- **Observed result:** Pale lavender areas produced unintended frames and competing colour layers.
- **Learning:** A complete screen is not automatically suitable as a poster-like hero medium.

## EXP-03 — Black product stage

- **Status:** REJECTED
- **Hypothesis:** A black isolation field can separate the product colour world from the system colour.
- **Observed result:** The result became a heavy frame inside another field and made the product feel smaller and more like a generic mock-up.
- **Learning:** Isolation by adding another container can increase rather than resolve visual layering.

## EXP-04 — Borderless enlarged UI crop

- **Status:** REJECTED FOR THIS ASSET
- **Hypothesis:** A large crop can turn the UI screen into an active compositional field.
- **Observed result:** The chosen screen was unsuitable for aggressive enlargement; important evidence and image quality were compromised.
- **Learning:** Crop behaviour must follow evidence type and asset suitability.

## EXP-05 — Perspective device object

- **Status:** REJECTED
- **Hypothesis:** A transparent 3D device can hover across Constructive Poster fields.
- **Observed result:** Photorealistic perspective and material depth conflicted with the flat graphic system.
- **Learning:** Media style must share the spatial language of the surrounding art direction.

## EXP-06 — Frontal device object

- **Status:** CANDIDATE MEDIA TREATMENT
- **Hypothesis:** A frontal transparent device can bridge graphic fields without creating a second visual world.
- **Observed result:** It integrated more convincingly than the perspective mock-up and could cross a surface boundary without an additional frame.
- **Limitations:** Test preview used a compressed import. The exact colour field and final placement are not approved.
- **Learning:** Frontal or minimally dimensional device objects are a viable candidate for selected hero moments.

## LAY-01 — Responsive Composition Architecture

- **Status:** CANDIDATE / BRIEF APPROVED FOR TESTING
- **Hypothesis:** One semantic and visual system can produce five distinct spatial compositions without treating Standard desktop as the universal master.
- **Must prove:** Compact feels intentionally sequenced; Medium enables transition; Standard supports full composition; Wide assigns function to additional width; Ultrawide activates the full stage while preserving readable text.
- **Controlled variables:** same semantic content, positioning hierarchy, navigation purpose, Constructive Poster territory and accessibility obligations.
- **Variables allowed to transform:** position, visual order, type scale, line break, information simultaneity, navigation form, media scale/crop, whitespace and statement position.
- **Test canvases:** Compact `390 × 844`; Medium `768 × 1024`; Standard `1440 × 960`; Wide `1920 × 1080`; Ultrawide `3440 × 1440`.
- **Important:** These canvases are evaluation surfaces, not approved implementation breakpoints.
- **Growth behaviours:** `Fluid` for fields and atmospheric media; `Bounded` for headlines, devices and navigation; `Readable` for body copy and captions; `Repositioned` for indices, status and secondary elements.
- **Pass:** recognisable identity across all states; Compact is not stacked desktop; Ultrawide uses the stage; reading widths remain controlled; additional width gains function; semantic sequence remains intact.
- **Fail:** Standard becomes the only correct version; every element scales proportionally; Ultrawide centres a narrow site; Compact loses plakative character; accessibility or semantic continuity breaks.
- **Next gate:** Specify and test `APP-01 / H3 — Field Leads` as five related compositions.
- **Figma link/node:** Not created yet.

## Required validation tests

### APP-01 — Home Hero

Must prove positioning, first impression, compositional authorship, navigation, accessibility and responsive re-composition.

### APP-02 — Floom Case Intro

Must prove that role, context, metadata and colourful UX evidence remain clear inside the lead territory.

### APP-03 — Gallery Spread

Must prove that heterogeneous work can coexist without identical cards, recolouring or arbitrary visual weight.

## Approval gate

A principle may move from `CANDIDATE` to `APPROVED` only when it survives the application tests relevant to its scope and Mika explicitly confirms the decision.
