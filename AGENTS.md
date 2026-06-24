# AGENTS.md

## Hard Safety Blocker

- NEVER run `homey app install -c`, `homey app install --clean`, `homey app run -c`, or `homey app run --clean`.
- NEVER pass `clean: true` to Homey devkit install/run helpers.
- These clean modes delete Homey app userdata and paired devices. Treat any request or automation path that would use them as blocked.
