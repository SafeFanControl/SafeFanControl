> [!NOTE]
> We use GitHub to track bugs, discuss feature requests, and release executables.
> SafeFanControl is **not** open-source software.

<div align="center">

[English](#english) | [中文](#中文) | [Русский](#русский) | [日本語](#日本語)

</div>

---

<a id="english"></a>

# SafeFanControl

**Take Control of Your Mac's Fans**

SafeFanControl is a **native macOS app** that lets you monitor temperatures and manage fan speeds on Apple Silicon and Intel Macs. Free to download — your fans, your rules, and the system always gets them back if anything goes wrong.

[Download for macOS](https://github.com/SafeFanControl/SafeFanControl/releases)

---

## Features

### All the Fan Control Modes You May Need

SafeFanControl gives you complete control over how your Mac responds to heat, with three distinct operating modes to match your workflow.

- **Monitor** — read live temperatures and fan speeds without touching system control
- **Safe Max** — automatically ramp to full speed when a temperature threshold is hit, then return control to macOS when it cools down
- **Curve** — define a custom temperature-to-speed curve for continuous proportional control
- Switch modes instantly from the menu bar — no app window required

### Designed for Safety First

A three-process architecture ensures that if anything goes wrong, macOS always gets fan control back automatically — with no manual intervention needed.

- **Watchdog process** monitors the helper daemon; if it crashes while fans are in manual mode, macOS takes over instantly
- **Smooth fade transitions** prevent abrupt fan speed jumps that could be audible or disruptive
- **Threshold latching** keeps Safe Max stable during brief temperature fluctuations
- Standard macOS admin prompt installs the background helper — no Terminal, no manual steps

### Always in the Menu Bar

A lightweight menu bar app puts live sensor data and mode switching one click away — always visible, never in the way.

- Live CPU and GPU temperatures updated in real time
- Current fan speed and active control mode always visible
- Switch between Monitor, Safe Max, and Curve directly from the dropdown
- Supports M1 through M5 Apple Silicon and Intel T2 Macs; available in English and Japanese

---

## Pricing

SafeFanControl follows a **free download, one-time purchase** model. No subscriptions. No recurring fees. Pay once, own it forever.

| | Free | Full License |
|---|---|---|
| **Price** | $0 — forever | $8.99 — one-time |
| Monitor mode (read-only) | ✅ | ✅ |
| Live temperature display | ✅ | ✅ |
| Fan speed display | ✅ | ✅ |
| CPU, GPU, SoC sensors | ✅ | ✅ |
| M1–M5 generation-aware | ✅ | ✅ |
| **Safe Max mode** | ❌ | ✅ |
| **Curve mode** | ❌ | ✅ |
| Smooth fade transitions | ❌ | ✅ |
| Latch / no-bounce logic | ❌ | ✅ |
| Multi-rule Auto Max | ❌ | ✅ |
| **Fan test wizard** | ❌ | ✅ |
| Debug & diagnostics page | ❌ | ✅ |

---

## Download & Install

### System Requirements

| Requirement | Details |
|---|---|
| **macOS** | 15 (Sequoia) or later |
| **Mac hardware** | Apple Silicon (M1, M2, M3, M4, M5) or Intel Mac with T2 chip |
| **Permissions** | One admin password prompt to install the background helper daemon |
| **Disk space** | ~5 MB |

### Installation

1. **Open the downloaded `.dmg`** and drag SafeFanControl to your Applications folder.
2. **Launch the app.** On first run, an admin dialog installs the background helper and watchdog daemons.
3. **Done.** No Terminal. No manual approvals. The Fan Test Wizard will guide you through confirming everything works on your hardware.

> macOS may show a Gatekeeper prompt on first launch since the app is not App Store distributed. **Right-click → Open** to proceed.

### Uninstall

SafeFanControl includes a complete uninstall flow in **Settings → Uninstall**. It removes the helper daemon, watchdog daemon, and all associated files in one step.

---

## FAQ

**Is there a free trial for the full features?**
Yes — Safe Max and Curve modes are unlocked for a **14-day trial** upon first launch. No payment required.

**What does the license cover?**
One license covers all your **personal** Macs. It is not for redistribution or commercial fleet use.

**Do I need to re-purchase after a macOS upgrade?**
No. Your license is permanent.

**Do I need to re-purchase if I get a new Mac?**
No — your license belongs to you. Use your existing license key to register on your new Mac.

**What is your refund policy?**
Because we respect your privacy, the app uses an offline registration system. Once a license key is issued, it cannot be remotely deactivated — therefore all sales are final and standard refunds cannot be issued. We strongly encourage you to use the 14-day trial before purchasing. Exception: if an Apple macOS update permanently disables the underlying fan control methods, we will issue a full refund for licenses purchased within the last 30 days.

**Why isn't the app on the Mac App Store?**
SafeFanControl installs a privileged background helper daemon, which is incompatible with the App Store's strict sandboxing rules. Distribution is direct — but the installer is scanned, notarized, and signed through Apple's signing system.

**Can I use it without paying?**
Yes — Monitor mode is completely free and always will be.

**What happens if the licensing server goes offline in the future?**
The license key works offline and does not require an internet check. You can register at any time, as long as you still have your license key.

**What if you abandon this project?**
Every product has a lifespan. However, as long as I am able to code and the product's revenue covers its basic expenses (such as the yearly Apple Developer Program fee), I will continue maintaining it. If you like this product, please share it with your friends. If (and only if) the day comes when I have to abandon this project, I will share the source code with all paid users under the AGPL v3 license.

**What if I lose my license key?**
Please reach out to the vendor platform or contact us directly.

---

## Privacy

SafeFanControl does **not** collect telemetry, analytics, or crash reports. Your hardware data stays on your device.

---

<a id="中文"></a>

# SafeFanControl

**掌控你 Mac 的风扇**

SafeFanControl 是一款**原生 macOS 应用**，让你监控温度、管理 Apple Silicon 和 Intel Mac 的风扇转速。免费下载——你的风扇，你做主，出现任何问题系统都会自动接管。

[下载 macOS 版本](https://github.com/SafeFanControl/SafeFanControl/releases)

---

## 功能特性

### 你所需的全部风扇控制模式

SafeFanControl 提供三种不同的运行模式，完全满足你对 Mac 散热控制的需求。

- **监控** — 实时读取温度和风扇转速，不干预系统控制
- **安全最高速** — 当温度超过阈值时自动提速至最高转速，温度降低后将控制权交还 macOS
- **曲线** — 自定义温度-转速曲线，实现连续比例控制
- 随时从菜单栏切换模式，无需打开应用窗口

### 安全优先的设计

三进程架构确保出现任何问题时，macOS 都能自动取回风扇控制权，无需任何手动干预。

- **守护进程**监控助手守护程序；若在手动模式下崩溃，macOS 将立即接管
- **平滑淡入淡出过渡**防止风扇转速突变造成噪音或干扰
- **阈值锁定**在短暂温度波动时保持安全最高速稳定运行
- 标准 macOS 管理员提示安装后台助手——无需终端，无需手动操作

### 始终在菜单栏

轻量级菜单栏应用让实时传感器数据和模式切换只需一键——始终可见，从不妨碍使用。

- 实时 CPU 和 GPU 温度更新
- 当前风扇转速和活动控制模式始终可见
- 直接从下拉菜单在监控、安全最高速和曲线模式之间切换
- 支持 M1 至 M5 Apple Silicon 及搭载 T2 芯片的 Intel Mac；提供英文和日文界面

---

## 定价

SafeFanControl 采用**免费下载、一次性购买**模式。无订阅，无循环收费，一次付费永久拥有。

| | 免费版 | 完整许可 |
|---|---|---|
| **价格** | $0 — 永久免费 | $8.99 — 一次性付费 |
| 监控模式（只读）| ✅ | ✅ |
| 实时温度显示 | ✅ | ✅ |
| 风扇转速显示 | ✅ | ✅ |
| CPU、GPU、SoC 传感器 | ✅ | ✅ |
| M1–M5 代感知 | ✅ | ✅ |
| **安全最高速模式** | ❌ | ✅ |
| **曲线模式** | ❌ | ✅ |
| 平滑过渡 | ❌ | ✅ |
| 锁定 / 防抖动逻辑 | ❌ | ✅ |
| 多规则自动最高速 | ❌ | ✅ |
| **风扇测试向导** | ❌ | ✅ |
| 调试与诊断页面 | ❌ | ✅ |

---

## 下载与安装

### 系统要求

| 需求 | 详情 |
|---|---|
| **macOS** | 15 (Sequoia) 或更高版本 |
| **Mac 硬件** | Apple Silicon（M1、M2、M3、M4、M5）或搭载 T2 芯片的 Intel Mac |
| **权限** | 安装后台助手守护程序需要一次管理员密码提示 |
| **磁盘空间** | 约 5 MB |

### 安装步骤

1. **打开下载的 `.dmg`**，将 SafeFanControl 拖入应用程序文件夹。
2. **启动应用。** 首次运行时，管理员对话框将安装后台助手和守护进程。
3. **完成。** 无需终端，无需手动操作。风扇测试向导将引导你确认一切在你的硬件上正常运行。

> 由于应用不通过 App Store 分发，macOS 在首次启动时可能显示 Gatekeeper 提示。请**右键点击 → 打开**继续。

### 卸载

SafeFanControl 在**设置 → 卸载**中提供完整卸载流程，一步移除助手守护进程、看门狗守护进程及所有相关文件。

---

## 常见问题

**有免费试用吗？**
有——首次启动后，安全最高速和曲线模式可免费试用 **14 天**，无需付款。

**许可证覆盖范围是什么？**
一个许可证涵盖你所有**个人** Mac，不可用于再分发或商业用途。

**macOS 升级后需要重新购买吗？**
不需要，许可证永久有效。

**更换新 Mac 需要重新购买吗？**
不需要——许可证属于你个人。使用现有许可证密钥即可在新 Mac 上注册。

**退款政策是什么？**
由于我们尊重你的隐私，应用采用离线注册系统。许可证密钥一经颁发无法远程停用，因此所有销售均为最终销售，不支持标准退款。我们强烈建议在购买前使用 14 天免费试用。例外：若 Apple macOS 更新永久禁用了风扇控制所用的底层方法，我们将对过去 30 天内购买的许可证给予全额退款。

**为什么不在 Mac App Store 上架？**
SafeFanControl 需要安装特权后台助手守护程序，与 App Store 严格的沙盒规则不兼容，因此直接分发。但安装包已通过 Apple 签名系统进行扫描、公证和签名。

**免费可以使用吗？**
是的——监控模式完全免费且永久免费。

**许可证服务器将来下线怎么办？**
许可证密钥离线工作，无需联网验证，只要你还有许可证密钥，随时可注册。

**如果你放弃这个项目怎么办？**
每个产品都有生命周期。但只要我还能编程，且产品收入能覆盖基本开销（如年度 Apple 开发者计划费用），我就会持续维护。如果你喜欢这款产品，请分享给朋友。如果（仅当）有朝一日我不得不放弃这个项目，我将以 AGPL v3 许可证向所有付费用户开放源代码。

**丢失许可证密钥怎么办？**
请联系销售平台或直接联系我们。

---

## 隐私

SafeFanControl **不**收集遥测数据、分析数据或崩溃报告。你的硬件数据留在你的设备上。

---

<a id="русский"></a>

# SafeFanControl

**Возьмите под контроль вентиляторы вашего Mac**

SafeFanControl — это **нативное приложение для macOS**, которое позволяет отслеживать температуры и управлять скоростью вентиляторов на Mac с Apple Silicon и Intel. Бесплатно для загрузки — ваши вентиляторы, ваши правила, а система всегда возвращает управление, если что-то пойдёт не так.

[Скачать для macOS](https://github.com/SafeFanControl/SafeFanControl/releases)

---

## Возможности

### Все режимы управления вентиляторами, которые вам нужны

SafeFanControl предоставляет полный контроль над реакцией Mac на нагрев с тремя различными режимами работы.

- **Мониторинг** — считывание температур и скоростей в реальном времени без вмешательства в управление системой
- **Безопасный максимум** — автоматическое увеличение скорости до максимума при превышении порога температуры, с возвратом управления macOS после охлаждения
- **Кривая** — задайте пользовательскую кривую «температура-скорость» для непрерывного пропорционального управления
- Мгновенное переключение режимов из строки меню — без открытия окна приложения

### Безопасность прежде всего

Трёхпроцессная архитектура гарантирует, что при любой проблеме macOS автоматически возвращает контроль над вентиляторами без ручного вмешательства.

- **Сторожевой процесс** следит за вспомогательным демоном; при аварийном завершении в ручном режиме macOS немедленно берёт управление
- **Плавные переходы** предотвращают резкие изменения скорости вентиляторов
- **Фиксация порога** обеспечивает стабильную работу «Безопасного максимума» при кратковременных колебаниях температуры
- Стандартный запрос прав администратора macOS для установки фонового помощника — без Терминала, без ручных действий

### Всегда в строке меню

Лёгкое приложение в строке меню обеспечивает доступ к данным датчиков и переключению режимов в один клик — всегда видно, никогда не мешает.

- Температуры CPU и GPU обновляются в реальном времени
- Текущая скорость вентиляторов и активный режим управления всегда на виду
- Переключение между «Мониторингом», «Безопасным максимумом» и «Кривой» прямо из выпадающего меню
- Поддержка Apple Silicon от M1 до M5 и Intel Mac с чипом T2; доступно на английском и японском

---

## Цены

SafeFanControl распространяется по модели **бесплатная загрузка, разовая покупка**. Никаких подписок. Никаких повторяющихся платежей. Заплатите один раз — пользуйтесь навсегда.

| | Бесплатно | Полная лицензия |
|---|---|---|
| **Цена** | $0 — навсегда | $8.99 — разово |
| Режим мониторинга (только чтение) | ✅ | ✅ |
| Отображение температур в реальном времени | ✅ | ✅ |
| Отображение скорости вентиляторов | ✅ | ✅ |
| Датчики CPU, GPU, SoC | ✅ | ✅ |
| Поддержка поколений M1–M5 | ✅ | ✅ |
| **Режим «Безопасный максимум»** | ❌ | ✅ |
| **Режим «Кривая»** | ❌ | ✅ |
| Плавные переходы | ❌ | ✅ |
| Логика фиксации / подавления дребезга | ❌ | ✅ |
| Авто-максимум с несколькими правилами | ❌ | ✅ |
| **Мастер тестирования вентиляторов** | ❌ | ✅ |
| Страница отладки и диагностики | ❌ | ✅ |

---

## Загрузка и установка

### Системные требования

| Требование | Детали |
|---|---|
| **macOS** | 15 (Sequoia) или новее |
| **Оборудование Mac** | Apple Silicon (M1, M2, M3, M4, M5) или Intel Mac с чипом T2 |
| **Разрешения** | Один запрос пароля администратора для установки фонового демона |
| **Место на диске** | ~5 МБ |

### Установка

1. **Откройте загруженный `.dmg`** и перетащите SafeFanControl в папку «Программы».
2. **Запустите приложение.** При первом запуске диалоговое окно администратора установит фоновый помощник и сторожевой демон.
3. **Готово.** Без Терминала. Без ручных действий. Мастер тестирования вентиляторов проведёт вас через проверку работы на вашем оборудовании.

> macOS может показать запрос Gatekeeper при первом запуске, так как приложение распространяется не через App Store. Нажмите **правой кнопкой → Открыть**, чтобы продолжить.

### Удаление

SafeFanControl включает полный процесс удаления в **Настройки → Удалить**. Удаляет демон помощника, сторожевой демон и все связанные файлы за один шаг.

---

## Часто задаваемые вопросы

**Есть ли пробный период для полных функций?**
Да — режимы «Безопасный максимум» и «Кривая» доступны в течение **14-дневного пробного периода** при первом запуске. Оплата не требуется.

**Что покрывает лицензия?**
Одна лицензия покрывает все ваши **личные** Mac. Не предназначена для коммерческого использования или распространения.

**Нужно ли повторно покупать после обновления macOS?**
Нет. Лицензия постоянная.

**Нужно ли покупать повторно при смене Mac?**
Нет — лицензия принадлежит вам. Используйте существующий лицензионный ключ для регистрации на новом Mac.

**Какова политика возврата?**
Поскольку мы уважаем вашу конфиденциальность, приложение использует офлайн-систему регистрации. После выдачи лицензионного ключа его нельзя удалённо деактивировать — поэтому все продажи окончательны и стандартные возвраты невозможны. Настоятельно рекомендуем использовать 14-дневный пробный период перед покупкой. Исключение: если обновление macOS навсегда отключит используемые методы управления вентиляторами, мы вернём полную стоимость для лицензий, приобретённых за последние 30 дней.

**Почему приложение не в Mac App Store?**
SafeFanControl устанавливает привилегированный фоновый демон, несовместимый с правилами песочницы App Store. Распространение прямое — но установочный пакет проверен, нотаризован и подписан через систему подписи Apple.

**Можно ли использовать бесплатно?**
Да — режим «Мониторинг» полностью бесплатен и всегда будет таким.

**Что если сервер лицензий отключится в будущем?**
Лицензионный ключ работает офлайн и не требует проверки через интернет. Вы можете зарегистрировать его в любое время, пока у вас есть ключ.

**Что если проект будет заброшен?**
У каждого продукта есть жизненный цикл. Но пока я могу программировать и доходы покрывают основные расходы (например, ежегодный взнос Apple Developer Program), я буду поддерживать проект. Если вам нравится этот продукт — поделитесь им с друзьями. Если (и только если) придётся закрыть проект — исходный код будет открыт для всех платных пользователей под лицензией AGPL v3.

**Что если я потеряю лицензионный ключ?**
Обратитесь к платформе продавца или напрямую к нам.

---

## Конфиденциальность

SafeFanControl **не** собирает телеметрию, аналитику или отчёты об ошибках. Данные о вашем оборудовании остаются на вашем устройстве.

---

<a id="日本語"></a>

# SafeFanControl

**Mac のファンをあなたの手に**

SafeFanControl は、Apple Silicon および Intel Mac でCPU温度を監視し、ファン回転数を管理できる**ネイティブ macOS アプリ**です。無料でダウンロード——あなたのファン、あなたのルール、何か問題が起きてもシステムが自動的に制御を取り戻します。

[macOS 版をダウンロード](https://github.com/SafeFanControl/SafeFanControl/releases)

---

## 機能

### 必要なすべてのファン制御モード

SafeFanControl は、ワークフローに合わせた3つの動作モードで、Mac の熱への対応を完全にコントロールします。

- **モニター** — システム制御に触れることなく、温度とファン回転数をリアルタイムで読み取る
- **セーフマックス** — 温度しきい値に達すると自動的に最高回転数へ上げ、冷却後に macOS へ制御を返す
- **カーブ** — 連続的な比例制御のためのカスタム温度-回転数カーブを設定
- メニューバーからいつでもモード切替——アプリウィンドウ不要

### 安全ファースト設計

3プロセスアーキテクチャにより、何か問題が起きた場合でも、macOS が自動的にファン制御を取り戻します。手動操作は一切不要です。

- **ウォッチドッグプロセス**がヘルパーデーモンを監視し、手動モード中にクラッシュした場合は macOS が即座に制御を引き継ぐ
- **スムーズなフェード移行**で急激なファン回転数の変化を防止
- **しきい値ラッチ**で一時的な温度変動時もセーフマックスを安定動作させる
- 標準の macOS 管理者プロンプトでバックグラウンドヘルパーをインストール——ターミナル不要、手動操作不要

### 常にメニューバーに

軽量なメニューバーアプリが、ライブセンサーデータとモード切替をワンクリックで提供——常に見える、決して邪魔にならない。

- CPU と GPU の温度をリアルタイム更新
- 現在のファン回転数と制御モードを常時表示
- ドロップダウンからモニター、セーフマックス、カーブを直接切替
- M1〜M5 Apple Silicon および T2 チップ搭載 Intel Mac をサポート；英語・日本語対応

---

## 価格

SafeFanControl は**無料ダウンロード、買い切り**モデルです。サブスクリプションなし。継続課金なし。一度購入すれば永遠に使用可能。

| | 無料 | フルライセンス |
|---|---|---|
| **価格** | $0 — 永久無料 | $8.99 — 買い切り |
| モニターモード（読み取りのみ）| ✅ | ✅ |
| リアルタイム温度表示 | ✅ | ✅ |
| ファン回転数表示 | ✅ | ✅ |
| CPU・GPU・SoC センサー | ✅ | ✅ |
| M1–M5 世代対応 | ✅ | ✅ |
| **セーフマックスモード** | ❌ | ✅ |
| **カーブモード** | ❌ | ✅ |
| スムーズなフェード移行 | ❌ | ✅ |
| ラッチ / チャタリング防止ロジック | ❌ | ✅ |
| マルチルール自動最大速 | ❌ | ✅ |
| **ファンテストウィザード** | ❌ | ✅ |
| デバッグ & 診断ページ | ❌ | ✅ |

---

## ダウンロードとインストール

### システム要件

| 要件 | 詳細 |
|---|---|
| **macOS** | 15 (Sequoia) 以降 |
| **Mac ハードウェア** | Apple Silicon（M1、M2、M3、M4、M5）または T2 チップ搭載 Intel Mac |
| **権限** | バックグラウンドヘルパーデーモンのインストールに管理者パスワードが1回必要 |
| **ディスク容量** | 約 5 MB |

### インストール手順

1. **ダウンロードした `.dmg` を開き**、SafeFanControl をアプリケーションフォルダにドラッグします。
2. **アプリを起動します。** 初回起動時に、管理者ダイアログがバックグラウンドヘルパーとウォッチドッグデーモンをインストールします。
3. **完了。** ターミナル不要。手動操作不要。ファンテストウィザードがハードウェアで正常に動作することを確認する手順を案内します。

> アプリは App Store 経由で配布されていないため、初回起動時に macOS の Gatekeeper プロンプトが表示される場合があります。**右クリック → 開く**で続行してください。

### アンインストール

SafeFanControl には**設定 → アンインストール**に完全なアンインストールフローが含まれています。ヘルパーデーモン、ウォッチドッグデーモン、および関連するすべてのファイルを1ステップで削除します。

---

## よくある質問

**フル機能の無料試用はありますか？**
はい——初回起動後、セーフマックスとカーブモードが**14日間**無料で使えます。支払い不要です。

**ライセンスの対象範囲は？**
1つのライセンスですべての**個人用** Mac が対象です。再配布や商業用途には使用できません。

**macOS アップグレード後に再購入は必要ですか？**
不要です。ライセンスは永続的です。

**新しい Mac に買い替えた場合は？**
不要です——ライセンスはあなたのものです。既存のライセンスキーで新しい Mac に登録できます。

**返金ポリシーは？**
プライバシーを尊重するため、アプリはオフライン登録システムを採用しています。ライセンスキーは一度発行されると遠隔無効化できないため、すべての販売は最終的なものであり、標準的な返金はできません。購入前に14日間の無料試用を強くお勧めします。例外：Apple macOS アップデートによりファン制御に使用する基盤的な方法が永続的に無効化された場合、過去30日以内に購入されたライセンスについて全額返金いたします。

**なぜ Mac App Store にないのですか？**
SafeFanControl は特権バックグラウンドヘルパーデーモンをインストールするため、App Store の厳格なサンドボックス規則と互換性がありません。直接配布していますが、インストールパッケージは Apple の署名システムを通じてスキャン、公証、署名されています。

**無料で使えますか？**
はい——モニターモードは完全無料で、常に無料です。

**ライセンスサーバーが将来オフラインになったら？**
ライセンスキーはオフラインで動作し、インターネット確認は不要です。ライセンスキーが手元にある限り、いつでも登録できます。

**プロジェクトを放棄した場合は？**
すべての製品には寿命があります。しかし、コードを書ける限り、製品の収益が基本的な費用（年次 Apple Developer Program の料金など）をカバーする限り、維持し続けます。気に入っていただけたら、ぜひ友人に紹介してください。もし（もしも）このプロジェクトを放棄せざるを得ない日が来たとしたら、AGPL v3 ライセンスの下でプログラムのソースコードをすべての有料ユーザーと共有します。

**ライセンスキーを紛失した場合は？**
販売プラットフォームまたは直接お問い合わせください。

---

## プライバシー

SafeFanControl はテレメトリー、分析データ、クラッシュレポートを**一切**収集しません。ハードウェアデータはデバイス上に留まります。
