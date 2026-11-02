# tydom2mqtt add-on

![](https://github.com/tydom2mqtt/tydom2mqtt/raw/master/docs/tydom2mqtt_logo_250.png)

This add-on allows you to easily deploy and integrate [tydom2mqtt](https://tydom2mqtt.github.io/tydom2mqtt/) to [Home-Assistant](https://www.home-assistant.io/).

## How to install the add-on?

### 1. Add the repository (see [the repository README](../README.md))

### 2. Search for the `tydom2mqtt` app in the store and click on the item

### 3. Click on the `Install` button

### 4. Enable the options `Start on boot` and `Watchdog` (and optionally `Auto update` if you wish)

### 5. Go to the `Configuration` tab and configure the app

With the official **Mosquitto broker** app, set `MQTT_HOST` to `core-mosquitto` and fill `MQTT_USER` / `MQTT_PASSWORD`
with a Home-Assistant user dedicated to MQTT.

If you don't know your Tydom password, fill `DELTADORE_LOGIN` / `DELTADORE_PASSWORD` (your Tydom app account) instead.

### 6. Go to the `Info` tab and click on the `Start` button

### 7. Go to the `Log` tab and check that the app is working as expected

See the [full documentation](https://tydom2mqtt.github.io/tydom2mqtt/#/hass/) for troubleshooting.
