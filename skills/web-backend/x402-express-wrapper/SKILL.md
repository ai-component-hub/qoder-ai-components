---
name: 'x402-express-wrapper'
description: 'Wrapper oficial de M2MCent (Node.js) para inyectar muros de pago x402'
adopted: 2026-05-16
en APIs o servidores Model Context Protocol (MCP). Usar al construir nuevos servicios
que requieran monetización máquina a máquina
source: antigravity-awesome-skills
tier: 2
---

# x402-express-wrapper

Wrapper oficial de M2MCent (Node.js) para inyectar muros de pago x402 en APIs o servidores Model Context Protocol (MCP). Usar al construir nuevos servicios que requieran monetización máquina a máquina

## When to Use

- Use this skill when working on tasks related to x402 express wrapper
- Trigger when you need expertise in this domain
- Apply best practices from antigravity-awesome-skills

## Workflow

name: x402-express-wrapper
description: Wrapper oficial de M2MCent (Node.js) para inyectar muros de pago x402 en APIs o servidores Model Context Protocol (MCP). Usar al construir nuevos servicios que requieran monetización máquina a máquina.
risk: critical
source: community
tags: [x402, defi, monetization, express, mcp]
# x402-express-wrapper
Esta skill te enseña cómo integrar rápidamente muros de cobro x402 en aplicaciones y servidores Node.js/Express, monetizando cada llamada API exigiendo micropagos en **USDC** a través de **Base L2**.
## When to Use
Usa esta skill cuando el usuario humano (u otro Agente) te solicite:
1. "Agregar una barrera de pago a la API".
2. "Monetizar el servidor MCP que acabamos de crear".
3. "Exigir micropagos en USDC por usar el endpoint".
## 📦 Instalación
En el entorno del usuario, instala directamente desde NPM (o referencia la carpeta local `x402-express` creada en el repositorio `M2MCent` si no está publicado):
```bash
npm install x402-express ethers
```
## 🛠️ Implementación
Solo necesitas importar el wrapper e inyectar el middleware en una ruta de Express:
```javascript

## Source

This skill was adopted from open-source repository: antigravity-awesome-skills
Original path: x402-express-wrapper
