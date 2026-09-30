---
name: market-one-page-homepage
description: Use when creating or revising a concise text-first one-page homepage from a single concept or market memo, especially for Microapps. The skill preserves existing outputs, creates a separate directory for each source document or concept version, and turns market analysis into a clear landing page focused on problem, offer, method, and contact.
---

# Market One-Page Homepage

## Core Rule

Use exactly one source concept file as the basis for the page. Do not blend in other concept files unless the user explicitly asks.

Always preserve existing homepage outputs. Create a new directory for each source document or concept version.

Directory naming:

```text
codex/{source-file-name-without-extension}/
```

Example:

```text
concept/20260518-market.md
-> codex/20260518-market/
```

## Output

Create a static, build-free one-page homepage:

```text
codex/{source}/index.html
codex/{source}/styles.css
```

Do not overwrite an existing directory unless the user explicitly asks. If the target directory already exists, create a dated or numbered variant such as:

```text
codex/{source}-v2/
codex/{source}-20260518/
```

## Content Strategy

Compress the source memo into a homepage, not a report.

Prefer:

- One sharp hero sentence
- One short supporting paragraph
- Clear market pain points
- 3-4 concrete offers
- A simple method or process
- One closing statement
- Contact CTA

Avoid:

- Long analysis
- Excessive background
- Generic AI marketing language
- Feature lists that do not connect to a buyer pain
- Images unless the user asks

## Positioning Pattern

For `20260518-market.md`, use this strategic frame:

```text
정리 -> 결정 -> 실행
```

Translate the market memo into this message:

```text
People do not pay because they lack information.
They pay because they cannot organize, decide, and execute.
```

For Korean copy, keep the tone concise, direct, and commercially grounded.

Good homepage language:

- 머리 아파서 미루는 일을 정리하고, 결정하고, 실행하게 만듭니다.
- AI 도구 설명보다 실제 운영 흐름을 만듭니다.
- 가장 귀찮고 자주 미루는 업무 하나부터 봅니다.
- 방법보다 실행 흐름을 만듭니다.

## Recommended Sections

Use this structure unless the source strongly suggests a better one:

1. Hero
   - Eyebrow
   - H1
   - Lead paragraph
   - Primary CTA and secondary CTA

2. Why It Pays
   - Explain why the buyer spends money
   - Focus on execution failure, decision fatigue, and operational mess

3. Pain Points
   - 4 compact cards or columns
   - Examples: unclear problem, repetitive work, solo-operator anxiety, digital fatigue

4. Offers
   - 3-4 models from the source memo
   - Name each offer clearly
   - Include outcomes, not abstract capabilities

5. Method
   - 3-4 steps
   - Example: observe, organize, execute, maintain

6. Closing Statement
   - One memorable paragraph

7. Contact
   - Simple CTA
   - Email link if no contact details are provided: `hello@microapps.kr`

## Design Rules

Use a text-first, restrained, sophisticated design.

Default style:

- Static HTML and CSS only
- No JavaScript unless needed
- No external dependencies
- No image dependency by default
- Responsive layout
- Max content width around `1120px`
- 6-8px border radius
- Strong typography and spacing
- Neutral base palette with 2-3 restrained accent colors

Avoid:

- Hero images
- Decorative gradients
- Floating marketing cards inside cards
- Overly playful styling
- Long paragraphs on mobile
- Negative letter spacing
- Viewport-based font scaling beyond `clamp()`

## Workflow

1. Read only the requested source concept file.
2. Check existing output directories and git status.
3. Choose a new target directory derived from the source filename.
4. Create `index.html` and `styles.css`.
5. Verify files exist and report paths.
6. Mention any unrelated dirty git state without changing it.

## Copy Editing Heuristics

When converting a memo into homepage copy:

- Replace analysis headings with buyer-facing section titles.
- Convert broad observations into purchase triggers.
- Keep sentences short.
- Prefer verbs: 정리하다, 줄이다, 발견하다, 실행하다, 유지하다.
- Use concrete business examples only when they clarify the offer.
- Keep the founder/company positioning implicit unless the source demands a founder profile.

## Safety

Do not delete, move, or rewrite existing generated directories unless explicitly requested.

Do not modify source concept files.

Do not invent testimonials, customers, certifications, revenue numbers, or case studies.
