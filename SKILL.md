        ---
        name: "b02-skills-main--devops"
        description: >
          ☁️ DevOps Engineering Skills — TDD and planning skills for infrastructure-as-code, pipelines and SRE tooling.
          Derived from skills-main (mattpocock/skills). CI/CD pipelines, container orchestration, IaC, monitoring.
        version: "1.0.0"
        domain: devops
        tags: ["devops", "cloud", "docker", "kubernetes", "ci-cd"]
        source_concept: "DevOps Engineering Skills"
        license: MIT
        ---

        # ☁️ DevOps Engineering Skills

        > **TDD and planning skills for infrastructure-as-code, pipelines and SRE tooling**
        > Derived from _skills-main (mattpocock/skills)_ — real-engineering TDD and planning skills for professional developers

        ## Available Skills

        - `/iac-tdd` — TDD cycle for Terraform/Pulumi modules with terratest or policy-as-code tests
- `/pipeline-prd` — Turn CI/CD requirements into a structured PRD filed as a GitHub issue
- `/infra-to-issues` — Break infrastructure design into independently-deployable GitHub issues
- `/pipeline-design` — Design multiple CI/CD architectures with parallel agent trade-off analysis
- `/k8s-refactor` — Kubernetes manifest refactor plan with zero-downtime migration commits
- `/sre-grill` — Interview mode for SLO design and on-call procedure decisions
- `/ops-triage` — Triage infrastructure issues through runbook-linked GitHub label state machine
- `/monitoring-tdd` — TDD for alerting rules — write test cases against metric conditions first

        ## Interaction Pattern

        ```
        ① Scope    — confirm target, depth and output format
        ② Execute  — live progress with block-character bar
        ③ Findings — structured table sorted by impact
        ④ Actions  — quick wins → medium-term → strategic
        ⑤ Next     — suggested follow-up skill
        ```

        ## UI Conventions

        | Symbol | Meaning          |
        |--------|------------------|
        | ✓      | Pass / complete  |
        | ✗      | Fail / critical  |
        | ⚠      | Warning / review |
        | ⟳      | In progress      |
        | 🔴🟠🟡🟢 | Severity levels |

        Progress: `[████████░░] 80%`

        ## Quick Install

        ```bash
        cp -r . ~/.claude/skills/b02-skills-main--devops/
        # In Claude Code:
        /read ~/.claude/skills/b02-skills-main--devops/SKILL.md
        ```
