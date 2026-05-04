# 🧠 IA para la búsqueda de empleo – Cuaderno práctico

> Esto no es teoría. Es un sistema replicable.
> Si haces esto bien, no “buscas trabajo”… entiendes cómo funciona el mercado y juegas mejor.

---

# 1. 🎯 Enfoque

Antes de tocar IA:

* Tener un mínimo de dirección profesional
* Entender que esto va de **reducir incertidumbre en quien contrata**
* Aceptar una realidad incómoda: tu perfil ahora mismo probablemente no está optimizado

La IA no arregla eso.
Lo acelera.

---

# 2. 🧩 Flujo completo del sistema

Este es el sistema que hemos construido:

1. Capturar mercado → Ofertas reales
2. Estructurar datos → Markdown
3. Generar perfil objetivo → NotebookLM
4. Construir tu perfil → archivos .md
5. Comparar → DAFO
6. Detectar gaps → oportunidades
7. Aplicar → CV, LinkedIn, estrategia

---

# 3. ⚙️ Paso a paso

## 🔹 Paso 1 – Capturar ofertas reales

### Objetivo

Entender qué está pidiendo el mercado REAL (no lo que crees tú)

### Qué hacer

1. Buscar 3–5 ofertas que realmente te interesen
2. Guardar sus URLs
3. Pasarlas a una IA (ChatGPT, Gemini, etc.)

---

### 📄 Plantilla base [00_plantilla_oferta.md](02_ofertas_diana/00_plantilla_oferta.md)

Esto es una versión resumida de la propuesta que encontrarás en el repositorio: [00_plantilla_oferta.md](02_ofertas_diana/00_plantilla_oferta.md). Puedes (y debes) mejorarla y adaptarala a tus necesidades y en base a tu experiencia y las ofertas que realmente te interesen:

```markdown
# Oferta

## Empresa

## Puesto

## Descripción

## Responsabilidades

## Requisitos

## Tecnologías

## Nivel requerido

## Soft skills

## Otros detalles relevantes
```

---

### 🤖 Prompt recomendado

Usa el sistema de agente para crearte un asistente que te ayude a extraer y analizar oferatas en base a la plantilla anterior, o directamente utiliza un prompt similar a este (revisa y adapta):

```markdown
Analiza la oferta de empleo en esta url y extrae la información en formato markdown usando esta plantilla:

[PEGAR PLANTILLA] (o adjuntar el archivo md directamente, si el chat te lo permite)

Oferta:
[PEGAR URL]

Condiciones:
- No inventar información
- Sintetizar
- Usar lenguaje claro
- Mantener consistencia entre ofertas
```

---

### Resultado esperado

* 3–5 archivos `.md` estructurados
* Información comparable

---

## 🔹 Paso 2 – Generar perfil objetivo

### Objetivo

Construir el perfil que el mercado está buscando

---

### Cómo hacerlo (NotebookLM + Gemini)

1. Subir los `.md` de ofertas a NotebookLM
2. Usarlos como fuentes
3. Pedirle que genere un perfil consolidado

---

### 🤖 Prompt recomendado

Usa el sistema de agentes para crearte un asistente que te ayude a crear perfiles profesionales objetivo demanadados por la industria en base a las ofertas analizadas. Recuerda que puedes usar cuadernos de NotebookLM como fuentes en una conversación de Gemini, o subir archivos md directamtente en muchos chats.
También puedes utilizar directamente un prompt similar a este (muy recomendamble que lo revises y adaptes):

```markdown
A partir de estas ofertas de empleo, genera un perfil profesional objetivo.

Incluye:
- Resumen profesional
- Skills técnicas clave
- Soft skills más demandadas
- Nivel esperado
- Tecnologías recurrentes
- Responsabilidades típicas

No inventes nada fuera de las fuentes.
Detecta patrones.
```

---

### Resultado

`perfil_objetivo_generado.md`

---

## 🔹 Paso 3 – Construir tu perfil

### Objetivo

Tener tu información estructurada y reutilizable

---

### Estructura (this-is-me)

* Perfil
* Objetivo
* Experiencia
* Proyectos
* Skills
* Formación
* Logros
* Valores
* Preferencias

---

### ⚠️ Error típico

❌ Rellenar con frases genéricas

Ejemplo malo:

> “Me apasiona la tecnología”

Ejemplo bueno:

> “He desarrollado X usando Y y resolviendo Z”

---

### Resultado

Carpeta `this-is-me/` completa

---

## 🔹 Paso 4 – Análisis (DAFO)

### Objetivo

Comparar:

* Perfil objetivo (mercado)
* Tu perfil actual

---

### 🤖 Prompt sugerido
Recuerda que **lo ideal es que crees un agente (GEM o GPT)**, especializado, que puedas ir depurando y mejorando, hasta lograr los resutlados que desees y que realmente te funcionen.

```markdown
Compara estos dos perfiles:

1. Perfil objetivo (mercado)
2. Perfil personal

Genera un análisis DAFO:
- Debilidades
- Amenazas
- Fortalezas
- Oportunidades

Además:
- Identifica gaps concretos
- Propón acciones específicas
```

---

### Resultado

* `dafo.md`
* `gaps_detectados.md`

---

## 🔹 Paso 5 – Aplicación práctica

### Objetivo

Convertir análisis en acción

---

### Ejemplos de uso

Con todo este material, puedes reutilizarlo para mejorar y enriquecer elementos de tu búsqueda de empleo, como por ejemplo:

#### CV

```markdown
Genera ideas para mejorar mi CV en base a:
- Perfil objetivo
- DAFO

Prioriza:
- claridad
- impacto
- adaptación a mercado
```

---

#### LinkedIn

```markdown
Optimiza mi perfil de LinkedIn para este tipo de ofertas.

Incluye:
- titular
- resumen
- enfoque de contenido
```

---

#### Estrategia

```markdown
Sugiere una estrategia de posicionamiento profesional basada en:
- mis fortalezas
- gaps detectados
- demanda del mercado
```

---

# 4. 🛠️ Herramientas utilizadas

## NotebookLM

* Ideal para trabajar con fuentes
* Generación basada en contexto real

## Gemini

* Integración con NotebookLM
* Creación de GEMs

## ChatGPT

* Versátil
* Bueno para iterar prompts

## Otros

* Qwen
* AI Studio

---

# 5. ⚠️ Consejos clave

* No automatices lo que no entiendes
* No copies outputs sin revisar
* No te creas todo lo que genera la IA

La IA no piensa.
Predice.
