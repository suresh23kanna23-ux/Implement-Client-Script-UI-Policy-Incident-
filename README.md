# ServiceNow Skill Wallet - Incident Client Script & UI Policy

## Project Overview
This project implements Client Scripts and UI Policies on the ServiceNow Incident table.

## Configurations

### UI Policy
- Name: High Impact Control
- Table: Incident
- Condition: Impact is 1 - High
- Assignment Group: Mandatory
- Reverse if false: Enabled

### Client Scripts
1. Auto set urgency for high impact
2. Prevent save if Assigned To missing
3. Prevent state change via list edit

## Testing
- High Impact incidents require Assignment Group and Assigned To.
- Urgency is automatically set to High.
- Saving without Assigned To is prevented.
- State cannot be changed through list editing.
- State can be changed from the Incident form.
