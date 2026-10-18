# Add a native Plasma widget and installable Linux AppImage

Adds a KDE Plasma dock widget and packages the general Tauri UI as an installable,
updatable AppImage; both use the existing daemon.

- KDE: themed battery/ANC controls, EQ editing, device management, settings and a battery-ring icon.
- Tauri: resizable, pinnable three-tab panel with matching controls, automatic preferred-device saving and dismissible errors.
- Backend/packaging: validated BlueZ renaming with shared D-Bus updates, Arch KDE recipe, AppImage installer/update metadata, release workflow and tests.

Validated: Rust workspace, Tauri, frontend, installer and KDE offscreen tests;
local AppImage build/checksum. Live audio tests, KDE D-Bus integration, clean-distro
installation and the GitHub release workflow still need external validation.

<details>
<summary>Screenshots: KDE light/dark and Tauri</summary>

Demo device data. KDE uses the shared QML panel; Tauri uses its real frontend in
Firefox. See [capture instructions](screenshots/README.md).

| Feature | KDE light | KDE dark | Tauri |
| --- | --- | --- | --- |
| Controls | <img src="screenshots/kde-controls.png" width="220" alt="KDE light controls"> | <img src="screenshots/kde-dark-controls.png" width="220" alt="KDE dark controls"> | <img src="screenshots/tauri-controls.png" width="220" alt="Tauri controls"> |
| EQ editor | <img src="screenshots/kde-equalizer.png" width="220" alt="KDE light EQ editor"> | <img src="screenshots/kde-dark-equalizer.png" width="220" alt="KDE dark EQ editor"> | <img src="screenshots/tauri-equalizer.png" width="220" alt="Tauri EQ editor"> |
| Devices | <img src="screenshots/kde-devices.png" width="220" alt="KDE light devices"> | <img src="screenshots/kde-dark-devices.png" width="220" alt="KDE dark devices"> | <img src="screenshots/tauri-devices.png" width="220" alt="Tauri devices"> |
| Settings/About | <img src="screenshots/kde-settings.png" width="220" alt="KDE light settings"> | <img src="screenshots/kde-dark-settings.png" width="220" alt="KDE dark settings"> | <img src="screenshots/tauri-settings.png" width="220" alt="Tauri settings"> |

Tray icons:

| KDE light | KDE dark | Tauri |
| --- | --- | --- |
| <img src="screenshots/kde-tray.png" width="80" alt="KDE light tray icon"> | <img src="screenshots/kde-dark-tray.png" width="80" alt="KDE dark tray icon"> | <img src="screenshots/tauri-tray.png" width="80" alt="Tauri tray icon"> |

</details>
