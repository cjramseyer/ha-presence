# ha-presence
Home Assistant Presence configuration

This repository is specifically created to share all the pieces of my presence configuration and automation in Home Assistant.
There are several primary components.

1.  Device trackers via Google Location Sharing
2.  Several Input booleans for each individual and some general control points
3.  NodeRed for the automations

Some notes about my setup:

- I use the Google Maps integration, because, in my experience, it was faster, more accurate than the companion app, and didn't require anything to be installed (my kids didn't need the HA companion app on their phones).
- I wanted to track a variable number of people.  This started with 4 (me, fiance, and 2 kids), plus guest(s).  This solution enables me to have any number of people/devices.
- I wanted the ability to identify each individual, whether the house was occupied or not overall including the number of people home, plus accounting for times when we might have guests, so we can have automations that do or do not run when there are guests in our house.
- I use NodeRed for all automations in my SmartHome.  This was an easy integration, and enables me to duplicate presence changes for individuals very easily.

This is my primary automation because presence in the house is key to when and if certain other automations should run.  For example, while the exterior lights will be turned on at sundown whether we are home or not, there is not reason to turn on the interior lights if we aren't here.

This repository is so that I can share all the components for this (google maps, devices, input booleans and sensors, and automations) in one place where you can use any or all of it in your own setup.

Please note that this is NOT my entire HA setup, which is available (minus secrets) in another repo, and my automations are available in my NodeRed repo.
This is simply all the parts to do presence.
