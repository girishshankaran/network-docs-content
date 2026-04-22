---
topic_id: NET-SSH-TASK-001
title: Configure SSH access
lifecycle:
  introduced_in: "19.0"
  updated_in: ["20.0"]
  deprecated_in: null
  status: active
  replaced_by: null
  applies_to: ["19.9", "20.0", "21.0"]
retrieval:
  is_canonical: true
  dedupe_key: configure-ssh-access
  allow_in_ai_results: true
---

# Configure SSH access

Use this procedure to enable SSH access on the router.

## Steps

:::version range="19.9"
1. Open **Configuration > Device Settings**.
2. Enable **SSH Server**.
3. Save the running configuration.
:::

:::version range="20.0+"
1. Open **Configuration > Security > Access**.
2. Turn on **SSH Access**.
3. Apply the policy.
:::

## Verification

Confirm that the SSH service shows as enabled in the router access summary.
