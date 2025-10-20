# **Inter‑Drive Dataset**

Dataset page: https://huggingface.co/datasets/wjchang/inter-drive

## **Overview**

Inter‑Drive is a large‑scale dataset of **human annotations for interactive behavior** in autonomous driving scenarios, built on top of the **Waymo Open Motion Dataset (WOMD) v1.2**. It provides fine‑grained interaction annotations for pairs of agents in complex driving scenarios.

## **Dataset Statistics**

| Split | Number of Scenes | Source Dataset |
| --- | --- | --- |
| **Training** | ~81k scenes | WOMD v1.2 Training |
| **Validation Interactive** | ~43k scenes | WOMD v1.2 Validation Interactive |

**Total**: Over 125,000 annotated interaction scenarios

## **Data Format**

### **File Naming Convention**

Each annotation file is named using the Waymo scenario ID:

```
{scenario_id}.json
```

Example: `caa55997a1842b73.json`, `1a2c6e1bfa3fee38.json`

where `scenario_id` is a 16‑character hexadecimal string that uniquely identifies each scene in WOMD.

### **JSON Structure**

Each file contains annotations for exactly two interacting agents:

```json
{
  "agent_0": {
    "track_id": 3864,
    "interact_with_other_agent": true,
    "interaction_type": "Yielding Behaviors",
    "interaction_subtype": "Pedestrian yielding to vehicles when crossing",
    "no_behavior_description": ""
  },
  "agent_1": {
    "track_id": 1514,
    "interact_with_other_agent": true,
    "interaction_type": "Passing Behaviors",
    "interaction_subtype": "Passing a Pedestrian",
    "no_behavior_description": ""
  }
}

```

### **Field Descriptions**

| Field | Type | Description |
| --- | --- | --- |
| `track_id` | int | Unique track identifier from WOMD for the agent in this scene |
| `interact_with_other_agent` | bool | Whether the agent is actively interacting with another agent |
| `interaction_type` | str | High‑level interaction category |
| `interaction_subtype` | str | Detailed behavior description within the interaction type |
| `no_behavior_description` | str | Free‑text description used only when standard categories don't apply (typically empty) |

## **Release Plan**

- [x] Example scenarios (2025‑10‑20)
- [ ] WOMD human annotations (2025‑11)
- [ ] WOMD heuristics annotations (2025‑11)
- [ ] nuPlan human annotations (2025‑11)

## **Contact**

For questions, please open an issue or contact the authors listed in `README.md`.