# OpenStreetMap state packs

One file per US state (`VA.json`, …) with the river launches, the parking beside them and along rivers,
campsites, and dams and weirs that Bear River shows on its map, plus `index.json`, which lists each pack,
when it was built and the box its places fill. The app downloads a state's pack the first time a river
there is opened and keeps it for use with no signal. Pennsylvania, New Jersey, New York, Delaware and
Maryland are built into the app instead.

Built from Geofabrik's state extracts by `ios/scripts/fetch_osm_access.py --pack` in the app's repo, not
from live Overpass queries.

**Licence:** © OpenStreetMap contributors. These packs are a derived database of OpenStreetMap data and are
available under the [Open Database License 1.0](https://opendatacommons.org/licenses/odbl/1-0/). See
<https://www.openstreetmap.org/copyright>. The app credits OpenStreetMap contributors wherever it shows them.
