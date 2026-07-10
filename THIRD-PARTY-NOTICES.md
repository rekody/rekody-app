# Third-Party Notices — Rekody.app

Rekody.app bundles the open-source components below. Each is governed solely
by its own license, which controls for that component (see EULA §3). Copyright
remains with the respective authors.

## Bundled components

### rekody (dictation engine daemon)
- Source: https://github.com/rekody/rekody
- License: MIT — https://github.com/rekody/rekody/blob/main/LICENSE
- The bundled daemon binary is built from this repository and statically links
  its Rust crate dependencies (see below).

### Sparkle (software update framework)
- Source: https://github.com/sparkle-project/Sparkle
- License: MIT, with portions under their own permissive licenses —
  https://github.com/sparkle-project/Sparkle/blob/2.x/LICENSE

## Rust crate dependencies of the bundled daemon

The daemon statically links third-party Rust crates (MIT/Apache-2.0 and
similar permissive licenses). The authoritative inventory is the `Cargo.lock`
of https://github.com/rekody/rekody at the bundled version.

<!-- TODO before big-launch: generate the full flattened inventory with
     `cargo about generate` (or `cargo bundle-licenses`) at release-cut time,
     append it here, and bundle this file inside Rekody.app/Contents/Resources
     so MIT/Apache notice obligations travel with the binary. Track in
     release-app.sh. -->
