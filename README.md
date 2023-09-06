# ESP CherryUSB Fork

[![Component Registry](https://components.espressif.com/components/leeebo/cherryusb/badge.svg)](https://components.espressif.com/components/leeebo/cherryusb)

This is a fork of [CherryUSB](https://github.com/cherry-embedded/CherryUSB), which is a tiny and portable USB Stack (device & host) for embedded system with USB IP.

This fork repository is wrapped as an ESP-IDF component and finally publish to [ESP-IDF Component Registry](https://components.espressif.com/components/leeebo/cherryusb).

This component can not be built as a standalone library, it is only used as a dependency of the [cherryusb_esp32](https://github.com/leeebo/cherryusb_esp32) component.

## How to use

### Use this component together with [cherryusb_esp32](https://github.com/leeebo/cherryusb_esp32).

Just add ``idf_component.yml`` to your main component with the following content::

```yaml
## IDF Component Manager Manifest File
dependencies:
  leeebo/cherryusb_esp32: "*"
```

Or simply run:

```
idf.py add-dependency "leeebo/cherryusb_esp32"
```

During the build process, the ESP-IDF build system will automatically download and install this component.

## API Documentation

1. Library introduction can be found on [README](https://github.com/cherry-embedded/CherryUSB#readme) from the upstream CherryUSB.
2. Full API code documentations and step by step guides can be found in [CherryUSB Docs Website](https://cherryusb.readthedocs.io/).