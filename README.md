# ESP CherryUSB Fork

This is a fork of [CherryUSB](https://github.com/cherry-embedded/CherryUSB), which is a tiny and portable USB Stack (device & host) for embedded system with USB IP.

This fork repository is wrapped as an ESP-IDF component and finally publish to [ESP-IDF Component Registry](https://components.espressif.com/).

This component can not be built as a standalone library, it is only used as a dependency of the [esp_cherryusb](https://github.com/leeebo/esp_cherryusb) component.

## How to use

### Use this component together with [esp_cherryusb](https://github.com/leeebo/esp_cherryusb).

Just add ``idf_component.yml`` to your main component with the following content::

```yaml
## IDF Component Manager Manifest File
dependencies:
  esp_cherryusb: "*"
```

Or simply run:

```
idf.py add-dependency "esp_cherryusb"
```

During the build process, the ESP-IDF build system will automatically download and install this component.

## API Documentation

1. Library introduction can be found on [README](https://github.com/cherry-embedded/CherryUSB/blob/master/README.md) from the upstream CherryUSB.
2. Full API code documentations and step by step guides can be found in [CherryUSB Docs Website](https://cherryusb.readthedocs.io/).