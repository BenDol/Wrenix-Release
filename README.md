# Agent Cohort release-stub branch

Release tags (`staging-edge`, `bleeding-edge`, `vX.Y.Z`) in this
repository are pinned to the single commit on this branch.

GitHub auto-attaches "Source code (zip)" and "Source code (tar.gz)" to every
release based on the underlying tag's commit. By pinning every release tag to
this stub, those auto-generated archives contain ONLY this README — not the
project source. Project source is proprietary and is not distributed through
the release pages.

End-user installers and update channel manifests are uploaded as release
assets (Setup.exe, .dmg, .AppImage, .deb, .rpm, plugins.zip, *.yml, *.sha256,
*.blockmap, *-sha.txt).

This branch is managed by `scripts/pin-release-tag-to-stub.mjs`. The pinning
step in `.github/actions/pin-release-tag-to-stub/` auto-creates this branch
on first use. Do not push additional commits here.
