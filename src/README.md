# 🔮 Futuriza - Astrología y Numerología

## Especificación Técnica y Alcance

**Documento:** ESPEC-2026-003  
**Versión:** 0.1  
**Fecha:** Octubre de 2026  
**Preparado por:** Ingeniería Frontend  
**Estado:** Fase de Setup / v0.1

---

## 1. Resumen ejecutivo

**Futuriza** es una plataforma interactiva de astrología y numerología que ofrece cálculos personalizados en tiempo real. La aplicación permite a los usuarios descubrir su signo zodiacal, calcular su número de vida y evaluar la compatibilidad astrológica, todo bajo una arquitectura frontend moderna, tipada y modular.

## 2. Alcance

### Incluido (v1.0)

- Calculadora de signo zodiacal basada en fecha de nacimiento.
- Calculadora de número de vida (numerología) basada en nombre y fecha.
- Módulo de compatibilidad entre dos signos zodiacales.
- Persistencia del perfil del usuario (localStorage).
- UI responsiva, accesible (WCAG AA) y con feedback visual dinámico.

### Excluido (fuera de alcance v1.0)

- Integración con APIs de efemérides astronómicas en tiempo real.
- Sistema de usuarios con backend y autenticación (JWT).
- Pagos o suscripciones premium.

## 3. Requisitos funcionales

| ID    | Requisito                                                       | Prioridad | Estado v0.1  |
| ----- | --------------------------------------------------------------- | --------- | ------------ |
| RF-01 | Renderizar catálogo de 12 signos zodiacales y 9 números de vida | Alta      | ⏳ Pendiente |
| RF-02 | Lógica de cálculo de signo zodiacal por rango de fechas         | Alta      | ⏳ Pendiente |
| RF-03 | Lógica de reducción numerológica a un solo dígito (1-9)         | Alta      | ⏳ Pendiente |
| RF-04 | Algoritmo de compatibilidad con porcentaje y descripción        | Media     | ⏳ Pendiente |
| RF-05 | Persistencia de datos del perfil en `localStorage`              | Media     | ⏳ Pendiente |
| RF-06 | Formateo de fechas y números según localidad (es-CO)            | Baja      | ⏳ Pendiente |

## 4. Requisitos no funcionales

| ID     | Requisito                                                                    |
| ------ | ---------------------------------------------------------------------------- |
| RNF-01 | TypeScript estricto (`strict: true`) como lenguaje principal.                |
| RNF-02 | Arquitectura modular en capas: `type/` → `data/` → `components/` → `utils/`. |
| RNF-03 | Bundler moderno (Vite) con HMR y configuración `bundler`.                    |
| RNF-04 | Cero dependencias de frameworks de UI (Vanilla JS/TS + DOM API).             |
| RNF-05 | Accesibilidad avanzada: `aria-live`, `aria-pressed` y gestión de foco.       |
| RNF-06 | Design tokens (variables CSS) para consistencia visual y modo claro/oscuro.  |

## 5. Stack Tecnológico

> ![TypeScript](https://img.shields.io/badge/TypeScript-7.0+-3178C6?style=flat&logo=typescript)
> ![Vite](https://img.shields.io/badge/Vite-8.0+-646CFF?style=flat&logo=vite)
> ![PNPM](https://img.shields.io/badge/PNPM-F692000?style=flat&logo=pnpm)
> ![HTML5](https://img.shields.io/badge/HTML5-E3aa46?style=flat&logo=html5)
> ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3)
> ![License](https://img.shields.io/badge/license-MIT-green)

---

## Licencia

MIT

## 👨‍💻 Autor

**Julián Lobón** - Desarrollador Frontend  
_"No solo aprendí a codificar. Aprendí a pensar como arquitecto."_
