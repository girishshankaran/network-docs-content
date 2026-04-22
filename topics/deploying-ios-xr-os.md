---
topic_id: NET-IOSXR-DEPLOY-TASK-001
title: Deploying IOS-XR OS
lifecycle:
  introduced_in: "19.9"
  updated_in: ["20.0"]
  deprecated_in: null
  status: active
  replaced_by: null
  applies_to: ["19.9", "20.0"]
retrieval:
  is_canonical: true
  dedupe_key: deploy-ios-xr-os
  allow_in_ai_results: true
---

# Deploying IOS-XR OS

Use this procedure to deploy an IOS-XR OS image to supported routers in releases 19.9 and 20.0.

## Before you begin

- Download the approved IOS-XR OS image for the target router model.
- Verify that the router has enough available storage for the new image.
- Back up the running configuration before you start the deployment.
- Schedule a maintenance window because the router may restart during activation.

## Steps

1. Open **Administration > Software Management**.
2. Click **Upload Image** and select the IOS-XR OS package.
3. Wait for the checksum validation to complete and confirm the image details.
4. Click **Add to Repository** to make the image available for deployment.
5. Select the target routers from the inventory list.
6. Click **Deploy Image** and choose the uploaded IOS-XR OS version.
7. Review the deployment summary and click **Start Deployment**.
8. Monitor the progress until the routers return to an `Up` state.

## Verification

Confirm that the device inventory page shows the expected IOS-XR OS version and that the routers report a healthy status after the deployment completes.
