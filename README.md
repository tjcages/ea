# EA — Executive Assistant

Give routine work to scripts and bounded JEV decisions. Keep judgment and verification with your main agent.

## Install

```sh
npx skills add tjcages/ea
```

## Use

Ask your agent:

- “Use EA to check these links. Report only broken ones.”
- “Use EA to find the best browser skill for this task.”
- “Use EA to group these errors by severity.”

Known operations use deterministic tools. JEV selects among explicit options;
your agent executes and verifies the result. Your existing JEV connection takes
precedence. Cloudflare is the recommended default when none is configured.

## Update

```sh
npx skills update
```

[Read the skill](SKILL.md) · [Reviewed catalogue](references/jev-catalogue.md) · [Website](https://offbr.co/skills/ea)

Python 3.11+ is needed only for the bundled Cloudflare client. Source monitoring
also needs GitHub CLI. Neither monitoring nor computer access is installed automatically.
See [maintenance](references/maintenance.md) for opt-in checks.

## Verification

```sh
python3 -m unittest discover -s scripts -p 'test_*.py'
```

Client regression tests and limited supervised Cloudflare pilots are verified.
General unattended operation and net token savings are not established.
Third-party catalogue entries retain their own installation and testing status.

## Distribution

This repository is the public EA release mirror. Authoring currently lives in
`offbr/public/agent-skills/ea`; releases synchronize this folder and the website
archive together. Do not edit competing copies independently.
