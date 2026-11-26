EVE Time Converter — Location Update

Replace the existing files in your GitHub repository with these updated files.

Changes:
- Replaces fixed Hobart time with the Pixel's current system timezone.
- Adds a Find my location button using browser GPS permission.
- Looks up a nearby town/city using OpenStreetMap Nominatim reverse geocoding.
- Remembers the last identified place name on this device.
- Keeps live clocks, UTC conversion and hourly table working offline.
- Bumps service worker cache to v2 so the new app shell is fetched.

Important:
- Enable Android automatic time zone so the phone's timezone follows travel.
- GPS permission is requested only when the user taps Find my location.
- A place-name lookup requires internet and sends coordinates to OpenStreetMap Nominatim.
- If offline or lookup fails, it shows coordinates and continues using the phone's timezone.
- Timezone comes from the Pixel's system timezone. Browser GPS does not itself provide a timezone.
- OpenStreetMap attribution is included in the app footer.
