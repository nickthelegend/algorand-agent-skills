---
description: Build/compile Algorand smart contracts using AlgoKit
---

# /algo-build Workflow

<objective>
Compile smart contracts, generate ARC-56 specifications, and create typed clients for the current project.
</objective>

<process>

## 1. Verify Project

Ensure the current directory or target is an AlgoKit project. Look for `package.json` (JS/TS) or `pyproject.toml` (Python).

## 2. Execute Build

```bash
algokit project run build
```

**If build fails:**
1. Check for PuyaTs or PuyaPy compiler errors.
2. Fix contract syntax or logic.
3. Retry build.

## 3. Post-Build Actions

- Check `artifacts/` for compiled TEAL and ARC-56 specs.
- Verify typed clients are generated (e.g., `contracts/clients/`).

</process>

---

## Next Steps

/algo-test — Run your smart contract tests
/algo-deploy — Deploy your contracts to localnet
/algo-net start — Start localnet (if not running)
