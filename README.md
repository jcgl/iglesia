# Iglesia Católica Siempre con Dios

Contenido católico diario para la página de Facebook **"Iglesia Católica Siempre con Dios"**.

Cada día se generan **10 frases católicas** listas para publicar en redes sociales, en español, fieles al Magisterio de la Iglesia. Mezclan cuatro tipos:

- **Reflexiones** breves sobre la fe y la vida cristiana.
- **Evangelios / pasajes bíblicos**, cada uno con su cita exacta (p. ej. `(Mt 11,28)`).
- **Oraciones** cortas.
- **Mensajes de esperanza** y aliento.

## Estructura

```
frases/
  AAAA-MM-DD.md   # 10 frases numeradas del día, con tipo entre corchetes
```

Cada archivo empieza con el encabezado `# Frases catolicas - AAAA-MM-DD` y lista las 10 frases. Ejemplo:

```
1. [Evangelio] «Vengan a mí todos los que están fatigados y agobiados, y yo los aliviaré.» (Mt 11,28)
2. [Reflexión] ...
```

## Generación automática

Las frases las crea una **rutina de Claude Code en la nube** (cloud agent) que corre todos los días a las **7:00 AM (America/Mexico_City)**. La rutina:

1. Obtiene la fecha de hoy.
2. Escribe `frases/AAAA-MM-DD.md` con las 10 frases.
3. Hace commit y push a la rama `main`.

Gestión de la rutina: https://claude.ai/code/routines

## Uso

Toma el archivo del día en `frases/` y publica las frases en la página de Facebook.
