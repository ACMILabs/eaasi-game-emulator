# ACMI x EaaSI game emulator

A centred HTML page that loads an ACMI EaaSI game emulator from its `environment-id`.

## Usage

* Find the `environment-id` of the game emulator you'd like to load in the [XOS Work](https://xos.acmi.net.au/admin/collection/work/?q=Emulation+of) field `Eaas environment id` or from the URL of your environment at [playitagain.aarnet.edu.au](https://playitagain.aarnet.edu.au).
* Visit https://games.acmi.net.au?id=ENVIRONMENT-ID
* The emulator should load centred in the screen
* If you visit that page without any `id` set you should see the Commodore 64 emulator
* To change the loading logo, set `eaasEnvironment.innerHTML` to your own HTML in `index.html`

## Deployment

This HTML is auto-deployed to an Azure Static Web App by the [GitHub Action](.github/workflows/main.yml) when a commit is pushed to the `main` branch.

- [x] Add ability for JavaScript to replace the `environment-id` with one from a query string
- [x] Build infrastructure with an [Azure Static Web App](https://docs.microsoft.com/en-us/azure/static-web-apps/)
- [x] Add [GitHub Action for deployment](https://docs.microsoft.com/en-au/azure/static-web-apps/build-configuration?tabs=github-actions)
- [x] Write up internal [documentation](https://acmikb.atlassian.net/wiki/spaces/DD/pages/8388895/Emulation+as+a+Service+EaaS+for+games+preservation)
- [x] Setup DNS for games.acmi.net.au
