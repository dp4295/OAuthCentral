# Systems:

## Phase 1:

### Tenant Registration:
  - A tenant can be an internal group seeking to implement an authentication mechanism for their specific unit.
  - Tenant request via registration interface, initially the registration will be handle through a JSON request. Registration will require to be approved by OAuth  Team member. 
  - All the registeration will have a queued in will be process one by one. 
  - Requester can see the process using order id (In-Process, Submitted, Approved, Dis-Approved). 
  - History of all the submission by tenant needs to be pre-serve for audit and providing past information. 
  - Once the OAuth Team approved the Tenant, the data will be create in key-store and isolated Dynamo DB will be generated for the Tenant. 


## Phase 1: Tenant Registration
### Tenant Registration:
- Definition of a Tenant: A tenant represents an internal group seeking to implement an authentication mechanism tailored to their specific needs.

- Registration Interface:
  - Tenants can register through a dedicated interface, initially handled via a JSON-based request.
  - The registration request will include all necessary tenant details and configuration preferences.
- Approval Process:
  - Each tenant registration request must be approved by a designated member of the OAuth team before the tenant is fully onboarded. 
  - The registration requests will be queued and processed sequentially, ensuring orderly and consistent processing.
- Status Tracking:
  - The requester can track the status of their registration request using an order ID, with possible statuses including "In-Process," "Submitted," "Approved," and "Disapproved."
- Audit and History:
  - A complete history of all tenant registration submissions must be preserved for audit purposes, allowing the OAuth team and tenants to review past information and decisions.
- Post-Approval Actions:
  - Once a tenant's registration is approved:
  A secure key-store entry will be created for the tenant.
  An isolated DynamoDB instance or table will be generated for the tenant to ensure data segregation and security.