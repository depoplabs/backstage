---
'@backstage/plugin-kubernetes-backend': patch
---

Check if the namespace exists before listing resources. Before the list operations would throw 403 error (Forbidden). Now it is returning an empty array.