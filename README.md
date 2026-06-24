# Flipper Zero Hacking Toolkit

Welcome to the Flipper Zero Hacking Toolkit repository! This collection of files and tools is designed to help you explore and experiment with various hardware hacking techniques using the Flipper Zero device. Before diving into the world of hardware hacking, please take a moment to read this README carefully.

## Table of Contents

1. [Introduction](#introduction)
2. [Included Tools and Definitions](#included-tools-and-definitions)
   - NFID
   - NFC
   - Sub-GHz
   - IR/IR Fuzzer
   - Brute Force Attack
   - iButton/iButton Fuzzer
   - Bad USB
3. [Tool Repositories](#tool-repositories)
4. [Disclaimer](#disclaimer)
5. [Getting Started](#getting-started)
6. [System Requirements](#system-requirements)
7. [Usage and Caution](#usage-and-caution)
8. [Contributing](#contributing)
9. [Credits](#credits)
10. [Security Best Practices](#security-best-practices)
11. [Updates and Maintenance](#updates-and-maintenance)
12. [License](#license)

## Introduction

The Flipper Zero is a versatile hacking and security tool designed for exploring and interacting with various electronic devices. This repository contains a collection of files and tools that can be used in conjunction with the Flipper Zero device to perform various hardware hacking tasks. It's important to use these tools responsibly and legally.

## Included Tools and Definitions

### NFID (Near-Field Identification)

NFID refers to the process of identifying and interacting with nearby electronic devices using radio frequency communication. This can include devices like RFID cards, access control systems, and more.

### NFC (Near-Field Communication)

NFC is a subset of NFID that allows for two-way communication between devices over short distances. It is commonly used for contactless payments, access control, and data transfer between smartphones and other devices.

### Sub-GHz

Sub-GHz frequencies refer to radio frequencies that are below 1 GHz. These frequencies are commonly used for wireless communication in devices like remote controls, IoT devices, and industrial applications.

### IR/IR Fuzzer (Infrared/Infrared Fuzzer)

Infrared (IR) communication involves the use of infrared light to transmit data between devices. An IR fuzzer can be used to test and interact with IR-based systems such as remote controls and IR receivers.

### Brute Force Attack

A brute force attack is a method of trying all possible combinations or passwords systematically in order to gain unauthorized access to a system or device.

### iButton/iButton Fuzzer

iButton is a brand of electronic tokens that can be used for various applications, including access control. An iButton fuzzer is a tool for testing and interacting with iButton-based systems.

### Bad USB

Bad USB refers to a type of attack where a compromised USB device, such as a USB keyboard or flash drive, is used to exploit vulnerabilities in a target system.

## Tool Repositories

The `apps/` folder bundles 256 `.fap` applications (built for Momentum firmware). The
tables below map every app to its upstream source repository, grouped by the on-device
category.

**Notes:**
- Links are **best-effort**. Where an app's catalog manifest points to an aggregator
  mono-repo, that repo is listed (e.g. many apps live in
  [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins)).
- Apps marked *Bundled with firmware* ship inside the firmware itself and have no
  separate standalone repo — see [Next-Flip/Momentum-Firmware](https://github.com/Next-Flip/Momentum-Firmware)
  and [flipperdevices/flipperzero-good-faps](https://github.com/flipperdevices/flipperzero-good-faps).
- A handful are marked *Unknown* where no source repo could be confidently identified.

**Primary upstream sources:**
- [Next-Flip/Momentum-Firmware](https://github.com/Next-Flip/Momentum-Firmware) — the firmware these apps target
- [flipperdevices/flipperzero-firmware](https://github.com/flipperdevices/flipperzero-firmware) — official firmware
- [flipperdevices/flipper-application-catalog](https://github.com/flipperdevices/flipper-application-catalog) — official app catalog (manifests + source URLs)
- [flipperdevices/flipperzero-good-faps](https://github.com/flipperdevices/flipperzero-good-faps) — official bundled apps
- [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) — community aggregator mono-repo
- [djsime1/awesome-flipperzero](https://github.com/djsime1/awesome-flipperzero) — curated index of everything Flipper Zero

### Bluetooth

| App | Repository |
| --- | --- |
| ble_spam.fap | Bundled with firmware (official good-faps / Momentum) |
| bt_trigger.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| findmy.fap | [MatthewKuKanich/FindMyFlipper](https://github.com/MatthewKuKanich/FindMyFlipper) |
| hid_ble.fap | [fidian/flipper-hid-app](https://github.com/fidian/flipper-hid-app) |
| pc_monitor.fap | [TheSainEyereg/flipper-pc-monitor](https://github.com/TheSainEyereg/flipper-pc-monitor) |

### Games

| App | Repository |
| --- | --- |
| 4inrow.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| air_arkanoid.fap | [flipperdevices/flipperzero-good-faps](https://github.com/flipperdevices/flipperzero-good-faps) |
| air_labyrinth.fap | [jamisonderek/flipper-zero-tutorials](https://github.com/jamisonderek/flipper-zero-tutorials) |
| arkanoid.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| asteroids.fap | [SimplyMinimal/FlipperZero-Asteroids](https://github.com/SimplyMinimal/FlipperZero-Asteroids) |
| blackjack.fap | [doofy-dev/flipper_blackjack](https://github.com/doofy-dev/flipper_blackjack) |
| bomberduck.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| chess.fap | [xtruan/flipper-chess](https://github.com/xtruan/flipper-chess) |
| color_guess.fap | [leedave/flipper-zero-color-guess](https://github.com/leedave/flipper-zero-color-guess) |
| doom.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| flappy_bird.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| flipper_pong.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| game_2048.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| game15.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| gameoflife.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| geometry_flip.fap | [gooseprjkt/flipperzero-geometryflip](https://github.com/gooseprjkt/flipperzero-geometryflip) |
| heap_defence.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| jetpack_joyride.fap | [timstrasser/flipper-jetpack-game](https://github.com/timstrasser/flipper-jetpack-game) |
| laser_tag.fap | [RocketGod-git/Flipper-Zero-Laser-Tag](https://github.com/RocketGod-git/Flipper-Zero-Laser-Tag) |
| minesweeper_redux.fap | [squee72564/F0_Minesweeper_Fap](https://github.com/squee72564/F0_Minesweeper_Fap) |
| multi_dice.fap | Unknown |
| pinball0.fap | [rdefeo/pinball0](https://github.com/rdefeo/pinball0) |
| quadrastic.fap | [ivanbarsukov/flipperzero-quadrastic](https://github.com/ivanbarsukov/flipperzero-quadrastic) |
| reversi.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| roots_of_life.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| rubiks_cube_scrambler.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| scorched_tanks.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| simon_says.fap | [SimplyMinimal/FlipperZero-SimonSays](https://github.com/SimplyMinimal/FlipperZero-SimonSays) |
| slotmachine.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| snake20.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| solitaire.fap | [doofy-dev/flipper_solitaire](https://github.com/doofy-dev/flipper_solitaire) |
| t_rex_runner.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| tama_p1.fap | [GMMan/flipperzero-tamagotch-p1](https://github.com/GMMan/flipperzero-tamagotch-p1) |
| tanks.fap | Bundled with firmware (official good-faps / Momentum) |
| tetris.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| tictactoe.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| umpire_indicator.fap | [RocketGod-git/Flipper-Zero-Umpire-Indicator](https://github.com/RocketGod-git/Flipper-Zero-Umpire-Indicator) |
| videopoker.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| yapinvaders.fap | [dagnazty/Yappy_Invaders](https://github.com/dagnazty/Yappy_Invaders) |
| yatzee.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| zombiez.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |

### GPIO

| App | Repository |
| --- | --- |
| air_mouse.fap | [ginkage/FlippAirMouse](https://github.com/ginkage/FlippAirMouse) |
| avr_isp.fap | [flipperdevices/flipperzero-good-faps](https://github.com/flipperdevices/flipperzero-good-faps) |
| blackhat.fap | [o7-machinehum/flipper-blackhat-app](https://github.com/o7-machinehum/flipper-blackhat-app) |
| camera_suite.fap | [CodyTolene/Flipper-Zero-Camera-Suite](https://github.com/CodyTolene/Flipper-Zero-Camera-Suite) |
| co2_logger.fap | [harryob2/co2_logger](https://github.com/harryob2/co2_logger) |
| coleco.fap | [ezod/flipperzero-rc2014-coleco](https://github.com/ezod/flipperzero-rc2014-coleco) |
| dap_link.fap | [flipperdevices/flipperzero-good-faps](https://github.com/flipperdevices/flipperzero-good-faps) |
| esp_flasher.fap | [0xchocolate/flipperzero-esp-flasher](https://github.com/0xchocolate/flipperzero-esp-flasher) |
| esp32_wifi_marauder.fap | [0xchocolate/flipperzero-wifi-marauder](https://github.com/0xchocolate/flipperzero-wifi-marauder) |
| esp8266_deauther.fap | [SequoiaSan/FlipperZero-Wifi-ESP8266-Deauther-Module](https://github.com/SequoiaSan/FlipperZero-Wifi-ESP8266-Deauther-Module) |
| esp8266_ifttt_virtual_button.fap | [Ferrazzi/FlipperZero_IFTTT_Virtual_Button](https://github.com/Ferrazzi/FlipperZero_IFTTT_Virtual_Button) |
| esp8266_wifi_deauther_v2.fap | [Timmotools/flipperzero_esp8266_deautherv2](https://github.com/Timmotools/flipperzero_esp8266_deautherv2) |
| eth_troubleshooter.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| evil_portal.fap | [bigbrodude6119/flipper-zero-evil-portal](https://github.com/bigbrodude6119/flipper-zero-evil-portal) |
| flashlight.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| flip_downloader.fap | [jblanked/FlipDownloader](https://github.com/jblanked/FlipDownloader) |
| flip_library.fap | [jblanked/FlipLibrary](https://github.com/jblanked/FlipLibrary) |
| flip_social.fap | [jblanked/FlipSocial](https://github.com/jblanked/FlipSocial) |
| flip_tdi.fap | [flipperdevices/flipperzero-good-faps](https://github.com/flipperdevices/flipperzero-good-faps) |
| flip_trader.fap | [jblanked/FlipTrader](https://github.com/jblanked/FlipTrader) |
| flip_weather.fap | [jblanked/FlipWeather](https://github.com/jblanked/FlipWeather) |
| flip_wifi.fap | [jblanked/FlipWiFi](https://github.com/jblanked/FlipWiFi) |
| flip_world.fap | [jblanked/FlipWorld](https://github.com/jblanked/FlipWorld) |
| flipboard_blinky.fap | [jamisonderek/flipboard](https://github.com/jamisonderek/flipboard) |
| flipboard_keyboard.fap | [jamisonderek/flipboard](https://github.com/jamisonderek/flipboard) |
| flipboard_signal.fap | [jamisonderek/flipboard](https://github.com/jamisonderek/flipboard) |
| flipboard_simon.fap | [jamisonderek/flipboard](https://github.com/jamisonderek/flipboard) |
| flipper_atomicdiceroller.fap | [nmrr/flipperzero-atomicdiceroller](https://github.com/nmrr/flipperzero-atomicdiceroller) |
| flipper_geiger.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| flipper_spi_terminal.fap | [janwiesemann/flipper-spi-terminal](https://github.com/janwiesemann/flipper-spi-terminal) |
| flipperscope.fap | [anfractuosity/flipperscope](https://github.com/anfractuosity/flipperscope) |
| fm_radio.fap | [victormico/flipperzero-radio](https://github.com/victormico/flipperzero-radio) |
| fmtx_app.fap | [GooseDev72/flipperzero-kt0803-transmitter](https://github.com/GooseDev72/flipperzero-kt0803-transmitter) |
| free_roam.fap | [jblanked/Free-Roam](https://github.com/jblanked/Free-Roam) |
| ghost_esp.fap | [Spooks4576/ghost_esp_app](https://github.com/Spooks4576/ghost_esp_app) |
| gpio_badge.fap | [jamisonderek/flipper-zero-tutorials](https://github.com/jamisonderek/flipper-zero-tutorials) |
| gpio_controller.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| gpio_explorer_app.fap | [EvgeniGenchev07/gpio_explorer](https://github.com/EvgeniGenchev07/gpio_explorer) |
| gpio_reader_a.fap | [aureli1c/flipperzero_GPIO_read](https://github.com/aureli1c/flipperzero_GPIO_read) |
| gpio_reader_b.fap | [biotinker/flipperzero-gpioreader](https://github.com/biotinker/flipperzero-gpioreader) |
| gpio_sentry_safe.fap | [H4ckd4ddy/flipperzero-sentry-safe-plugin](https://github.com/H4ckd4ddy/flipperzero-sentry-safe-plugin) |
| gpio.fap | Bundled with firmware (official good-faps / Momentum) |
| gps_nmea.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| hc_sr04.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| i2ctools.fap | [NaejEL/flipperzero-i2ctools](https://github.com/NaejEL/flipperzero-i2ctools) |
| ina_meter.fap | [cepetr/flipper-tina](https://github.com/cepetr/flipper-tina) |
| lightmeter.fap | [oleksiikutuzov/flipperzero-lightmeter](https://github.com/oleksiikutuzov/flipperzero-lightmeter) |
| longwave_clock.fap | [m7i-org/flipper_longwave_clock](https://github.com/m7i-org/flipper_longwave_clock) |
| magspoof.fap | [zacharyweiss/magspoof_flipper](https://github.com/zacharyweiss/magspoof_flipper) |
| malveke_gb_cartridge.fap | [EstebanFuentealba/MALVEKE-Flipper-Zero](https://github.com/EstebanFuentealba/MALVEKE-Flipper-Zero) |
| malveke_gb_emulator.fap | [EstebanFuentealba/MALVEKE-Flipper-Zero](https://github.com/EstebanFuentealba/MALVEKE-Flipper-Zero) |
| malveke_gb_link_camera.fap | [EstebanFuentealba/MALVEKE-Flipper-Zero](https://github.com/EstebanFuentealba/MALVEKE-Flipper-Zero) |
| malveke_gb_live_camera.fap | [EstebanFuentealba/MALVEKE-Flipper-Zero](https://github.com/EstebanFuentealba/MALVEKE-Flipper-Zero) |
| malveke_gb_photo.fap | [EstebanFuentealba/MALVEKE-Flipper-Zero](https://github.com/EstebanFuentealba/MALVEKE-Flipper-Zero) |
| malveke_gba_cartridge.fap | [EstebanFuentealba/MALVEKE-Flipper-Zero](https://github.com/EstebanFuentealba/MALVEKE-Flipper-Zero) |
| malveke_pin_test.fap | [EstebanFuentealba/MALVEKE-Flipper-Zero](https://github.com/EstebanFuentealba/MALVEKE-Flipper-Zero) |
| mayhem_camera.fap | [eried/flipperzero-mayhem](https://github.com/eried/flipperzero-mayhem) |
| mayhem_marauder.fap | [eried/flipperzero-mayhem](https://github.com/eried/flipperzero-mayhem) |
| mayhem_morseflash.fap | [eried/flipperzero-mayhem](https://github.com/eried/flipperzero-mayhem) |
| mayhem_motion.fap | [eried/flipperzero-mayhem](https://github.com/eried/flipperzero-mayhem) |
| mayhem_nannycam.fap | [eried/flipperzero-mayhem](https://github.com/eried/flipperzero-mayhem) |
| mayhem_qrcode.fap | [eried/flipperzero-mayhem](https://github.com/eried/flipperzero-mayhem) |
| nearby_files.fap | [Stichoza/flipper-nearby-files](https://github.com/Stichoza/flipper-nearby-files) |
| nrf24batch.fap | [vad7/nRF24-Batch](https://github.com/vad7/nRF24-Batch) |
| nrf24channelscanner.fap | [htotoo/NRF24ChannelScanner](https://github.com/htotoo/NRF24ChannelScanner) |
| nrf24mousejacker.fap | [mothball187/flipperzero-nrf24](https://github.com/mothball187/flipperzero-nrf24) |
| nrf24scan.fap | [vad7/nrf24scan](https://github.com/vad7/nrf24scan) |
| nrf24sniff.fap | [mothball187/flipperzero-nrf24](https://github.com/mothball187/flipperzero-nrf24) |
| pokemon.fap | [kbembedded/Flipper-Zero-Game-Boy-Pokemon-Trading](https://github.com/kbembedded/Flipper-Zero-Game-Boy-Pokemon-Trading) |
| r4tkn.fap | [rusyln/flipper-zero-bw16-r4tkn](https://github.com/rusyln/flipper-zero-bw16-r4tkn) |
| radar_scanner.fap | [MatthewKuKanich/flipper-radar](https://github.com/MatthewKuKanich/flipper-radar) |
| signal_generator.fap | Bundled with firmware (official good-faps / Momentum) |
| spi_mem_manager.fap | Bundled with firmware (official good-faps / Momentum) |
| swd_probe.fap | [g3gg0/flipper-swd_probe](https://github.com/g3gg0/flipper-swd_probe) |
| timelapse.fap | [theageoflove/flipperzero-zeitraffer](https://github.com/theageoflove/flipperzero-zeitraffer) |
| uart_terminal.fap | [cool4uma/UART_Terminal](https://github.com/cool4uma/UART_Terminal) |
| unitemp.fap | [quen0n/unitemp-flipperzero](https://github.com/quen0n/unitemp-flipperzero) |
| uv_meter_as7331.fap | [michaelbaisch/uv_meter](https://github.com/michaelbaisch/uv_meter) |
| vgm_air_mouse.fap | Bundled with firmware (official good-faps / Momentum) |
| video_game_module_tool.fap | Bundled with firmware (official good-faps / Momentum) |
| wardriver.fap | [Sil333033/flipperzero-wardriver](https://github.com/Sil333033/flipperzero-wardriver) |
| web_crawler.fap | [jblanked/WebCrawler-FlipperZero](https://github.com/jblanked/WebCrawler-FlipperZero) |
| wifi_scanner.fap | [SequoiaSan/FlipperZero-WiFi-Scanner_Module](https://github.com/SequoiaSan/FlipperZero-WiFi-Scanner_Module) |
| wii_ec_anal.fap | [csBlueChip/FlipperZero_WiiEC](https://github.com/csBlueChip/FlipperZero_WiiEC) |
| wire_tester.fap | Unknown |

### iButton

| App | Repository |
| --- | --- |
| fuzzer_ibtn.fap | [DarkFlippers/Multi_Fuzzer](https://github.com/DarkFlippers/Multi_Fuzzer) |
| ibutton_converter.fap | [Leptopt1los/ibutton_converter](https://github.com/Leptopt1los/ibutton_converter) |
| ibutton.fap | Bundled with firmware (official good-faps / Momentum) |

### Infrared

| App | Repository |
| --- | --- |
| flame_rng.fap | [OrionW06/Flame-RNG](https://github.com/OrionW06/Flame-RNG) |
| flipper_xremote.fap | [kala13x/flipper-xremote](https://github.com/kala13x/flipper-xremote) |
| hitachi_ac_remote.fap | [dogtopus/flipperzero-hitachi-ac-remote](https://github.com/dogtopus/flipperzero-hitachi-ac-remote) |
| infrared.fap | Bundled with firmware (official good-faps / Momentum) |
| ir_intervalometer.fap | [Nitepone/flipper-intervalometer](https://github.com/Nitepone/flipper-intervalometer) |
| ir_remote.fap | [Hong5489/ir_remote](https://github.com/Hong5489/ir_remote) |
| ir_scope.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| lidar_emulator.fap | [regaly/flipperzero-lidar_emulator](https://github.com/regaly/flipperzero-lidar_emulator) |
| midea_ac_remote.fap | [xakep666/flipperzero-midea-ac-remote](https://github.com/xakep666/flipperzero-midea-ac-remote) |
| mitsubishi_ac_remote.fap | [achistyakov/flipperzero-mitsubishi-ac-remote](https://github.com/achistyakov/flipperzero-mitsubishi-ac-remote) |
| xbox_controller.fap | [gebeto/flipper-xbox-controller](https://github.com/gebeto/flipper-xbox-controller) |
| xremote.fap | [leedave/flipper-zero-cross-remote](https://github.com/leedave/flipper-zero-cross-remote) |

### Media

| App | Repository |
| --- | --- |
| bpm_tapper.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| etch.fap | Unknown |
| flizzer_tracker.fap | [LTVA1/flizzer_tracker](https://github.com/LTVA1/flizzer_tracker) |
| fmatrix.fap | [misterwaztaken/fmatrix](https://github.com/misterwaztaken/fmatrix) |
| fzspground.fap | [alanfortlink/fzspground](https://github.com/alanfortlink/fzspground) |
| image_viewer.fap | [polioan/flipper-zero-image-viewer](https://github.com/polioan/flipper-zero-image-viewer) |
| metronome.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| morse_code.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| music_player.fap | [flipperdevices/flipperzero-good-faps](https://github.com/flipperdevices/flipperzero-good-faps) |
| paint.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| text2sam.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| tuning_fork.fap | [besya/flipperzero-tuning-fork](https://github.com/besya/flipperzero-tuning-fork) |
| usb_midi.fap | [kribesk/flipper-zero-usb-midi](https://github.com/kribesk/flipper-zero-usb-midi) |
| video_player.fap | [LTVA1/flipper-zero-video-player](https://github.com/LTVA1/flipper-zero-video-player) |
| wav_player.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |

### NFC

| App | Repository |
| --- | --- |
| cyborg_detector.fap | [RocketGod-git/Flipper-Zero-Cyborg-Detector](https://github.com/RocketGod-git/Flipper-Zero-Cyborg-Detector) |
| metroflip.fap | [luu176/Metroflip](https://github.com/luu176/Metroflip) |
| mfc_editor.fap | [TollyH/flipper-apps](https://github.com/TollyH/flipper-apps) |
| mfkey.fap | Bundled with firmware (official good-faps / Momentum) |
| mifare_fuzzer.fap | [spheeere98/mifare_fuzzer](https://github.com/spheeere98/mifare_fuzzer) |
| nfc_apdu_runner.fap | [SpenserCai/nfc_apdu_runner](https://github.com/SpenserCai/nfc_apdu_runner) |
| nfc_eink.fap | [RebornedBrain/nfc_eink](https://github.com/RebornedBrain/nfc_eink) |
| nfc_magic.fap | Bundled with firmware (official good-faps / Momentum) |
| nfc_maker.fap | [Next-Flip/Momentum-Apps](https://github.com/Next-Flip/Momentum-Apps) |
| nfc_playlist.fap | [acegoal07/FlipperZero_NFC_Playlist](https://github.com/acegoal07/FlipperZero_NFC_Playlist) |
| nfc.fap | Bundled with firmware (official good-faps / Momentum) |
| passy.fap | [bettse/passy](https://github.com/bettse/passy) |
| picopass.fap | [bettse/picopass](https://github.com/bettse/picopass) |
| seader.fap | [bettse/seader](https://github.com/bettse/seader) |
| seos.fap | [bettse/seos_compatible](https://github.com/bettse/seos_compatible) |
| weebo.fap | [bettse/weebo](https://github.com/bettse/weebo) |

### RFID

| App | Repository |
| --- | --- |
| em4100_generator.fap | [Milk-Cool/fz-em4100-generator](https://github.com/Milk-Cool/fz-em4100-generator) |
| fuzzer_rfid.fap | [DarkFlippers/Multi_Fuzzer](https://github.com/DarkFlippers/Multi_Fuzzer) |
| lfrfid.fap | Bundled with firmware (official good-faps / Momentum) |
| simultaneous_rfid_reader.fap | [haffnerriley/Simultaneous-UHF-RFID-FlipperZero](https://github.com/haffnerriley/Simultaneous-UHF-RFID-FlipperZero) |
| t5577_multiwriter.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| t5577_writer.fap | [zinongli/T5577_Raw_Writer](https://github.com/zinongli/T5577_Raw_Writer) |
| uhf_rfid.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |

### Sub-GHz

| App | Repository |
| --- | --- |
| chief_cooker.fap | [denr01/FZ-ChiefCooker](https://github.com/denr01/FZ-ChiefCooker) |
| esubghz_chat.fap | [twisted-pear/esubghz_chat](https://github.com/twisted-pear/esubghz_chat) |
| flipper_share.fap | [lomalkin/flipper-zero-apps](https://github.com/lomalkin/flipper-zero-apps) |
| fmf_to_sub.fap | [jamisonderek/flipper-zero-tutorials](https://github.com/jamisonderek/flipper-zero-tutorials) |
| hc11_modem.fap | [Giraut/flipper_zero_hc11_wireless_modem](https://github.com/Giraut/flipper_zero_hc11_wireless_modem) |
| meal_pager.fap | [leedave/flipper-zero-meal-pager](https://github.com/leedave/flipper-zero-meal-pager) |
| pocsag_pager.fap | [xMasterX/flipper-pager](https://github.com/xMasterX/flipper-pager) |
| protoview.fap | [antirez/protoview](https://github.com/antirez/protoview) |
| radio_scanner.fap | [RocketGod-git/Flipper-Zero-Radio-Scanner](https://github.com/RocketGod-git/Flipper-Zero-Radio-Scanner) |
| rolling_flaws.fap | [jamisonderek/flipper-zero-tutorials](https://github.com/jamisonderek/flipper-zero-tutorials) |
| spectrum_analyzer.fap | [jolcese/flipperzero-firmware](https://github.com/jolcese/flipperzero-firmware/tree/spectrum/applications/spectrum_analyzer) |
| sub_analyzer.fap | Bundled with firmware (official good-faps / Momentum) |
| subghz_bruteforcer.fap | [DarkFlippers/flipperzero-subbrute](https://github.com/DarkFlippers/flipperzero-subbrute) |
| subghz_fap.fap | Bundled with firmware (official good-faps / Momentum) |
| subghz_playlist_creator.fap | Bundled with firmware (official good-faps / Momentum) |
| subghz_playlist.fap | [darmiel/flipper-playlist](https://github.com/darmiel/flipper-playlist) |
| subghz_remote.fap | [DarkFlippers/SubGHz_Remote](https://github.com/DarkFlippers/SubGHz_Remote) |
| subghz_scheduler.fap | [shalebridge/flipper-subghz-scheduler](https://github.com/shalebridge/flipper-subghz-scheduler) |
| tpms.fap | Bundled with firmware (official good-faps / Momentum) |
| weather_station.fap | [flipperdevices/flipperzero-good-faps](https://github.com/flipperdevices/flipperzero-good-faps) |

### Tools

| App | Repository |
| --- | --- |
| bad_kb.fap | Bundled with firmware (official good-faps / Momentum) |
| barcode_app.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| caesar_cipher.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| calculator.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| cntdown_tim.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| combo_cracker.fap | [CharlesTheGreat77/ComboCracker-FZ](https://github.com/CharlesTheGreat77/ComboCracker-FZ) |
| counter.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| dtmf_dolphin.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| flip_crypt.fap | [Tyl3rA/FlipCrypt](https://github.com/Tyl3rA/FlipCrypt) |
| flipbip.fap | [xtruan/FlipBIP](https://github.com/xtruan/FlipBIP) |
| flipp_pomodoro.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| hex_editor.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| hex_viewer.fap | [QtRoS/flipper-zero-hex-viewer](https://github.com/QtRoS/flipper-zero-hex-viewer) |
| key_copier.fap | [zinongli/KeyCopier](https://github.com/zinongli/KeyCopier) |
| multi_converter.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| nfc_rfid_detector.fap | [flipperdevices/flipperzero-good-faps](https://github.com/flipperdevices/flipperzero-good-faps) |
| nightstand.fap | Unknown |
| passgen.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| programmercalc.fap | [armixz/Flipper-Zero-Programmer-Calculator](https://github.com/armixz/Flipper-Zero-Programmer-Calculator) |
| qrcode.fap | [bmatcuk/flipperzero-qrcode](https://github.com/bmatcuk/flipperzero-qrcode) |
| quac.fap | [rdefeo/quac](https://github.com/rdefeo/quac) |
| resistors.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| tasks.fap | [MadLadSquad/FlipperTasks](https://github.com/MadLadSquad/FlipperTasks) |
| text_viewer.fap | [xMasterX/all-the-plugins](https://github.com/xMasterX/all-the-plugins) |
| tone_gen.fap | [GEMISIS/tone_gen](https://github.com/GEMISIS/tone_gen) |
| totp.fap | [akopachov/flipper-zero_authenticator](https://github.com/akopachov/flipper-zero_authenticator) |
| upython.fap | [ofabel/mp-flipper](https://github.com/ofabel/mp-flipper) |
| voltcalc_app.fap | [HappyAmos/Flipper_FAPS](https://github.com/HappyAmos/Flipper_FAPS) |

### USB

| App | Repository |
| --- | --- |
| hid_usb.fap | [fidian/flipper-hid-app](https://github.com/fidian/flipper-hid-app) |
| ldtoypad.fap | [SegerEnd/Flipper-Zero-LD-Toypad-Emulator](https://github.com/SegerEnd/Flipper-Zero-LD-Toypad-Emulator) |
| mass_storage.fap | [flipperdevices/flipperzero-good-faps](https://github.com/flipperdevices/flipperzero-good-faps) |
| portal_of_flipper.fap | [sanjay900/portal_of_flipper](https://github.com/sanjay900/portal_of_flipper) |
| u2f.fap | Bundled with firmware (official good-faps / Momentum) |
| usb_ccb.fap | [WithSecureLabs/usb-consumer-control](https://github.com/WithSecureLabs/usb-consumer-control) |
| xinput_controller.fap | [expected-ingot/flipper-xinput](https://github.com/expected-ingot/flipper-xinput) |

### System &amp; Settings

| App | Repository |
| --- | --- |
| about.fap | Bundled with firmware (official good-faps / Momentum) |
| bt_settings.fap | Bundled with firmware (official good-faps / Momentum) |
| clock_settings.fap | Bundled with firmware (official good-faps / Momentum) |
| desktop_settings.fap | Bundled with firmware (official good-faps / Momentum) |
| expansion_settings.fap | Bundled with firmware (official good-faps / Momentum) |
| input_settings.fap | Bundled with firmware (official good-faps / Momentum) |
| js_app.fap | Bundled with firmware (official good-faps / Momentum) |
| momentum_app.fap | [Next-Flip/Momentum-Firmware](https://github.com/Next-Flip/Momentum-Firmware) |
| notification_settings.fap | Bundled with firmware (official good-faps / Momentum) |
| passport.fap | Bundled with firmware (official good-faps / Momentum) |
| power_settings.fap | Bundled with firmware (official good-faps / Momentum) |
| storage_settings.fap | Bundled with firmware (official good-faps / Momentum) |
| system_settings.fap | Bundled with firmware (official good-faps / Momentum) |

## Disclaimer

**WARNING:** The tools and techniques provided in this repository are intended for educational and research purposes only. Unauthorized or illegal use of these tools to hack into devices or systems without proper authorization is strictly prohibited and may have legal consequences. Always ensure that you have proper authorization before attempting any hardware hacking activities.

## Getting Started

To get started with the Flipper Zero Hacking Toolkit, follow these steps:

1. Clone or download this repository to your local machine.
2. Ensure you have a Flipper Zero device.

## System Requirements

The only system requirement for this toolkit is a Flipper Zero device.

## Usage and Caution

While this toolkit provides a wide range of tools and resources, always exercise caution and follow ethical guidelines when using them. Only hack devices and systems for which you have explicit authorization. Unauthorized hacking activities can lead to legal consequences.

## Contributing

If you have additional tools, resources, or improvements to contribute to this toolkit, feel free to submit pull requests or open issues. We welcome contributions from the community to make this toolkit even more useful and safe.

## Credits

We would like to give credit to the following individuals for their contributions to this toolkit:

- [UberGuidoZ](https://github.com/UberGuidoZ)
- [Talking-Sasquach](https://github.com/Talking-Sasquach)
- [UNC0V3R3D](https://github.com/UNC0V3R3D)
- [I-Am-Jakoby](https://github.com/I-Am-Jakoby)

## Security Best Practices

When using the Flipper Zero Hacking Toolkit, always adhere to the following security best practices:

- Obtain proper authorization before attempting any hardware hacking activities.
- Respect the privacy and security of individuals and organizations.
- Report any security vulnerabilities you discover through responsible disclosure channels.

## Updates and Maintenance

This repository will be regularly updated and maintained to improve its functionality and security. Check back for updates and improvements to the toolkit.

## License

This repository is provided under the [LICENSE](LICENSE) file included with the toolkit. Make sure to review and adhere to the terms of the license when using these tools.

Remember to always act responsibly, ethically, and within the boundaries of the law when using the Flipper Zero Hacking Toolkit. Happy hacking, and stay safe!
