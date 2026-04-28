        # ☁️ Examples — DevOps Engineering Skills

        ## Quick Command Example

        ```bash
        /iac-tdd my-target --output md
        ```

        **Output:**


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

        ## Workflow Example

        ```bash
        /workflows:infra-sprint my-target --scope full
        ```

        ```
        ╔══════════════════════════════════════════════════════════╗
        ║  Step 1/5  Discovery   ✓  Done                          ║
        ║  Step 2/5  Analysis    ✓  Done                          ║
        ║  Step 3/5  Planning    ⟳  Running …                    ║
        ║  [████████████░░░░░░]  60%   ETA ~12 min                ║
        ╚══════════════════════════════════════════════════════════╝
        ```

        ## Tips

        1. Start with `/iac-tdd` for a quick overview.
        2. Use `--scope quick` for fast scans, `--scope full` for production.
        3. Chain: run analysis first → use findings as input for planning.
        4. `--output html` generates a stakeholder-ready report.
