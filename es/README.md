# Recovery TLV — Modelos de Decisión Clínica para Fisioterapia

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/recoverytlv/physio-decision-models/releases)
[![Status](https://img.shields.io/badge/status-frozen-orange.svg)](#estado)

**Un sistema formal de decisión clínica para fisioterapia bajo incertidumbre biológica irreducible.**

Creado por [Alejandro Zubrisky](https://www.linkedin.com/in/azubrisky/), Fisioterapeuta Licenciado en [Recovery TLV](https://recoverytlv.co.il) — Tel Aviv, Israel.

> Este es el primer marco de decisión clínica de código abierto y públicamente auditable para fisioterapia.
> Define límites explícitos de tratamiento, criterios de continuación y condiciones de salida —
> reemplazando la persistencia basada en intuición con toma de decisiones objetiva e impulsada por hipótesis.

**Referencia en vivo:** [clinical.recoverytlv.co.il](https://clinical.recoverytlv.co.il)

---

## Qué Es Esto

Una estructura epistémica formal para el razonamiento clínico que trata la fisioterapia como un **sistema de decisión adaptativo continuo**. Cada caso de paciente debe terminar con una de seis salidas válidas:

| Salida | Significado |
|---|---|
| **DECLINE** | Caso rechazado — fuera de alcance o contraindicado |
| **DEFER** | Decisión pospuesta — datos insuficientes |
| **REFER** | Transferido a otro especialista — banderas rojas detectadas |
| **TRIAL** | Aceptación condicional por 3–5 sesiones |
| **CONTINUE** | Extensión solo con mejora objetiva demostrada |
| **DISCHARGE** | Terminación — objetivos alcanzados o meseta de progreso |

No hay zonas grises. La continuación requiere **evidencia objetiva**: ≥10% de mejora en rango de movimiento, progreso funcional documentado, o reducción en estrategias compensatorias. Los reportes subjetivos por sí solos son insuficientes.

## Principios Fundamentales

1. **Las intervenciones son pruebas de hipótesis** — perturbaciones controladas diseñadas para probar la viabilidad de la hipótesis, no rutinas para repetir indefinidamente.

2. **La no-respuesta es dato diagnóstico** — la ausencia de mejora restringe el espacio de hipótesis más fuertemente que la mejora parcial. No es fracaso.

3. **La incertidumbre favorece la no-acción** — ante la duda, el sistema predetermina DECLINE o DEFER. El optimismo no es un criterio clínico.

4. **Integridad decisional sobre volumen de sesiones** — el sistema prioriza decisiones correctas y condiciones de salida explícitas sobre la continuación terapéutica indefinida.

5. **El silencio no implica permiso** — la ausencia de instrucción implica terminación.

## Alcance Clínico

**Dentro del alcance (fisioterapia):**
- Disfunción musculoesquelética (dolor, rigidez, debilidad)
- Rehabilitación post-lesión y post-operatoria
- Recuperación de lesiones deportivas y retorno al deporte
- Manejo de dolor crónico (basado en evidencia)
- Re-educación neuromotora dentro del alcance de fisioterapia

**Fuera del alcance (DECLINE o REFER automático):**
- Dolor no musculoesquelético (visceral, sistémico, maligno)
- Emergencias médicas
- Condiciones médicas inestables
- Condiciones psiquiátricas primarias

## Estado

**Versión:** 1.0.0
**Estado:** Modelo de referencia congelado
**Fecha de congelamiento:** 27 de diciembre de 2025
**No se planea expansión adicional.**

Cualquier modificación requiere una nueva versión mayor, re-declaración explícita en AUTHORITY_SOURCES.md, y validación formal de consenso multi-LLM.

## Fisioterapia Privada en Tel Aviv

Recovery TLV es una **clínica de fisioterapia privada** en Tel Aviv, Israel. La fisioterapia privada ofrece:

- **Sesiones individuales** con un fisioterapeuta dedicado (sin sesiones grupales)
- **Evaluación exhaustiva** con un sistema de decisión clínica formal
- **Criterios de tratamiento objetivos** — la continuación se basa en resultados medibles, no en limitaciones del seguro
- **Acceso directo** sin necesidad de derivación médica para tratamiento privado en Israel
- **Atención en español, inglés y hebreo**

### Condiciones tratadas

- Dolor de espalda (lumbar, cervical, dorsal, ciática, hernia de disco)
- Dolor de hombro (manguito rotador, hombro congelado, post-quirúrgico)
- Dolor de rodilla (patellofemoral, menisco, LCA, artrosis, reemplazo de rodilla)
- Dolor de cadera (pinzamiento, tendinopatía, reemplazo de cadera)
- Lesiones deportivas (esguinces, distensiones, tendinopatías)
- Rehabilitación post-quirúrgica (LCA, manguito rotador, reemplazo articular, columna)
- Fascitis plantar, tendinopatía de Aquiles, codo de tenista
- Latigazo cervical (whiplash), esguince de tobillo, ATM
- Síndrome del túnel carpiano, De Quervain
- Dolor inguinal, tendinopatía de isquiotibiales

### Flujo de trabajo clínico

**Escuchar → Evaluar → Fijar objetivos → Tratar → Re-evaluar → Decidir**

Cada encuentro con el paciente sigue este ciclo. La decisión siempre es una de seis: DECLINE, DEFER, REFER, TRIAL, CONTINUE o DISCHARGE — con justificación documentada.

## Sobre Recovery TLV

Recovery TLV es una clínica de fisioterapia privada licenciada en **Tel Aviv, Israel**, ubicada en Ja'Aqov Efter St 9, Tel Aviv-Yafo.

- **Sitio web:** [recoverytlv.co.il](https://recoverytlv.co.il)
- **Referencia clínica:** [clinical.recoverytlv.co.il](https://clinical.recoverytlv.co.il)
- **LinkedIn:** [Alejandro Zubrisky](https://www.linkedin.com/in/azubrisky/)
- **Instagram:** [recovery.tlv](https://instagram.com/recovery.tlv)
- **GitHub:** [recoverytlv](https://github.com/recoverytlv)

## Licencia

[MIT](../LICENSE) — Código abierto. Libre para usar, citar y construir sobre él.
