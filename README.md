        # ☁️ DevOps Engineering Skills

        ![Domain](https://img.shields.io/badge/Domain-DevOps%20&%20Cloud%20Infrastructure-blue?style=for-the-badge)
        ![Skills](https://img.shields.io/badge/Skills-8-blue?style=for-the-badge)
        ![Workflows](https://img.shields.io/badge/Workflows-3-orange?style=for-the-badge)
        ![Source](https://img.shields.io/badge/Source-skills-main%20(mattpocock/skills)-grey?style=for-the-badge)
        ![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

        > **TDD and planning skills for infrastructure-as-code, pipelines and SRE tooling**

        Adapted from **skills-main (mattpocock/skills)** — _real-engineering TDD and planning skills for professional developers_

        ---

        ## What This Does

        CI/CD pipelines, container orchestration, IaC, monitoring.

        This collection brings the **DevOps Engineering Skills** approach to DevOps & Cloud Infrastructure work,
        providing **8 domain-specific skills** and **3 end-to-end workflows**
        with structured output and live progress tracking.

        ---

        ## Skills

        | Skill | Description |
        |-------|-------------|
        | `/iac-tdd` | TDD cycle for Terraform/Pulumi modules with terratest or policy-as-code tests |
| `/pipeline-prd` | Turn CI/CD requirements into a structured PRD filed as a GitHub issue |
| `/infra-to-issues` | Break infrastructure design into independently-deployable GitHub issues |
| `/pipeline-design` | Design multiple CI/CD architectures with parallel agent trade-off analysis |
| `/k8s-refactor` | Kubernetes manifest refactor plan with zero-downtime migration commits |
| `/sre-grill` | Interview mode for SLO design and on-call procedure decisions |
| `/ops-triage` | Triage infrastructure issues through runbook-linked GitHub label state machine |
| `/monitoring-tdd` | TDD for alerting rules — write test cases against metric conditions first |

        ---

        ## Workflows

        | Workflow | Description |
        |----------|-------------|
        | `infra-sprint` | IaC TDD sprint: design → PRD → vertical-slice implementation → review → apply |
| `pipeline-rebuild` | CI/CD rebuild: interview → design → issues → TDD → canary → full rollout |
| `sre-setup` | New service SRE setup: SLO design → alerts → runbook → on-call → test |

        ---

        ## UI Preview


```
╔══════════════════════════════════════════════════╗
║  IaC TDD Cycle  —  eks-cluster module            ║
╠══════════════════════════════════════════════════╣
║  🔴 RED    terratest: cluster creates in 15min   ║
║  🟢 GREEN  Terraform module passes test          ║
║  🔵 REFACTOR Extract reusable node-group module  ║
╚══════════════════════════════════════════════════╝

Slice #2/5: "node group scales on CPU > 70%"
  Test result: ✓ PASS (HPA fires within 90s)
  Coverage: autoscaling policy, IAM roles, CloudWatch alarms
  Next: "cluster upgrades without downtime"
```

        ---

        ## How It Works

        Every skill follows the same 5-step interaction:

        ```
        ① Scope Confirmation   verify target + options
        ② Live Progress        [████████░░] 80%
        ③ Structured Findings  table sorted by impact (🔴🟠🟡🟢)
        ④ Action Plan          quick wins → medium-term → strategic
        ⑤ Next Steps           suggested follow-up skills
        ```

        ---

        ## Install

        ```bash
        # Copy to Claude skills directory
        cp -r . ~/.claude/skills/b02-skills-main--devops/

        # Load in Claude Code session
        /read ~/.claude/skills/b02-skills-main--devops/SKILL.md
        ```

        ## Source

        Derived from **skills-main (mattpocock/skills)** — real-engineering TDD and planning skills for professional developers.
        Original patterns adapted and domain-specialised for DevOps & Cloud Infrastructure.

        ---
        MIT License
