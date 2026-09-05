# HelixPA releases

Desktop builds for [HelixPA](https://helixpa.vercel.app).

This repository is **private on purpose**. The builds are handed out by the
site's `/api/download`, which claims one of the hundred beta seats and then
redirects to a signed URL that expires in minutes. A public release would be a
URL anyone could fetch directly, and the seat would never be claimed.

Asset names are load-bearing — `api/download.mjs` looks them up by name:

| Platform | Asset |
| --- | --- |
| Apple silicon | `HelixPA-arm64.dmg` |
| Intel Mac | `HelixPA-x64.dmg` |
| Windows | `HelixPA-Setup-x64.exe` |

Publish to the `latest` release and the site needs no change.
