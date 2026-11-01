# SoW Beta

Beta build of the SoW notebook-checklist PWA: **https://steph1420.github.io/sow-beta/**

- Source: [steph1420/sow](https://github.com/steph1420/sow). This repo holds no app code. Its workflow builds the tag named in `BETA_REF` with `SOW_BASE=/sow-beta/` and `VITE_SOW_FLAVOR=beta`.
- The Beta app always talks to the **TEST copy** sheet bridge (its /exec address is built in). The token is never built in; you enter it on each device or pair the device.
- Stable stays at https://steph1420.github.io/sow/ (repo `steph1420/sow`). Beta keeps its own IndexedDB (`sow-beta`) and its own settings keys, so the two apps never mix data.
- To ship a new Beta, change `BETA_REF` to the new tag and push.
