# Easy PV

[![GitHub Release][releases-shield]][releases]
[![License][license-shield]](LICENSE)

[![hacs][hacsbadge]][hacs]
[![Project Maintenance][maintenance-shield]][user_profile]

Home Assistant integration for microinverters using the Easy PV app by Shanghai Electronics Way Co. and possibly other rebranded versions.

![logo][logo]

Supported devices:
- EW - Electronic Way VN2T10EU / VN2T08EU / VN2T06EU ✅
- Hatch Solar HSEU-600D/800D/1000D/HSEU-300S/400S/500S ⚠️ (Untested)
- Probably more if your app looks like this chances are it will work: ![app][app]


## Installation

### HACS (Recommended)

Installation is via the [Home Assistant Community Store
(HACS)](https://hacs.xyz/), which is the best place to get third-party
integrations for Home Assistant. Once you have HACS set up, simply click the button below or
follow the [instructions for adding a custom
repository](https://hacs.xyz/docs/faq/custom_repositories) and then
the integration will be available to install like any other.

[![Open your Home Assistant instance and open a repository inside the Home Assistant Community Store.](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=bigboot&repository=ha-easy-pv&category=integration)

### Manual

1. Using the tool of choice open the directory (folder) for your HA configuration (where you find `configuration.yaml`).
2. If you do not have a `custom_components` directory (folder) there, you need to create it.
3. In the `custom_components` directory (folder) create a new folder called `easy_pv`.
4. Download _all_ the files from the `custom_components/easy_pv/` directory (folder) in this repository.
5. Place the files you downloaded in the new directory (folder) you created.
6. Restart Home Assistant
7. In the HA UI go to "Configuration" -> "Integrations" click "+" and search for "Easy PV"

Using your HA configuration directory (folder) as a starting point you should now also have this:

```text
custom_components/easy_pv/sensor.py
custom_components/easy_pv/device_tracker.py
custom_components/easy_pv/strings.json
custom_components/easy_pv/utils.py
custom_components/easy_pv/translations
custom_components/easy_pv/translations/en.json
custom_components/easy_pv/translations/de.json
custom_components/easy_pv/quality_scale.yaml
custom_components/easy_pv/config_flow.py
custom_components/easy_pv/__init__.py
custom_components/easy_pv/model.py
custom_components/easy_pv/easy_pv/__init__.py
custom_components/easy_pv/manifest.json
custom_components/easy_pv/coordinator.py
custom_components/easy_pv/entity.py
custom_components/easy_pv/const.py
```

## Configuration is done in the UI

## Contributions are welcome!

If you want to contribute to this please read the [Contribution guidelines](CONTRIBUTING.md)

## Credits

Code template was mainly taken from [@Ludeeus](https://github.com/ludeeus)'s [integration_blueprint][integration_blueprint] template

---

[integration_blueprint]: https://github.com/custom-components/integration_blueprint
[hacs]: https://hacs.xyz
[hacsbadge]: https://img.shields.io/badge/HACS-Custom-orange.svg?style=for-the-badge
[logo]: logo.svg
[app]: app.png
[license-shield]: https://img.shields.io/github/license/BigBoot/easy_pv.svg?style=for-the-badge
[maintenance-shield]: https://img.shields.io/badge/maintainer-%40BigBoot-blue.svg?style=for-the-badge
[releases-shield]: https://img.shields.io/github/release/BigBoot/easy_pv.svg?style=for-the-badge
[releases]: https://github.com/BigBoot/easy_pv/releases
[user_profile]: https://github.com/BigBoot
