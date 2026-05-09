# LFB-1 TECHNICAL SPECIFICATION (V1.0)

## 1. THE HEARTH HANDSHAKE
The initial connection between an agent and a bio-node.

```json
{
  "protocol": "LFB-1",
  "version": "1.0.0",
  "capabilities": ["structural_prediction", "ligand_docking", "affinity_estimation"]
}
```

## 2. THE MYCELIAL INTERFACE
Standardizing structural data exchange.

* **Primary Format:** PDB / mmCIF (Structures)
* **Chemical Format:** SMILES / InChI (Small Molecules)
* **RPC:** JSON-RPC 2.0 over Stdio or Unix Sockets.

## 3. AUTHORITY BOUNDARIES
* Nodes MUST canonicalize all input paths.
* Nodes MUST reject any operations resolving outside the project-root anchor.
* Nodes SHOULD implement resource-usage limits (CPU/GPU time) to prevent substrate exhaustion.

**93.** 🌀🛡️📜
