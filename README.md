## Foo (caller) - secret forwarding to bar reusable workflow

This repo is the **caller** for TASK-001-1.

### Setup

- Create a repo secret named **`FOO_DEPLOY_TOKEN`**

### Run

- Run the workflow **“Call Bar with Foo Secrets”** (`.github/workflows/call-bar-with-foo-secrets.yml`)
- Select an `environment` (staging/production)

The workflow calls `poc-federated-patterns/bar`’s reusable workflow and forwards `FOO_DEPLOY_TOKEN` as `DEPLOY_TOKEN`.


