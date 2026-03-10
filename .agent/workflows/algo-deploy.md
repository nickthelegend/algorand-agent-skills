---
description: Deploy your Algorand smart contracts using AlgoKit
---

# /algo-deploy Workflow

<objective>
Deploy compiled smart contracts to a specified network (localnet, testnet, or mainnet) using AlgoKit.
</objective>

<process>

## 1. Verify Build

Check if smart contracts are built (`algokit project run build`).

## 2. Confirm Target Network

Ask the user: "Where do you want to deploy?"
- **localnet** (default)
- **testnet**
- **mainnet**

## 3. Verify Localnet (if target)

If deploying to localnet, ensure it's running:
```bash
algokit localnet start
```

## 4. Execute Deployment

```bash
algokit project deploy <network>
```

**If deployment fails:**
1. Check network connection/status.
2. Verify account balances (if testnet/mainnet).
3. Review deployment logs.

## 5. Post-Deployment

- Confirm the App ID of the deployed contract.
- Provide links to explorers (if testnet/mainnet).

</process>

---

## Next Steps

/algo-test — Test your deployed contracts
/algo-net status — Check localnet state
/algo-net stop — Stop localnet
