# publish-classic-fixture

A **test fixture** for publishing on 3-Torus ("Publish your app" in the portal).

It is a *classic* repository on purpose: it is not adapted to 3-Torus, so it has
no `.3torus/app.yaml` (only the `adapted` control variant adds one). Keep it
that way; the publishing tests depend on it.

**Variant on this branch: `compose`** — a compose file whose first service names a public image, and a Dockerfile.

The content of this branch is replaced, one ordinary commit at a time, by
`scripts/publish-fixture-variant.sh` in the 3-Torus platform repository. Do not
edit it by hand: the next switch overwrites the edit.

The app is [podinfo](https://github.com/stefanprodan/podinfo)
(`ghcr.io/stefanprodan/podinfo:6.7.1`, port 9898). Nothing here is a secret,
and nothing ever should be.
