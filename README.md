# Pivot Pyramid Plugin for Claude Code

A Claude Code plugin that turns Claude into a startup pivot advisor using the **Pivot Pyramid framework** — a strategic framework for knowing what to change, when to change it, and how to execute without destroying what works.

Created by [Selcuk Atli](https://selcukatli.com) (YC W14, 500 Startups Venture Partner).

## What It Does

When you describe your startup or ask about pivoting, the plugin activates a guided diagnostic interview that:

1. **Maps your startup** onto the five layers of the Pivot Pyramid (Customers → Problem → Solution → Technology → Growth)
2. **Scores each layer** (1-5) based on evidence strength and health signals
3. **Identifies the broken layer** — traces symptoms to root causes, not surface problems
4. **Recommends action** — persist, optimize, or pivot — with the right playbook, cascade analysis, and real-world case studies
5. **Helps plan the pivot** with templates for planning, success criteria, and stakeholder communication

## The Framework

The Pivot Pyramid breaks every startup into five layers:

```
    ┌─────────┐
    │ Growth  │  ← Changes most frequently, zero cascade
    ├─────────┤
    │Technology│
    ├──────────┤
    │ Solution  │
    ├───────────┤
    │  Problem   │
    ├────────────┤
    │  Customers  │  ← Foundation, changes cascade through everything
    └─────────────┘
```

**Lower layers are more fundamental.** A Customer pivot affects all four layers above. A Growth pivot affects nothing below. Most startup failures come from either **over-pivoting** (changing everything) or **under-pivoting** (tweaking the surface while the foundation is broken).

## Install

```bash
claude install-plugin github:Selcukatli/pivotpyramid-plugin
```

## Usage

Just describe your situation naturally. The skill triggers automatically when you say things like:

- "Diagnose my startup"
- "Should I pivot?"
- "We can't retain users"
- "Our CAC is too high"
- "Why aren't we growing?"
- "What layer is broken?"
- "Should we change direction?"

The plugin remembers your startup profile across sessions (saved to `.pivot-pyramid/startup-profile.md`), so you can pick up where you left off.

## What's Inside

```
skills/pivot-advisor/
├── SKILL.md                              # Core diagnostic flow
└── references/
    ├── five-layers.md                    # Layer definitions + validation questions
    ├── cascade-rules.md                  # How changes ripple through layers
    ├── diagnostic-scorecard.md           # Scoring framework + interview guide
    ├── case-studies.md                   # 20+ real pivots (Slack, Instagram, Netflix...)
    ├── pivot-playbooks.md               # Step-by-step execution per pivot type
    ├── planning-templates.md            # 8 practical tools and templates
    └── common-traps.md                  # Over-pivot, under-pivot, when NOT to pivot
```

~10,000 words of framework knowledge with progressive disclosure — the core skill stays lean, detailed references load only when relevant.

## Based On

*[The Pivot Pyramid: A Founder's Complete Guide to Strategic Startup Experimentation](https://pivotpyramid.com)* by Selcuk Atli.

The book covers the full framework across 14 chapters: diagnosis, execution playbooks for each pivot type, multi-layer pivots, building pivot-ready culture, and a complete toolkit with templates and case studies.

## License

MIT
