# Sistema de Gestión de Inventarios

Aplicación web para defensa del Seminario de Título — IACC 2026.
**Felipe Valenzuela Carrasco**

---

## Acceso para profesores

**URL:** https://inventario.hyperfunnel.cl

**Credenciales:**
- Usuario: `demo`
- Contraseña: `demo2026`

**SKUs de prueba** disponibles para escaneo:
- `SKU-2026-04587` (Notebook Lenovo)
- `SKU-2026-04588` (Monitor LG)
- `SKU-2026-04589` (Teclado Logitech)
- `SKU-2026-04590` (Mouse Logitech)
- `SKU-2026-04591` (SSD Samsung)
- `SKU-2026-04624` (Pistola lectora)
- `SKU-2026-04625` (Pistola lectora 2D)

---

## Despliegue en Coolify

1. Subir este repositorio a GitHub.
2. En Coolify: **+ New → Application → Public Repository**.
3. Pegar la URL del repositorio.
4. **Build Pack:** Dockerfile (autodetectado).
5. **Port exposed:** `80`.
6. **Domain:** `inventario.hyperfunnel.cl`.
7. Activar **HTTPS automático**.
8. Click **Deploy**.

Listo. Coolify hace el resto.

---

## Stack técnico

- **Frontend:** HTML5 + CSS3 + JavaScript vanilla (sin dependencias)
- **Servidor:** Nginx Alpine
- **Despliegue:** Docker en VPS Hetzner gestionado por Coolify
- **HTTPS:** Let's Encrypt automático

---

## Funcionalidades

| Módulo | Estado |
|--------|--------|
| Autenticación con sesión | ✓ |
| Recepción de stock con validación SKU | ✓ |
| Transacciones con confirmación ACID | ✓ |
| Historial de movimientos | ✓ |
| Panel de salud de microservicios | ✓ |
| Métricas de latencia en tiempo real | ✓ |
| Diseño responsivo (PWA) | ✓ |

---

## Notas para la comisión

Este sistema es un **prototipo funcional** que demuestra la interfaz de usuario y los flujos operativos descritos en el seminario. La arquitectura completa de microservicios desacoplados, la base de datos PostgreSQL con propiedades ACID, y la integración con sistemas legados mediante API Gateway están documentadas en la presentación y formarían parte de la implementación productiva.
