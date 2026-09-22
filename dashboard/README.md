# Command Center (Dashboard)
The visibility and control layer for Operon, where humans see what the agents are doing and approve or reject their generated drafts.

- Dashboards giving visibility across the business
- Role-based access for internal FA Systems roles
- An approval queue where every agent-generated draft waits for a named person to accept or reject before moving further
- An audit log view: every generated artifact tied to its inputs and its approver

### Design
- Nothing an agent produces takes effect without going through this approval flow
- Every approval/rejection is logged
- Access is role-based
