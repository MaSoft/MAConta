# MAConta

Contabilidad de casa en el móvil y en el ordenador: apuntar gastos, ingresos y transferencias entre cuentas, ver saldos y estadísticas, y exportarlo todo a Excel. Los datos se guardan cifrados y no se envían a internet.

**Aplicación gratuita para Android y Windows desarrollada por [Masoft.es](https://masoft.es)**

- **Android 1.5.0:** [descargar el APK](https://github.com/MaSoft/MAConta/releases/tag/android-v1.5.0)
- **Windows 1.2.0:** [descargar el instalador](https://github.com/MaSoft/MAConta/releases/tag/escritorio-v1.2.0)

Más información y los manuales también en [masoft.es](https://masoft.es/android.html#maconta).

![MAConta en el ordenador y en el móvil](capturas/01-portada-portada.webp)

**Funcionan juntas.** El PC hace de servidor y el móvil se sincroniza con él por la red de casa: emparejados con un código QR, cifrado AES-256 y automático, sin cuentas ni nube. Cada una funciona también sola.

## Android 1.5.0

**Android 13 o superior · 58,7 MB** · [Descargar](https://github.com/MaSoft/MAConta/releases/tag/android-v1.5.0) (`MAConta-1.5.0.apk`)

### Qué hace
- Movimientos en tres vistas, diario, calendario y mensual, con totales por día, semana y mes.
- Transferencias entre cuentas en un solo apunte, con la comisión como gasto.
- Estadísticas de gastos e ingresos por categoría, evolución de 12 meses, por cuenta y presupuestos.
- Tickets y facturas con la cámara: la foto se guarda y el movimiento se abre ya relleno para revisarlo.
- Pendientes: libreta de lo que te deben y de lo que debes, sin tocar los saldos.
- Recibos con cargo mensual, aviso antes de cada cargo y «Próximo mes» para calcular lo que vas a ingresar y gastar.
- Movimientos repetidos (recibos y nóminas que se apuntan solos), plantillas, calculadora en el importe y autocompletado.
- Exportación a Excel o CSV, copia automática diaria (se guardan 15) y copias manuales donde elijas.
- Base de datos cifrada, bloqueo opcional con huella o PIN, y tema claro u oscuro.

### Requisitos

| | |
|---|---|
| Sistema | Android 13 o superior |
| Permisos | Huella o PIN solo si se activa el bloqueo, y red local para sincronizar con el PC. No envía nada a internet. |
| Instalación | Se descarga el APK en el móvil y se abre; Android pide permiso para instalar aplicaciones de esa fuente. |
| Actualizar | La versión nueva se instala encima de la anterior sin perder los datos. |

### Capturas

| | |
|---|---|
| ![Movimientos y cuentas](capturas/02-movil-movimientos.webp)<br>**Movimientos y cuentas.** Diario del mes con ingresos, gastos y balance, y saldos por cuenta con activos, deudas y total. | ![Estadísticas](capturas/03-movil-estadisticas.webp)<br>**Estadísticas.** Gastos por categoría con su porcentaje y evolución de ingresos y gastos mes a mes. |
| ![Recibos y mes actual](capturas/04-movil-recibos.webp)<br>**Recibos y mes actual.** Recibos con cargo mensual y su próximo cargo, y la calculadora del mes con recibos e ingresos fijos. |  |

Comprobar la descarga en PowerShell: `Get-FileHash .\MAConta-1.5.0.apk` debe dar `6a4bc3f7d43fa940b37f7f861e09f1f3c77403de551173330e2ec90c3af65ebf`.

## Windows 1.2.0

**Windows 10 u 11 (64 bits) · 44,5 MB** · [Descargar](https://github.com/MaSoft/MAConta/releases/tag/escritorio-v1.2.0) (`MAConta_Escritorio_Setup_v1.2.0.exe`)

### Qué hace
- Diario, calendario y mensual con tablas grandes y ordenables, y resumen por semanas o meses.
- Ticket desde archivo: de una foto o un PDF, el OCR de Windows lee el total, la fecha, la hora y los datos del comercio.
- Importación de cualquier Excel o CSV de bancos y otras apps, con mapeo de columnas y perfiles.
- Estadísticas: anillo por categoría con subcategorías, barras de 12 meses y resumen por cuenta.
- Exportación a Excel, CSV e informe HTML interactivo, del periodo o de todo.
- Pendientes, copias automáticas diarias y manuales con los tickets, en el mismo formato que el móvil.
- Sincronización con el móvil emparejado por QR, cifrada y automática, con registro de conflictos.
- Tema claro u oscuro como Windows, y todos los datos en la carpeta del programa.

### Requisitos

| | |
|---|---|
| Sistema | Windows 10 u 11 (64 bits) |
| Instalación | Instalador para tu usuario: no pide permisos de administrador ni necesita Python. |
| Pantalla | 1080 × 680 como mínimo |
| Con el móvil | PC y móvil en la misma red y el puerto 47850 (TCP y UDP) permitido en el cortafuegos para redes privadas. |

Windows puede mostrar el aviso «Windows protegió su PC» porque el instalador no está firmado: «Más información» y «Ejecutar de todas formas».

### Capturas

| | |
|---|---|
| ![Movimientos](capturas/05-pc-pc_movimientos.webp)<br>**Movimientos.** Tabla ordenable del mes con ingresos, gastos, total y botón para leer un ticket. | ![Estadísticas](capturas/06-pc-pc_estadisticas.webp)<br>**Estadísticas.** Gastos por categoría en anillo y en tabla, presupuestos y evolución de 12 meses. |
| ![Cuentas](capturas/07-pc-pc_cuentas.webp)<br>**Cuentas.** Saldos por grupo y por cuenta, con activos, deudas y total. |  |

Comprobar la descarga en PowerShell: `Get-FileHash .\MAConta_Escritorio_Setup_v1.2.0.exe` debe dar `529e003e3e856953c23f20f465b685073bbd7293368a64f5c611323745f04657`.

## Instalación

- **Android:** las aplicaciones no están en Google Play. Se descarga el APK en el móvil y se abre; Android pide permiso para instalar aplicaciones de esa fuente y Google Play Protect puede avisar de que no conoce la aplicación.
- **Windows:** el instalador no está firmado digitalmente: Windows puede mostrar «Windows protegió su PC». Pulsa «Más información» y «Ejecutar de todas formas».

En cada versión de [Releases](https://github.com/MaSoft/MAConta/releases) están el archivo, su huella SHA-256 y el manual.

## Aviso legal

MAConta es gratuito y se entrega tal cual, sin garantía de ningún tipo. Al descargarlo y usarlo aceptas el aviso legal y las limitaciones de su manual.

> ⚠ MAConta es una herramienta de uso personal. Los cálculos dependen de los datos introducidos o importados; no sustituye a documentos bancarios ni tiene validez contable o fiscal.

**Limitaciones y exclusión de responsabilidad**
- Solo euros; no maneja varias monedas.
- Las copias .mcbak no están cifradas.
- La sincronización funciona en la red local (o una VPN a casa); no hay servidor en Internet.
- Importar MMBAK (en el escritorio) se basa en el formato observado en copias reales; otra versión del formato podría no leerse.
- MAConta se proporciona tal cual, sin garantía de ningún tipo.

Este repositorio solo contiene las aplicaciones compiladas y su documentación. © Masoft.es. Todos los derechos reservados.
