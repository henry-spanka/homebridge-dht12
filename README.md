[Install Homebridge]: https://github.com/nfarina/homebridge#installation
[Configuration]: #Configuration


# homebridge-dht12

Homebridge accessory plugin to read DHT12 sensors via I2C bus.

[![NPM](https://nodei.co/npm/homebridge-dht12.png?compact=true)](https://npmjs.org/package/homebridge-dht12)

# Features
* Read Temperature and Humidity from DHT12 sensor via I2C.
* Display fault if sensor is unavailable.

# Setup / Installation
1. [Install Homebridge]
2. `npm install homebridge-dht12`
3. Edit `config.json` and configure accessory. See [Configuration](#configuration) section.
4. Start Homebridge
5. Star the repository ;)

# Configuration

To configure the plugin add the following to the accessories section in `config.json`.
The i2cAddresses must be in Hex Format, preceded by `0x`.

```json
{
    "accessory": "I2C_DHT12",
    "name": "Kitchen",
    "i2cAddress": "0x5c",
    "i2cDevice": "/dev/i2c-1",
    "updateFrequency": "60"
}
```

# Help
If you have any questions or help please open an issue on the GitHub project page.

# Contributing
Pull requests are always welcome. If you have a device that is not supported yet please open an issue or open a pull request with
your modifications.

# License
The project is subject to the MIT license unless otherwise noted. A copy can be found in the root directory of the project [LICENSE](LICENSE).
