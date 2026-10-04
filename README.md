# Awesome Nintendo Switch Homebrew

Подборка homebrew для Nintendo Switch: прошивки, sys-модули, эмуляторы, нативные порты и утилиты.

> Требуется консоль с кастомной прошивкой (Atmosphère) и homebrew-доступом.
> Проекты помечены как `со своим копиями игры` там, где нужны собственные файлы игры.

## Содержание

- [Прошивка и загрузка](#прошивка-и-загрузка)
- [Меню, пакетники, файлы](#меню-пакетники-файлы)
- [Сохранения, читы, amiibo](#сохранения-читы-amiibo)
- [Sys-модули и оверлеи](#sys-модули-и-оверлеи)
- [Кастомизация](#кастомизация)
- [Медиа и стриминг](#медиа-и-стриминг)
- [Сетевая игра и онлайн](#сетевая-игра-и-онлайн)
- [Эмуляторы](#эмуляторы)
- [Нативные порты и рекомпиляции](#нативные-порты-и-рекомпиляции)
- [Linux / Android](#linux--android)
- [Для разработки](#для-разработки)
- [Серая зона](#серая-зона)
- [Legacy](#legacy)

## Прошивка и загрузка

- [Atmosphère](https://github.com/Atmosphere-NX/Atmosphere) — основная кастомная прошивка.
- [hekate](https://github.com/CTCaer/hekate) — кастомный бутлоадер: запуск payload'ов, emuMMC, бэкапы.
- [TegraRcmGUI](https://github.com/eliboa/TegraRcmGUI) — инжектор payload под Windows.
- [Rekado](https://github.com/MenosGrante/Rekado) — то же самое под Android.
- [nx-hbmenu](https://github.com/switchbrew/nx-hbmenu) — Homebrew Menu.
- [hb-appstore](https://github.com/fortheusers/hb-appstore) — App Store для homebrew.
- [sphaira](https://github.com/NaGaa95/sphaira) — современная альтернатива hbmenu, совместима с App Store.

### Сборки (AIO)

Готовые наборы «прошивка + программы + конфиги», распаковываются в корень SD-карты.

- [DeepSea](https://github.com/Team-Neptune/DeepSea) — CFW + homebrew, международная сборка.
- [PYXIS](https://github.com/mentalblank/PYXIS) — автоматическая AIO-сборка (скриптовая).
- [Kefir](https://github.com/rashevskyv/kefir) — сборка от xHR на базе модифицированной Atmosphère, с редиректом сейвов и своим апдейтером ([kefir-updater](https://github.com/rashevskyv/kefir-updater)).
- [UltraNX](https://github.com/Ultra-NX/UltraNX) — сборка от redraz: пред настроенный Horizon OC, андервольт, оверлей [Ultra-Tuner](https://github.com/Ultra-NX/Ultra/wiki).
- [NX Venom](https://github.com/CatcherITGF/NX-Venom) — сборка с упором в разгон и тюнинг железа (зеркало: [gitverse.ru](https://gitverse.ru/CatcherITGF/NX-Venom)).

> Сборки с предустановленными DBI/шопами и sigpatches тащат за собой серую зону — см. раздел [Серая зона](#серая-зона).

## Меню, пакетники, файлы

- [Goldleaf](https://github.com/XorTroll/Goldleaf) — многоцелевой тул: установка, файлы, тикеты.
- [Awoo Installer](https://github.com/Huntereb/Awoo-Installer) — установщик NSP/XCI/NSPZ.
- [nxdumptool](https://github.com/DarkMatterCore/nxdumptool) — дамп картриджей и установленных тайтлов.
- [hacPack](https://github.com/D3fau4/hacPack) — сборка и перепаковка NCA/NSP.
- [NX-Shell](https://github.com/joel16/NX-Shell) — файловый менеджер.
- [N-Xplorer](https://github.com/CompSciOrBust/N-Xplorer) — многофункциональный файловый менеджер.
- [ftpsrv](https://github.com/ITotalJustice/ftpsrv) — маленький быстрый FTP-сервер.
- [sys-ftpd](https://github.com/cathery/sys-ftpd) — FTP как sys-модуль, работает фоном.

## Сохранения, читы, amiibo

- [Checkpoint](https://github.com/BernardoGiordano/Checkpoint) — быстрый менеджер сейвов.
- [JKSV](https://github.com/J-D-K/JKSV) — менеджер сейвов с поддержкой профилей.
- [emuiibo](https://github.com/XorTroll/emuiibo) — эмуляция amiibo.
- [botw-unexplored](https://github.com/lud99/botw-unexplored) — карта неисследованных мест по сейву Breath of the Wild.
- [totk-unexplored](https://github.com/lud99/totk-unexplored) — то же для Tears of the Kingdom.

## Sys-модули и оверлеи

- [Tesla / ovlloader](https://github.com/WerWolv/Tesla-Menu) — система оверлеев поверх игры.
- [Ultrahand-Overlay](https://github.com/ppkantorski/Ultrahand-Overlay) — графический оверлей-конструктор.
- [libultrahand](https://github.com/ppkantorski/libultrahand) — библиотека для разработки оверлеев.
- [ovl-sysmodules](https://github.com/ppkantorski/ovl-sysmodules) — включение/выключение sys-модулей из оверлея.
- [Status-Monitor-Overlay](https://github.com/ppkantorski/Status-Monitor-Overlay) — статистика железа (FPS, температуры, частоты).
- [fastCFWswitch](https://github.com/Hartie95/fastCFWswitch) — перезагрузка в другие payload'ы из оверлея.
- [sys-clk](https://github.com/retronx-team/sys-clk) — разгон и андервольт CPU/GPU/RAM.
- [Horizon-OC](https://github.com/Horizon-OC/Horizon-OC) — открытый инструмент разгона.
- [ReverseNX-RT](https://github.com/masagrator/ReverseNX-RT) — переключение dock/portable на лету.
- [sys-con](https://github.com/cathery/sys-con) — USB-геймпады на Switch.
- [MissionControl](https://github.com/ndeadly/MissionControl) — контроллеры других консолей по Bluetooth.
- [sys-tune](https://github.com/HookedBehemoth/sys-tune) — музыка фоном из homebrew-плеера.
- [TriPlayer](https://github.com/tallbl0nde/TriPlayer) — фоновый музыкальный плеер с sys-модулем.
- [MangoHud](https://github.com/NaGaa95/MangoHud) — оверлей мониторинга FPS и нагрузки.

## Кастомизация

- [SwitchThemeInjector / NXThemes](https://github.com/exelix11/SwitchThemeInjector) — создание и установка тем оформления.

## Медиа и стриминг

- [SysDVR](https://github.com/exelix11/SysDVR) — захват видео с консоли на ПК по USB или сети.
- [Moonlight-Switch](https://github.com/XITRIX/Moonlight-Switch) — геймстрим с ПК (NVIDIA GameStream/Sunshine).
- [Switchfin](https://github.com/dragonflylee/switchfin) — нативный клиент Jellyfin.
- [TsVitch](https://github.com/giovannimirulla/TsVitch) — IPTV-плеер.
- [wiliwili](https://github.com/xfangfang/wiliwili) — клиент bilibili.
- [SwitchWave](https://github.com/averne/SwitchWave) — медиаплеер с аппаратным декодированием.
- [eBookReaderSwitch](https://github.com/SeanOMik/eBookReaderSwitch) — читалка книг.

## Сетевая игра и онлайн

Три слоя: клиент на ПК/эмуляторе, модуль на консоли, серверная часть.

### Switch

- [switch-lan-play](https://github.com/spacemeowx2/switch-lan-play) — клиент, который запускается на ПК и превращает его в шлюз для Switch. Без него [ldn_mitm](https://github.com/spacemeowx2/ldn_mitm) бесполезен, поэтому лежат вместе. Играть нужно на одном сервере, ПК и консоль — в одной сети.
- [ldn_mitm](https://github.com/spacemeowx2/ldn_mitm) — sys-модуль, перехватывает локальную беспроводную связь и уводит её в Lan-Play; так работают онлайн игры с поддержкой local wireless.
- [Prelude-Nro](https://github.com/NextendoNetwork/Prelude-Nro) — homebrew для реальной консоли: подключает Atmosphère к сети Nextendo (аккаунт, друзья, присутствие).

### ПК и эмуляторы

- [Ryujinx-Nextendo](https://github.com/NextendoNetwork/Ryujinx-Nextendo) — сборка Ryujinx с аккаунтом Nextendo и онлайн-игрой.
- [citron-nextendo](https://github.com/NextendoNetwork/citron-nextendo) — то же на базе Citron.

### Серверная часть

- [slp-server-rust](https://github.com/spacemeowx2/slp-server-rust) — сервер Lan-Play на Rust, если хочется поднять свой вместо публичных.
- [nextendo-nex](https://github.com/NextendoNetwork/nextendo-nex) — реализация протокола NEX/PRUDP с нуля на Go, ядро серверов Nextendo.
- [NextendoNetwork](https://github.com/orgs/NextendoNetwork/repositories) — серверы под конкретные игры: Mario Kart 8 Deluxe, Splatoon 2/3, Smash Ultimate, Animal Crossing: New Horizons, Super Mario Maker 2 и другие. Плюс инфраструктура (`nextendo-account`, `nx-dauth`, `nx-scsi`, `nextendo-nncs`).

- [RetroArch](https://github.com/libretro/RetroArch) — оболочка с ядрами от NES до PS1 и аркад.
- [ppsspp-nx](https://github.com/NaGaa95/ppsspp-nx) — PSP.
- [DrasticDS_nx](https://github.com/NaGaa95/DrasticDS_nx) — Nintendo DS.
- [NetherSX2_nx](https://github.com/NaGaa95/NetherSX2_nx) — PlayStation 2.
- [dolphin-nx](https://github.com/NaGaa95/dolphin-nx) — GameCube / Wii.
- [Cemu-nx](https://github.com/NaGaa95/Cemu-nx) — Wii U.
- [rpcs3-nx](https://github.com/NaGaa95/rpcs3-nx) — PlayStation 3.
- [Vita3K-nx](https://github.com/NaGaa95/Vita3K-nx) — PlayStation Vita (экспериментально).
- [melonDS](https://github.com/melonDS-emu/melonDS) — Nintendo DS, есть Switch-сборки.
- [ScummVM](https://github.com/scummvm/scummvm) — квесты LucasArts и Sierra.
- [fake-08](https://github.com/jtothebell/fake-08) — эмулятор Pico-8.
- [EasyRPG Player](https://github.com/EasyRPG/Player) — интерпретатор игр RPG Maker 2000/2003.
- [Skyline](https://github.com/skyline-emu/skyline) — рантайм для запуска Android-игр.

## Нативные порты и рекомпиляции

Рекомпиляции Xbox 360 (движок [ReXGlue](https://github.com/rexglue/rexglue-sdk)):

- [nfsmw-nx](https://github.com/StevensND/nfsmw-nx) — Need for Speed: Most Wanted (2005), 30 FPS без разгона. `со своими копиями игры`
- [nfsu2-sw](https://github.com/antoxa2584x/nfsu2-sw) — Need for Speed: Underground 2 (Xbox), лифт в C через xboxrecomp; Linux и Switch NRO. `со своими копиями игры`
- [UnleashedRecomp-NX](https://github.com/NaGaa95/UnleashedRecomp-NX) — Sonic Unleashed.
- [MarathonRecomp-NX](https://github.com/NaGaa95/MarathonRecomp-NX) — Sonic the Hedgehog (2006).
- [skate3recomp-nx](https://github.com/NaGaa95/skate3recomp-nx) — Skate 3.

Порты на базе Android-сборок: игра запускается как есть под Horizon OS через слой-обёртку. Всем нужны свои файлы игры (`со своими копиями игры`).

- [infinityblade_nx](https://github.com/aks796/infinityblade_nx) — Infinity Blade (UE3).
- [abreloaded_nx](https://github.com/aks796/abreloaded_nx) — Angry Birds Reloaded.
- [bombsquad_nx](https://github.com/aks796/bombsquad_nx) — BombSquad.
- [bs_joyride_nx](https://github.com/aks796/bs_joyride_nx) — BombSquad: Joyride Modpack.
- [bse_rebombed_nx](https://github.com/aks796/bse_rebombed_nx) — BombSquad ReBombed.
- [sm63redux_nx](https://github.com/aks796/sm63redux_nx) — Super Mario 63 Redux.
- [sm127_nx](https://github.com/aks796/sm127_nx) — Super Mario 127.
- [lummm_nx](https://github.com/aks796/lummm_nx) — Level UP: Mario's Minigames Mayhem.
- [gta3-nx](https://github.com/mariob0y/gta3-nx) — GTA III.
- [gtasa_nx](https://github.com/NaGaa95/gtasa_nx) — GTA: San Andreas.
- [gtalcs_nx](https://github.com/NaGaa95/gtalcs_nx) — GTA: Liberty City Stories.
- [gtactw_nx](https://github.com/NaGaa95/gtactw_nx) — GTA: Chinatown Wars.
- [bully_nx](https://github.com/NaGaa95/bully_nx) — Bully.
- [max_nx_v2.1.131](https://github.com/NaGaa95/max_nx_v2.1.131) — Max Payne.
- [hl2_nx](https://github.com/NaGaa95/hl2_nx) — Half-Life 2.
- [css_nx](https://github.com/NaGaa95/css_nx) — Counter-Strike: Source.
- [tf2_nx](https://github.com/NaGaa95/tf2_nx) — Team Fortress 2 Classic.
- [openmohaa_nx](https://github.com/NaGaa95/openmohaa_nx) — Medal of Honor: Allied Assault.
- [ct_nx](https://github.com/NaGaa95/ct_nx) — Chrono Trigger.
- [sotn_nx](https://github.com/NaGaa95/sotn_nx) — Castlevania: Symphony of the Night.
- [silent-hill-decomp-nx](https://github.com/ChaykaDed/silent-hill-decomp-nx) — Silent Hill (PSX), порт PC-версии на базе PSX-декомпиляции. `со своими копиями игры`
- [fallout-ce-switch](https://github.com/ryandeering/fallout-ce-switch) — Fallout (Community Edition). `со своими копиями игры`
- [fallout2-ce-switch](https://github.com/ryandeering/fallout2-ce-switch) — Fallout 2 (Community Edition). `со своими копиями игры`
- [ff4_3d_nx](https://github.com/NaGaa95/ff4_3d_nx) — Final Fantasy IV 3D Remake.
- [vcmi_nx](https://github.com/NaGaa95/vcmi_nx) — Heroes of Might and Magic III (VCMI).

Прочие порты и обёртки:

- [mari0_ae_nx](https://github.com/aks796/mari0_ae_nx) — Mari0: Alesan99's Entities (движок [love-nx](https://github.com/retronx-team/love-nx)).
- [flappy_bird_nx](https://github.com/aks796/flappy_bird_nx) — Flappy Bird, нативный рерайт.
- [Helltaker-switch](https://github.com/D3fau4/Helltaker-switch) — Helltaker.
- [rayverse](https://github.com/D3fau4/rayverse) — Rayman 1.
- [autorun](https://github.com/autorunhq/autorun) — Wine + FEX/Box64 + DXVK/VKD3D: запуск Windows-игр (x86/x64) прямо на консоли.

### GTA V на Switch

Порт, которого официально не существует: **GTA V Switch Port** от **Paralympics Productions** — GTA V Legacy с ПК превращается в NSP через патчер и репак-тул.

- Распространяется через Discord (GitHub-репозитория нет).
- Нужна своя копия игры, патчер только редактирует её файлы. `со своими копиями игры`
- Пошаговая инструкция: [geekmaxxer.github.io/GTA5-NX-Tutorial](https://geekmaxxer.github.io/GTA5-NX-Tutorial/).
- Вокруг порта есть экосистема модов: [радио-редактор](https://github.com/Geekmaxxer/gta-radio-editor), [обновлятор gameconfig.xml](https://github.com/Geekmaxxer/GTA5SwitchGCUpdater), [SDK для меню](https://github.com/Geekmaxxer/GTA5NX-MG-Menu).
- Инструкция опирается на Tinfoil/sigpatches — это [серая зона](#серая-зона).

Декомпиляции и открытые движки:

- [Ship of Harkinian](https://github.com/HarbourMasters/Shipwright) — Ocarina of Time.
- [2Ship2Harkinian](https://github.com/HarbourMasters/2ship2harkinian) — Majora's Mask.
- [sm64ex](https://github.com/sm64pc/sm64ex) — Super Mario 64.
- [DevilutionX](https://github.com/diasurgical/devilutionX) — Diablo.
- [OpenTTD](https://github.com/OpenTTD/OpenTTD) — Transport Tycoon Deluxe.
- [OpenLara](https://github.com/XProger/OpenLara) — движок Tomb Raider.
- [SRB2](https://github.com/STJr/SRB2) — Sonic Robo Blast 2.
- [TheXTech](https://github.com/Wohlstand/TheXTech) — движок Super Mario Bros. X.
- [SuperTuxKart](https://github.com/supertuxkart/stk-code) — аркадные гонки.
- [Butterscotch](https://github.com/D3fau4/Butterscotch) — рантайм для игр GameMaker: Studio.
- [OpenMW (fgsfdsfgs)](https://github.com/fgsfdsfgs/openmw) — Morrowind на движке OpenMW, свежие сборки 0.46. `со своими копиями игры`

## Linux / Android

- [switchroot](https://github.com/switchroot) — L4T Ubuntu и LineageOS (Android) для Switch.
- [Lakka](https://github.com/libretro/Lakka-LibreELEC) — дистрибутив с RetroArch.
- [L4T-Megascript](https://github.com/NaGaa95/L4T-Megascript) — установщик популярных программ в L4T.
- [mesa-switch](https://github.com/NaGaa95/mesa-switch) — порт Mesa: NVK (Vulkan), OpenGL/GLES, EGL.
- [nxvk](https://github.com/D3fau4/nxvk) — порт Vulkan-драйвера NVK.
- [L4T-OC-Kernel](https://github.com/NaGaa95/L4T-OC-Kernel) — разгонное ядро для L4T.

## Для разработки

- [devkitPro](https://github.com/devkitPro) — devkitA64, libnx, порты библиотек.
- [switch-cmake](https://github.com/vbe0201/switch-cmake) — CMake-тулчейн.
- [borealis](https://github.com/natinusala/borealis) — UI-библиотека в стиле системного меню.
- [Homebrodot / Godot](https://github.com/Homebrodot/Godot) — Godot для homebrew-платформ, есть Switch-порт ([D3fau4/godot](https://github.com/D3fau4/godot)).
- [nx-dev](https://github.com/D3fau4/nx-dev) — Docker-образ для сборки под libnx.
- [switchbrew](https://switchbrew.org) — вики по железу и ОС Switch.

## Серая зона

Инструменты, связанные с обходом защиты и пиратством. Отдельный раздел, ссылки не привожу: используй на свой риск.

- **Lockpick_RCM** — дамп ключей консоли.
- **sys-patch** / sigpatches — патчи проверки подписи.
- **Tinfoil** и шопы — установка и загрузка из неофициальных источников.
- **NSZ-конвертеры** — сжатие образов игр.
- **DBI** — установщик/FTP/MTP-мультитул (распространяется через GBAtemp).

Отдельно: **re3 / reVC** — реверс-инжиниринг GTA III и Vice City. Проект удалён с GitHub по DMCA от Take-Two (2021) вместе с Switch-портом (`AGraber/re3-nx`). Живые альтернативы — порты Android-сборок выше.

## Legacy

- **Kosmos** — старая AIO-сборка, заменена на DeepSea/PYXIS.
- **SX OS** — закрытая прошивка, проект мёртв.

## Правила подборки

- Один проект — одна строка: ссылка + короткое описание.
- Помечай `со своими копиями игры`, если нужны файлы игры.
- Заброшенные проекты уходят в `Legacy`.
- PR с новыми проектами приветствуются.

## Лицензия

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
