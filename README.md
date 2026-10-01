# C-008 harmless workflow policy fixture

This public repository contains only two minimal workflows used to test a repository Actions policy:

- `c008-protected.yml` uses the `c008-protected` environment and writes a uniquely named commit status containing an HMAC only when it actually receives the environment secret and executes.
- `c008-relay.yml` is an untargeted caller that invokes the protected workflow.

All messages and markers are harmless and researcher-owned. The environment key is never printed or persisted outside GitHub's encrypted secret store; only one-way HMAC values are retained. There are no third-party targets.
