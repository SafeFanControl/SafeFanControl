> [!NOTE]
> Usamos GitHub para registrar errores, debatir solicitudes de funciones y publicar los ejecutables.
> SafeFanControl **no** es software de código abierto.

<div align="center">

[English](README.md) | [简体中文](README.zh-Hans.md) | [繁體中文](README.zh-Hant.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Deutsch](README.de.md) | **Español** | [Français](README.fr.md) | [Русский](README.ru.md)

</div>

---

# SafeFanControl

**Toma el control de los ventiladores de tu Mac**

SafeFanControl es una **app nativa de macOS** que te permite monitorizar temperaturas y gestionar la velocidad de los ventiladores en Macs con Apple Silicon e Intel. Descarga gratuita: tus ventiladores, tus reglas, y el sistema siempre recupera el control si algo va mal.

[Descargar para macOS](https://github.com/SafeFanControl/SafeFanControl/releases)

---

## Características

### Todos los modos de control de ventiladores que puedas necesitar

SafeFanControl te da el control total sobre cómo responde tu Mac al calor, con tres modos de funcionamiento distintos para adaptarse a tu flujo de trabajo.

- **Monitor** — lee temperaturas y velocidades de ventilador en tiempo real sin tocar el control del sistema
- **Safe Max** — sube automáticamente a la velocidad máxima cuando se alcanza un umbral de temperatura y devuelve el control a macOS cuando se enfría
- **Curve** — define tu propia curva de temperatura a velocidad para un control continuo y proporcional
- Cambia de modo al instante desde la barra de menús, sin abrir ninguna ventana

### Diseñado pensando primero en la seguridad

Una arquitectura de tres procesos garantiza que, si algo va mal, macOS siempre recupera automáticamente el control de los ventiladores, sin ninguna intervención manual.

- Un **proceso de vigilancia (watchdog)** supervisa el ayudante en segundo plano; si se bloquea mientras los ventiladores están en modo manual, macOS toma el control al instante
- Las **transiciones suaves de atenuación** evitan saltos bruscos de velocidad que podrían resultar audibles o molestos
- El **enganche por umbral** mantiene Safe Max estable durante fluctuaciones breves de temperatura
- El diálogo de administrador estándar de macOS instala el ayudante en segundo plano: sin Terminal, sin pasos manuales

### Siempre en la barra de menús

Una app ligera en la barra de menús pone los datos de los sensores en vivo y el cambio de modo a un clic de distancia: siempre visible, nunca estorba.

- Temperaturas de CPU y GPU actualizadas en tiempo real
- Velocidad actual del ventilador y modo de control activo siempre visibles
- Cambia entre Monitor, Safe Max y Curve directamente desde el menú desplegable
- Compatible con Apple Silicon de M1 a M5 y Macs Intel con chip T2; disponible en 8 idiomas

---

## Precio

SafeFanControl sigue un modelo de **descarga gratuita y compra única**. Sin suscripciones. Sin cuotas recurrentes. Paga una vez y es tuyo para siempre.

| | Gratis | Licencia completa |
|---|---|---|
| **Precio** | $0 — para siempre | $8.99 — pago único |
| Modo Monitor (solo lectura) | ✅ | ✅ |
| Visualización de temperatura en vivo | ✅ | ✅ |
| Visualización de la velocidad del ventilador | ✅ | ✅ |
| Sensores de CPU, GPU y SoC | ✅ | ✅ |
| Reconocimiento por generación M1–M5 | ✅ | ✅ |
| **Modo Safe Max** | ❌ | ✅ |
| **Modo Curve** | ❌ | ✅ |
| Transiciones suaves de atenuación | ❌ | ✅ |
| Lógica de enganche / sin rebotes | ❌ | ✅ |
| Safe Max con múltiples reglas | ❌ | ✅ |
| **Asistente de prueba de ventiladores** | ❌ | ✅ |
| Página de depuración y diagnóstico | ❌ | ✅ |

---

## Descarga e instalación

### Requisitos del sistema

| Requisito | Detalles |
|---|---|
| **macOS** | 15 (Sequoia) o posterior |
| **Hardware Mac** | Apple Silicon (M1, M2, M3, M4, M5) o Mac Intel con chip T2 |
| **Permisos** | Una solicitud de contraseña de administrador para instalar el daemon ayudante en segundo plano |
| **Espacio en disco** | ~5 MB |

### Instalación

1. **Abre el `.dmg` descargado** y arrastra SafeFanControl a tu carpeta de Aplicaciones.
2. **Abre la app.** En el primer arranque, un diálogo de administrador instala el ayudante en segundo plano y el daemon de vigilancia.
3. **Listo.** Sin Terminal. Sin aprobaciones manuales. El Asistente de prueba de ventiladores te guiará para confirmar que todo funciona en tu hardware.

> macOS puede mostrar un aviso de Gatekeeper en el primer arranque, ya que la app no se distribuye por el App Store. Haz **clic derecho → Abrir** para continuar.

### Desinstalación

SafeFanControl incluye un proceso de desinstalación completo en **Ajustes → Desinstalar**. Elimina el daemon ayudante, el daemon de vigilancia y todos los archivos asociados en un solo paso.

---

## Preguntas frecuentes

**¿Hay una prueba gratuita de las funciones completas?**
Sí — los modos Safe Max y Curve se desbloquean durante una **prueba de 14 días** al iniciar la app por primera vez. No se requiere pago.

**¿Qué cubre la licencia?**
Una licencia cubre todos tus Macs **personales**. No es para redistribución ni uso comercial en flotas de equipos.

**¿Tengo que volver a comprar tras actualizar macOS?**
No. Tu licencia es permanente.

**¿Tengo que volver a comprar si consigo un Mac nuevo?**
No — tu licencia te pertenece. Usa tu clave de licencia existente para registrar tu nuevo Mac.

**¿Cuál es vuestra política de reembolso?**
Como respetamos tu privacidad, la app usa un sistema de registro sin conexión. Una vez emitida, una clave de licencia no puede desactivarse de forma remota, por lo que todas las ventas son definitivas y no se pueden emitir reembolsos estándar. Te recomendamos encarecidamente usar la prueba de 14 días antes de comprar. Excepción: si una actualización de macOS de Apple deshabilita de forma permanente los métodos de control de ventiladores subyacentes, emitiremos un reembolso completo para las licencias compradas en los últimos 30 días.

**¿Por qué la app no está en la Mac App Store?**
SafeFanControl instala un daemon ayudante privilegiado en segundo plano, lo cual es incompatible con las estrictas reglas de aislamiento (sandbox) del App Store. La distribución es directa, pero el instalador se analiza, notariza y firma a través del sistema de firma de Apple.

**¿Puedo usarla sin pagar?**
Sí — el modo Monitor es completamente gratuito y siempre lo será.

**¿Qué pasa si el servidor de licencias se desconecta en el futuro?**
La clave de licencia funciona sin conexión y no requiere comprobación por internet. Puedes registrarte en cualquier momento, siempre que conserves tu clave de licencia.

**¿Qué pasa si abandonas este proyecto?**
Todo producto tiene una vida útil. Sin embargo, mientras pueda programar y los ingresos del producto cubran sus gastos básicos (como la cuota anual del Apple Developer Program), seguiré manteniéndolo. Si te gusta este producto, compártelo con tus amigos. Si (y solo si) llega el día en que tenga que abandonar este proyecto, compartiré el código fuente con todos los usuarios de pago bajo la licencia AGPL v3.

**¿Qué pasa si pierdo mi clave de licencia?**
Ponte en contacto con la plataforma de venta o escríbenos directamente.

---

## Privacidad

SafeFanControl **no** recopila telemetría, analíticas ni informes de errores. Los datos de tu hardware permanecen en tu dispositivo.
