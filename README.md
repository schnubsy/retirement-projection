# Retirement projection — public build

A self-contained, single-file retirement projection dashboard. Open `index.html` in any
modern browser: it runs entirely client-side with **no server, no network and no build step**.

## Privacy

This artifact carries **ZERO personal data**. It ships with an empty plan template; every figure
you see is one you enter yourself, held only in your own browser's local storage. Nothing is
uploaded anywhere. (The build is verified by an automated, derived sentinel scan before release.)

## Using it

Open the page, then create a plan from scratch or import a plan file. Plans are separate profiles
on this browser — this is not a password: anyone using this browser can open any plan.

## Optional sync

You can optionally sync one plan across your own devices. If you turn it on, the plan is
AES-GCM encrypted **in your browser** with a passphrase that never leaves your device; only
unreadable ciphertext is stored, keyed by an unguessable id. No network request is made until
you explicitly enable sync. Lose the id or the passphrase and the synced copy cannot be recovered.

## About

Auditable, rules-based tax modelling (every headline number traces to a source). Built from a
modular engine into one self-contained file. Released via `tools/release.js` from the private
source repository — this public repository contains only the built artifact.

The **same built artifact** is published in two places from `tools/release.js`: this standalone
repository (served by GitHub Pages) and the `press` marquee as `retirement.html`. They are kept
byte-for-byte in step — refresh both from the same `dist/index.html`.

