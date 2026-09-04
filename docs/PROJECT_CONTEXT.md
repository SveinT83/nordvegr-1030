# Nordvegr 1030 — Project Context

## Working concept

Nordvegr 1030 is a historically grounded Unity project set in Norway around AD 1030.

The initial development focus is Innherred / Trøndelag. The project should be structured so later areas can be added without rebuilding the technical foundation.

## Current priorities

1. Establish a clean Unity project and repository workflow.
2. Build the terrain/world pipeline from real geographic and elevation data.
3. Create a focused first playable area before expanding the full geographic scope.
4. Develop reusable historical environment assets and systems.
5. Keep desktop and possible XR/VR needs in mind without allowing platform complexity to block the first playable build.

## Geographic direction

The larger vision may expand beyond the first playable area to additional historically relevant locations in Trøndelag and elsewhere in Norway.

Do not hard-code systems around one settlement or one map tile if a reusable regional approach is practical.

## Historical direction

The project should aim for evidence-based reconstruction rather than modern "Viking fantasy" aesthetics.

For uncertain details, documentation should distinguish:

- directly documented or archaeological evidence;
- plausible reconstruction;
- deliberate gameplay compromise;
- unresolved uncertainty.

## Technical direction

- Engine: Unity.
- Repository: GitHub (`SveinT83/nordvegr-1030`).
- Automated development: Codex may be used, following `AGENTS.md`.
- Unity version, render pipeline and packages are not fixed by this document; detect them from the actual Unity project once initialized.
- Do not select or install a Unity MCP bridge until the project is inspected for an existing configuration.

## Repository role

GitHub is the canonical source for code and persistent technical/project documentation. Important decisions made outside the repository should be reflected here when they affect future implementation.
