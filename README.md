# 🚚 HI CAR GPS · Torre de Control Delivery

Demo modular para presentaciones B2B de soluciones de delivery con trazabilidad foto+firma, cobranza con IA y portal para cliente corporativo.

**Demo en vivo:** `https://<TU-USUARIO>.github.io/hicargps-delivery-demo/`

---

## ¿Qué hace?

Webapp standalone (sin backend, sin servidores) que simula la operación completa de una empresa de delivery:

- **Login multi-rol:** Supervisor · Conductor · Cliente · SuperAdmin
- **Captura foto + firma** desde el celular del conductor
- **Acta corporativa** se genera automáticamente
- **Email simulado** al cliente con el acta
- **Dashboard del cliente** con KPIs interactivos + timeline visual por pedido
- **Reporte CxC consolidado** (factura única + IVA + 10% pronto pago + cuentas bancarias)
- **Cobranza con IA** (borrador generado por GPT)

Todo se persiste en `localStorage` del navegador (sin backend).

---

## 🛠 SuperAdmin · Personalizar para tu cliente

Click en **"🛠 SuperAdmin"** arriba a la derecha → edita:

1. **Empresa de delivery** (nombre, tagline, RUC, email, colores corporativos)
2. **Cliente corporativo** del demo (razón social, contacto, email)
3. **Supervisor** (jefe logístico)
4. **Conductores** (lista editable con cédula, placa, vehículo)
5. **Usuario cliente** para el portal
6. **Guías** (precargadas o subir tu CSV)

Al cambiar el nombre del cliente, la empresa o los colores, **todos los documentos** (actas, emails, reporte CxC) reflejan los cambios al instante.

---

## 🎯 Guía de demo (5–10 minutos) para KAM

1. **Login Supervisor** → tablero vacío *(15s)*
2. **Subir Excel / Precargar 9 guías** → aparecen en el funnel *(30s)*
3. **Logout, Login Conductor** (`mgonzalez` / `bemau2026`) → ve su ruta *(30s)*
4. **Iniciar ruta + entregar** con foto + firma *(2 min)*
5. **Ver acta generada** + email simulado al cliente *(30s)*
6. **Login Cliente** (`eduardo` / `bemau2026`) → dashboard + CxP *(1 min)*
7. **Descargar reporte PDF consolidado** *(30s)*
8. **Bot Telegram** `@hicargps_delivery_bot` → consultas IA en vivo *(2 min)*
9. **Cierre** con ROI + propuesta *(1 min)*

---

## Credenciales por defecto (datos demo Bemauexpress)

| Rol | Usuario | Password |
|---|---|---|
| Supervisor | `supervisor` | `bemau2026` |
| Conductor 1 | `dludena` | `bemau2026` |
| Conductor 2 | `dgarcia` | `bemau2026` |
| Conductor 3 | `mgonzalez` | `bemau2026` |
| Cliente | `eduardo` | `bemau2026` |
| SuperAdmin | (botón directo en header) | — |

> Para cambiar credenciales por demo, usa el SuperAdmin.

---

## Stack

- HTML5 + Bootstrap 5 + signature_pad
- localStorage para persistencia
- Generación client-side de actas, reportes CxC y emails (sin backend)
- Compatible con GitHub Pages (estático)

Bot Telegram complementario (live): [@hicargps_delivery_bot](https://t.me/hicargps_delivery_bot)

---

Made by **Agencia Jaguar.EC** · stack **HI CAR GPS**
