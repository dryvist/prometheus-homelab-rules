# prometheus-homelab-rules

Prometheus recording and alerting rule definitions for the homelab estate.

## Installation

Point a Prometheus or vmalert deployment's `rule_files` (or equivalent rule-group
loader) at the files under `rules/`. Which deployment loads this repository is
tracked separately — this repo holds only rule definitions, not deployment wiring.

## Usage

Each file under `rules/` is a standard Prometheus rule-group YAML file
(`groups: [{name, rules: [{record | alert, expr, ...}]}]`). Add a new file per
logical rule group rather than growing one file without bound.

## License

Apache License 2.0 — see [LICENSE](./LICENSE).
