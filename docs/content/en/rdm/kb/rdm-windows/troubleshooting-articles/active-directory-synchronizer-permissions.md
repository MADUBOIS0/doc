---
eleventyComputed:
  title: Active Directory synchronizer permissions
---
{{ en.RDM }} ***Active Directory Synchronizer*** will not synchronize or find objects with ***Read permissions***.
## Solution
Make sure that the Active Directory account that will perform the synchronization has the ***Read all properties*** permission.
