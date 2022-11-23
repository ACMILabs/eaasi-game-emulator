# ACMI x EaaSI game emulator

A centred HTML page that loads an ACMI EaaSI game emulator from its `environment-id`.

## Usage

* Find the `environment-id` of the game emulator you'd like to load in the [XOS Work](https://xos.acmi.net.au/admin/collection/work/?q=Emulation+of) field `Eaas environment id`.
* Visit https://games.acmi.net.au?id=ENVIRONMENT-ID
* The emulator should load centred in the screen
* If you visit that page without any `id` set you should see the Commodore 64 emulator

## Deployment

This HTML is deployed as an Azure Static Web App.

https://happy-pond-0c1947c00.2.azurestaticapps.net

- [x] Add ability for JavaScript to replace the `environment-id` with one from a query string
- [x] Build infrastructure with an [Azure Static Web App](https://docs.microsoft.com/en-us/azure/static-web-apps/)
- [x] Add [GitHub Action for deployment](https://docs.microsoft.com/en-au/azure/static-web-apps/build-configuration?tabs=github-actions)
- [ ] Write documentation and instructions
- [ ] Setup DNS for games.acmi.net.au
