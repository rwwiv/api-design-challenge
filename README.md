# API Design Challenge

## Prompt

Design an API execution platform which sits between applications on one side and databases on the other side.
 
This platform:
- Takes requests in the form of APIs from applications
- Converts the API requests into DB queries
- Executes these queries against the DB
- Gets responses back from the DB
- Buffers the response, deserializes the data and sends responses back to the API callers
 
### Design parameters

- Needs to be a multi-tenant system with the ability to scale to millions of tenants (each with a set of applications) handling billions of API calls across them
- SaaS platform built using cloud-native technologies
- Need to be highly performant - introduce the least possible latency between the application to DB and DB back to the application
- Needs to be highly reliable/available and highly fault-tolerant with the ability to offer guaranteed SLAs to users
- Designed to be highly secure
