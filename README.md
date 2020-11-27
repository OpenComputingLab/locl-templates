# locl-templates
Portainer templates feeds for lOCL environments

---
## About

Feeds for listing custom *App Templates* inside *portainer* UI.

Connect to the `raw` file to consume a feed according to the URL pattern:

`https://raw.githubusercontent.com/OpenComputingLab/locl-templates/main/TEMPLATE_FEED_NAME.json`

For example:

- the `ou-templates.json` template can be found at: `https://raw.githubusercontent.com/OpenComputingLab/locl-templates/main/ou-templates.json`

Example:

`docker run -d -p 80:8000 -p 9000:9000 --name=portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock portainer/portainer-ce --templates https://raw.githubusercontent.com/OpenComputingLab/locl-templates/main/ou-templates.json --logo https://github.com/OpenComputingLab/locl-templates/raw/main/logos/OU-logo-83x65.png`
