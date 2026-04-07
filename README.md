# Service-now-
Mandatory priority process# ServiceNow UI Policy - Mandatory Field

## Objective
Make "Priority" field mandatory when "State = In Progress"

## Steps
1. Create UI Policy on Incident table
2. Set condition: State = In Progress
3. Add UI Policy Action:
   - Field: Priority
   - Mandatory: True

## Testing
- Open Incident
- Change State to "In Progress"
- Priority becomes mandatory

## Issue
Invalid Reference in Caller field

## Fix
- Go to System Security → Users
- Create new user:
  - Name: alice p
  - User ID: alice.p
- Select using lookup

## Result
Priority field is enforced as mandatory successfully
