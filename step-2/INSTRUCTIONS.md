# Step 2: Control Without Home Assistant

1. In the dashboard home press **EDIT** on the device card.
1. Make these edits so the code:

    - Comment out the `api`, `ota` and `captive_portal` sections
    - Comment out the `wifi` credentials (`ssid` and `password`)
    - Add a `web_server` section:
      ```yaml
      web_server:
        version: 3
        local: True
      ```

1. Press **INSTALL**

1. Connect your laptop to the device's Hotspot. It should be called "Worshop <unique>'s Fallback Hotspot".

1. In the device card, click **VISIT**. This will open the web server running on the device.

1. Explore the Web Server controls.

1. Explore the [REST API](https://esphome.io/web-api/#api-rest). For example:
   ```sh
   curl 'http://workshop-<unique>.local/light/board_led/turn_on?brightness=255&effect=pulse'

   curl 'http://workshop-<unique>.local/light/board_led/turn_off
   ```

<div align=right><p>

➡️ Go to [Step 3](../step-3/INSTRUCTIONS.md)

</p></div>