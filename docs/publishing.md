# Releasing the package

The public repository is [`famfamfam/agent-market-protocol`](https://github.com/famfamfam/agent-market-protocol).
The generators and checks do not create repositories, push changes or publish releases.

## Standalone use

Move this directory to any chosen location and run the README commands from its root.
All local links, generators, schemas and tests resolve relative to this package.
Recreate its virtual environment at the new path; virtual environments are not
portable artifacts. No private material is needed.

This package has its own Git repository. GitHub runs
`.github/workflows/checks.yml` on pushes and pull requests.

## For each release

1. Run generators, `python tools/check.py` and `python -m pytest` in the package.
2. Inspect the exact files to be committed and verify the private-directory ignore
   rules. Git ignores do not prevent a filesystem archive from including local notes.
   Publish a tracked-file export, not an indiscriminate archive of the working copy.
3. Use the package repository and preserve existing remote history.
4. Check the target name, license, author attribution, draft status and schema namespace.
   The bundle uses a URN identifier and does not need network access to resolve schemas.
5. Push the reviewed files and check CI before creating a versioned prerelease tag.
   Record actual check results, not assumed success.

Do not claim an IETF submission, production deployment, independent implementation,
audited contracts or real payment integration. Issues should request concrete
counterexamples and independent implementations. Public evidence levels remain
honest: test signatures are real, external demonstration events are simulated.
