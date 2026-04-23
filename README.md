# network-docs-content

Canonical content repo for the production Option 2 model.

This repo stores:

- canonical topics
- reusable snippets
- content schemas
- content validation scripts

This repo does not store:

- release TOCs
- release manifests
- release metadata
- publishing configuration

Publishing is driven from the companion repo:

- `network-docs-releases`

Authoring flow:

- create new topics with `node scripts/create-topic.js --title "Topic title" --release "20.0"`
- the script assigns a system-generated `topic_id`
- CI validation remains strict on `main`
- local draft validation can allow missing `topic_id` with:
  - `ALLOW_MISSING_TOPIC_ID=true node scripts/validate-content.js`
