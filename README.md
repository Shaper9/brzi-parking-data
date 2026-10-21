# Brzi Parking zone data

Signed parking-zone data for the Brzi Parking app, served with GitHub Pages.

- `v1/<city>/manifest.json`: the newest zone file for a city, its SHA-256 and an Ed25519 signature.
- `v1/<city>/zones/<version>.json`: the zone files. They never change once published.

The app downloads these files at most once a day and uses one only if the signature, the
SHA-256 and its own full check all pass. Files here are written by the app's zone pipeline
(`zone-pipeline sign` and `zone-pipeline publish`); don't edit them by hand.

Contact: brziparking@gmail.com
