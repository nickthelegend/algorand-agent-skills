---
description: Run your Algorand smart contract tests
---

# /algo-test Workflow

<objective>
Execute the project's test suite to verify smart contract behavior.
</objective>

<process>

## 1. Verify Environment

Ensure:
1. Building is complete (`algokit project run build`).
2. Localnet is started (if tests require a live network).

## 2. Execute Tests

```bash
algokit project run test
```

**If tests fail:**
1. Check test logs for failed assertions.
2. Debug contract or test code.
3. Fix and retry.

## 3. Post-Test Actions

- Check for any failed test cases.
- Use `algokit localnet logs` if diagnosing network behavior.

</process>

---

## Next Steps

/algo-deploy — Deploy your contracts to localnet or testnet
/algo-build — Re-build your contracts after updates
/algo-net status — Check localnet state
