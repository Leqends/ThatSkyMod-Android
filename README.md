<a id="changelog-top"></a>
<div align="center">
  <h2>更新日志 / Changelog</h2>
  <p>
    维护者 Maintainer：<b>skykn</b> · <a href="mailto:ykncn@msn.com">ykncn@msn.com</a>
    <br />
    当前版本 Current build：<b>v0.34.5</b> · 适配游戏版本 Game version：<b>Sky 0.34.5</b>
  </p>
</div>

---


- **内置简体中文语言包 / Built-in Simplified Chinese translation pack**
  - 中文：内置简体中文语言包，首次启动即自动解包到 `Translations` 目录；仅当内置版本更新时才覆盖，可自由删除或替换。在 设置 → Language & Translations → Available Languages 中选择「简体中文」即可切换。
  - English: A Simplified Chinese translation pack is now built in. It is unpacked into the `Translations` directory on first launch and is only overwritten when the bundled version is newer; it can be deleted or replaced freely. Select "简体中文" under Settings → Language & Translations → Available Languages.


- **全量内存偏移更新 / Full memory offset refresh**
  - 中文：全部游戏内存偏移已更新至 0.34.5，并统一收敛到单一偏移定义文件；后续游戏升级只需维护该文件即可完成适配。
  - English: All game memory offsets have been updated for 0.34.5 and consolidated into a single offset definition file, so adapting to future game updates only requires editing that one file.

- **烛火 / 光翼 / 染料 ESP 点位修复 / Candle, wing buff and dye ESP fixes**
  - 中文：0.34.5 调整了烛火、光翼与染料实体的数据结构，导致相关 ESP 点位为空。已改用新的数据来源，烛火、光翼与染料点位可正常显示，自动收集功能恢复正常。
  - English: 0.34.5 changed the data layout behind candles, wing buffs and dye entities, which left the corresponding ESP markers empty. New data sources are now used, so candle, wing buff and dye markers display correctly again and auto-collection works as expected.

- **回家秒回修复 / Instant "go home" fix**
  - 中文：修复坐下回家需等待约 5 秒的问题，现在约 0.25 秒即可切换关卡。
  - English: Fixed the ~5 second delay when going home while sitting; the level now switches after roughly 0.25 seconds.

- **账号重登 / 光翼重登崩溃修复 / Account & wing buff relog crash fix**
  - 中文：修复 0.34.5 下账号重登与光翼重登导致的崩溃；账号访问链已重构并收敛到偏移定义文件。
  - English: Fixed the crash on account relog and wing buff relog under 0.34.5. The account access chain has been reworked and folded into the offset definition file.

- **账号登录状态判定修正 / Account login state detection fix**
  - 中文：修正账号登录状态的判定值（20 → 28）。此前因状态误判，「保存当前账号」始终处于锁定状态。
  - English: Corrected the account login state value used for detection (20 → 28). "Save Current Account" was previously always locked because the state was misread.

- **Anti Krill / Anti AFK 修复 / Anti Krill & Anti AFK fixes**
  - 中文：修复 0.34.5 下 Anti Krill 与 Anti AFK 失效的问题。
  - English: Fixed Anti Krill and Anti AFK, which had stopped working on 0.34.5.

- **新 Mod 图标 / New mod icon**
  - 中文：替换为新的 Mod 图标（PNG 格式，体积控制在 100 KB 以内，加载更快）。
  - English: Replaced the mod icon with a new one (PNG, kept under 100 KB for faster loading).


---

## 反馈与支持 / Feedback & Support

- 中文：使用中遇到问题，可通过 Discord 或邮件联系维护者 skykn（ykncn@msn.com）。
- English: If you run into any issue, please reach out via Discord or by email to skykn (ykncn@msn.com).

---

<a id="readme-top"></a>
<div align="center">
  <!-- PROJECT LOGO / TITLE -->
  <h1>That Sky Mod (Android)</h1>
    <img src="https://i.ibb.co/qL5TS2q4/icon.png" alt="TSM Logo" width="80" height="80">

  <p align="center">
    An all-in-one mod menu for Sky: Children of the Light
    <br />
  </p>

  <!-- BADGES -->
  <div align="center">
    <a href="https://discord.gg/wyQ9MZSZw">
      <img src="https://img.shields.io/discord/1542073770536079410?color=7289da&logo=discord&logoColor=white&style=for-the-badge" alt="Discord">
    </a>
    <br>
    <a href="https://github.com/XeTrinityz/ThatSkyMod-Android/releases">
      <img src="https://img.shields.io/github/downloads/XeTrinityz/ThatSkyMod-Android/total?style=for-the-badge" alt="Downloads">
    </a>
  </div>

  <!-- HERO IMAGE -->
  <img src="https://i.ibb.co/hRjwR5tx/TSM-A.png" alt="TSM Menu Screenshot">
</div>

---

## About This Repository

This repository hosts the Android binary (.so) for That Sky Mod (TSM). It is intended for end-users who only need to download updates to the mod.

- This is a binaries-only repo for releases of the Android module (`libTSM.so`).
- For help, support, and installation guidance, please visit our Discord.

## Key Features

- **Complete Player Freedom**: Extensive control over gameplay to minimize grind.
- **Exploration & QoL**: Teleports, visual tools, environment control, and more.
- **Automation**: Time-saving utilities so you can focus on having fun.
- **Mod Menu UI**: User-friendly interface for quick access to features.

## Download

- Get the latest Android build here:
  - https://github.com/XeTrinityz/ThatSkyMod-Android/releases/latest
- Asset name typically: `libTSM.so`
- Also included: `Canvas.apk` (recommended for easy setup).
- Older versions are available in the Releases page if needed.

## How to Use (Android)

1. Download `Canvas.apk` and `libTSM.so` from the latest release.
2. Install Canvas (enable installs from unknown sources if prompted).
3. Open Canvas → tap **Add Mod** → select `libTSM.so`.
4. Tap **Live**.
5. Launch Sky: Children of the Light and open the TSM menu in-game.

## Updating

- Replace your existing `libTSM.so` with the one from the latest release.
- Fully restart the game after updating.

## Compatibility

- Target platform: **Android**.
- We aim to support the latest global build of Sky: Children of the Light on Android. Game updates may require a new TSM release.
- If you encounter issues after a game update, check the Releases page or Discord for status and hotfixes.

## Troubleshooting

- **Crashes after update**: Ensure you fully replaced the previous `.so` and that no duplicate copies are being loaded.
- **Game update broke mod**: Check the latest release notes or Discord for a compatibility update.

## Support

- Need help with installation or configuration? Join the community:
  - Discord: https://discord.gg/wyQ9MZSZw

## Disclaimer

- That Sky Mod is an unofficial fan-made modification for Sky: Children of the Light.

- This project is not affiliated with, endorsed by, or sponsored by thatgamecompany (TGC) or Sky: Children of the Light.

- Use at your own risk. Users are responsible for complying with the game's Terms of Service and all applicable laws.

- This project does not include or distribute any proprietary game files, assets, or content belonging to thatgamecompany.

## Credits

- **Developer**: XeTrinityz
- Maintained by the community

<p align="right"><a href="#readme-top">Back to top</a></p>
