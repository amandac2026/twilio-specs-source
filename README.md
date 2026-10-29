# twilio-specs-source

Test source repo for twilio-traceable-sync. `spec/json/` holds the ORIGINAL OpenAPI specs
(prod `*.twilio.com` server URLs). The sync workflow watches this repo, rewrites the server
URLs to `*.stage.twilio.com`, and uploads only the specs that changed.

To trigger a run, change a spec and push, for example edit `info.description` in
`spec/json/twilio_lookups_v1.json`.
