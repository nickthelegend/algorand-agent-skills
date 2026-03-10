---
description: Manage your local Algorand network using AlgoKit
argument-hint: "[start | stop | reset | status | logs]"
---

# /algo-net Workflow

<objective>
Manage the local Algorand network (localnet) for testing and development.
</objective>

<process>

## 1. Parse Arguments

Extract from $ARGUMENTS (the command):
- `start` — Start localnet (default if none provided)
- `stop` — Stop localnet
- `reset` — Clear state and restart
- `status` — Check status
- `logs` — View logs

## 2. Execute Command

**If `start` (or none):**
```bash
algokit localnet start
```

**If `stop`:**
```bash
algokit localnet stop
```

**If `reset`:**
```bash
algokit localnet reset
```

**If `status`:**
```bash
algokit localnet status
```

**If `logs`:**
```bash
algokit localnet logs
```

## 3. Post-Action

Display the current status using:
```bash
algokit localnet status
```

</process>

---

## Next Steps

/algo-build — Re-compile contracts
/algo-deploy — Deploy to the running localnet
/algo-test — Run tests against the network
