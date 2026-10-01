# C-008 harmless workflow policy fixture

This public repository contains only two minimal workflows used to test a repository Actions policy:

- `c008-protected.yml` writes a uniquely named commit status when it actually executes.
- `c008-relay.yml` is an untargeted caller that invokes the protected workflow.

All markers are harmless and researcher-owned. There are no secrets, dependencies, user data, or third-party targets.
