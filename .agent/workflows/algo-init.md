---
description: Initialize a new Algorand project using AlgoKit
---

# /algo-init Workflow

<objective>
Bootstrap a new Algorand smart contract project or dApp using the official AlgoKit templates.
</objective>

<process>

## 1. Gather Project Details

Ask the user for the following information:
- **Project Name:** (e.g., `my-voting-app`)
- **Template:** (TypeScript [default], Python, React, etc.)
- **Preset:** (Production [default], Starter)
- **Author:** (Optional)

## 2. Execute Initialization

Run the appropriate `algokit init` command.

**Example for TypeScript (Production):**
```bash
algokit init -n <project-name> -t typescript --answer preset_name production --defaults
```

**Example for Python (Production):**
```bash
algokit init -n <project-name> -t python --answer preset_name production --defaults
```

## 3. Post-Initialization

Once the project is created:
1. `cd <project-name>`
2. Show the project structure.
3. Suggest next steps (build, test).

---

## Next Steps

/algo-build — Compile your new smart contracts
/algo-net start — Start a local Algorand network for testing
/algo-deploy — Deploy your contracts to localnet
</process>

<related>
## Related
### Skills
- `create-project` — Detailed initialization logic
- `use-algokit-cli` — Command reference
</related>
