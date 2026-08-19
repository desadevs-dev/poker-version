# poker-version

Feed de versión de cliente de **BetPlay** para POKERBOT.

Una GitHub Action (cron) entra a `betplay.com.co`, extrae la versión viva del
bundle (`v:"x.y.z"`) y la publica en `version.json`. La app POKERBOT lee este
archivo para mandar el header `device: web-<versión>` correcto y evitar el
error `505 "version not supported"` cuando BetPlay actualiza.

Lectura pública: `https://raw.githubusercontent.com/desadevs-dev/poker-version/main/version.json`
