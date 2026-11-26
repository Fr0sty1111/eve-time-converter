EVE Time Converter — Location Update (v3)

Replace the existing files in your GitHub repository with these updated files.

Changes:
- Replaces fixed Hobart time with the Pixel's current system timezone.
- Adds a Find my location button using browser GPS permission.
- Looks up a nearby town/city using OpenStreetMap Nominatim reverse geocoding.
- Remembers the last identified place name on this device.
- Removes the hourly conversion table.
- Keeps live clocks and UTC-to-local conversion working offline.
- Bumps service worker cache to v3 so the updated app shell is fetched.

Important:
- Enable Android automatic time zone so the phone's timezone follows travel.
- GPS permission is requested only when the user taps Find my location.
- A place-name lookup requires internet and sends coordinates to OpenStreetMap's Nominatim service.
- Timezone is read from the Pixel's system timezone. GPS coordinates alone do not provide a timezone.
- If offline or lookup fails, the app continues using the phone's timezone and last saved place name.
- Map data attribution: OpenStreetMap contributors.
