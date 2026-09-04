# AGENTS.md — Nordvegr 1030

This file defines the default working rules for Codex and other automated development agents in this repository.

## Project intent

Nordvegr 1030 is a historically grounded Unity project reconstructing Norway around AD 1030, beginning with Innherred / Trøndelag.

Historical plausibility matters. Do not introduce fantasy conventions, architecture, equipment, clothing, vegetation, terrain features or cultural details merely because they are common in Viking-themed media.

## Before changing anything

1. Inspect the actual repository before proposing implementation details.
2. Detect the Unity version from `ProjectSettings/ProjectVersion.txt` when it exists.
3. Inspect `Packages/manifest.json`, assembly definitions, render pipeline, input system and relevant scenes before making architectural assumptions.
4. Check whether a Unity MCP bridge is already configured before recommending or installing one.
5. Do not upgrade Unity, packages, render pipelines or tooling unless explicitly requested.
6. Read `LICENSE` and `CONTRIBUTING.md`.

## Development principles

- Prefer small, testable changes over broad rewrites.
- Preserve existing architecture and naming conventions unless there is a clear reason to change them.
- Keep gameplay systems modular so the geographic and historical scope can expand later.
- Avoid unnecessary dependencies.
- Do not silently add paid assets, proprietary SDKs, telemetry, accounts or cloud services.
- Never commit credentials, API keys, tokens, local paths or private data.
- Do not add third-party code or assets without verifying and documenting their license.
- Preserve Unity `.meta` files and GUID relationships.
- Prefer Editor-safe changes over hand-editing `.unity`, `.prefab` or `.asset` YAML.

## Historical content

When implementing historically meaningful content:

- Distinguish documented evidence from reconstruction, interpretation and speculation.
- Prefer archaeological, museum and academic sources.
- Record important source decisions in project documentation or the relevant pull request.
- If evidence is uncertain or disputed, make the uncertainty visible rather than presenting one interpretation as certain.

## Terrain and world building

- Treat real-world elevation and geographic data as source material, not automatically as a finished game world.
- Keep source datasets separate from processed Unity assets where practical.
- Preserve provenance and licensing information for imported geographic data.
- Build the initial playable area so later regions can be added without replacing the entire world pipeline.

## Validation

After code changes:

- Check compilation.
- Check Unity Console errors when Editor access is available.
- Run relevant EditMode or PlayMode tests when present.
- Verify changed scenes, prefabs and serialized references when applicable.
- Report what was actually validated and what could not be validated.

## Git workflow

- Keep commits focused and descriptive.
- Do not force-push or rewrite shared history unless explicitly requested.
- Use branches and pull requests for substantial changes.
- Do not delete user work or revert unrelated changes.

## Licensing

This project is source-available, not open source.

Do not replace the repository license with MIT, GPL, Apache, BSD or another standard open-source license unless the repository owner explicitly instructs you to do so.

Do not copy project code or assets into unrelated projects.
