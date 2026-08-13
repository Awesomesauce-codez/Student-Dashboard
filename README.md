# BusTrack — School Bus Tracking Prototype

A mobile-friendly school bus tracking prototype for students, parents, drivers, and school admins.

## Current prototype
- Live fleet map using Leaflet + OpenStreetMap
- Three demo buses with moving positions
- Bus status and estimated arrival times
- Route 27 stops and route line
- Responsive parent/student view
- Role selector for future parent/admin/driver experiences
- Clearly labeled DEMO MODE so no real student location is implied

## Backend foundation
The connected Supabase project now has tables for schools, buses, routes, stops, and bus_locations. The frontend currently uses simulated positions so it works immediately without exposing credentials or real student data.

## Next production steps
1. Add verified school/parent authentication with Supabase Auth.
2. Connect an authorized GPS feed from the district's bus tracking hardware.
3. Store live positions in `bus_locations` and subscribe with Supabase Realtime.
4. Restrict each parent/student to their assigned route.
5. Add school-admin fleet management and driver controls.
6. Deploy the static frontend through Vercel.

## Run it
Open `index.html` directly, or deploy the repository as a static site. Internet access is required for the map tiles and Leaflet library.

> This prototype uses simulated bus locations only. Do not connect real student or vehicle tracking data until authorization, authentication, privacy controls, and district policies are in place.
