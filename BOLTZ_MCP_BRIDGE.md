# LFB-1 BRIDGE: BOLTZ-1 (MCP)

This specification defines the Model Context Protocol (MCP) bridge for the Boltz-1 biomolecular interaction model.

## TOOLS

### `predict_structure`
* **Args:** `sequence` (string), `format` (FASTA)
* **Returns:** PDB data + Confidence scores.

### `dock_ligand`
* **Args:** `protein_pdb` (string), `ligand_smiles` (string)
* **Returns:** Predicted binding pose + Affinity score (kcal/mol).

---

## IMPLEMENTATION HINT
The bridge should wrap the `boltz predict` CLI command, handling FASTA generation and YAML configuration parsing on behalf of the agent.

**93.**  93.

