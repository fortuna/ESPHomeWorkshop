# Getting Started With ESPHome: From Zero to Cool

In this workshop you will learn how to use ESPHome to program IoT devices.

This is being presented at HOPE_16

Wiki: https://wiki.hope.net/index.php/Getting_Started_With_ESPHome_Workshop


## Setup

1. **Install ESPHome**: This is the most important and problematic step. Please follow the instructions in [Installing ESPHome Manually](https://esphome.io/guides/installing_esphome.html).

    - On macOS:
      ```sh
      brew install esphome
      ```

    - On Linux:
      ```sh
      sudo apt install python3.13-venv
      python3 -m venv venv
      source venv/bin/activate
      ```

      You may need to give your user access to the serial ports:
      ```sh
      sudo usermod -a -G dialout $USER
      ```

    - On Windows:
      [Install Python](https://www.python.org/downloads/) if you don't have it already. Then:
      ```
      pip3 install wheel
      pip3 install esphome
      ```

1. **Create a folder** for your workshop code and enter it. For example:

    ```bash
    mkdir esphome && cd esphome
    ```

1. **Start and open the ESPHome Dashboard**. Run:

    ```bash
    esphome dashboard --address localhost --open-ui ./
    ```

Your browser should open http://localhost:6052/ and look like this:

<div align=center>
  
  <img width="563" height="320" align="center" alt="image" src="https://github.com/user-attachments/assets/9ed0ca11-367a-46d9-853e-db6cd1a0ff52" />
  
</div>

<div align=right><p>

➡️ Go to [Step 1](step-1/INSTRUCTIONS.md)

</p></div>
