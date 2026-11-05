# Profe Nodo: ruta de 14 días para la Fase 1 de la OSIA

Plataforma de práctica, en una sola página web, para preparar la **Fase 1 (primera ronda en línea)** de la [Olimpiada Salvadoreña de Inteligencia Artificial](https://osia.com.sv/). El contenido sigue el temario público de [osia.com.sv/preparacion](https://osia.com.sv/preparacion/).

> Las lecciones y preguntas son material de práctica hecho a partir del temario público. **No son preguntas oficiales** y el formato del examen real puede ser distinto. La OSIA publica el alcance y los recursos permitidos antes de cada ronda.

## Qué incluye

- **Ruta de 14 días** con lección, actividades prácticas y quiz por día. El progreso se guarda en el navegador (`localStorage`).
- **Actividades interactivas**: tablas de verdad, filtro de spam con reglas, diagrama de flujo, explorador de grafos, revisión de un dataset, clasificador por vecinos (k-NN), k-medias paso a paso, detector de lobos sesgado, predicción de la siguiente palabra y laboratorio de prompts.
- **Simulacros con tiempo** y resultados por tema.
- **Glosario** con buscador.
- **Tutor con Gemini**: la página arma la consulta, la copia al portapapeles y abre Gemini en otra pestaña. No usa ninguna API ni clave: el estudiante conversa en Gemini con su propia cuenta de Google.

## Publicar con GitHub Pages

```bash
git clone https://github.com/mjlopeez/profe-nodo.git
cd profe-nodo
# copiá aquí index.html, README.md, GEM-INSTRUCCIONES.md y .nojekyll
git add .
git commit -m "Primera versión de Profe Nodo"
git push origin main
```

Luego, en GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: `main` / `(root)` → Save**. En uno o dos minutos queda en `https://mjlopeez.github.io/profe-nodo/`.

## Configurar el Gem (opcional)

Ver [GEM-INSTRUCCIONES.md](GEM-INSTRUCCIONES.md). Si creás y compartís un Gem “Profe Nodo”, pegá su enlace en `const GEM_URL = "";` dentro de `index.html`.

## Por qué no se conecta directamente a la API de Gemini

Los términos de la API de Gemini exigen tener 18 años o más y prohíben usarla en sitios dirigidos a menores de 18 o que probablemente usen menores, además de limitarla a uso profesional o de negocio ([Gemini API Additional Terms](https://ai.google.dev/terms)). Por eso el tutor usa la aplicación de Gemini, donde el estudiante entra con su propia cuenta.

## Privacidad

- No hay servidor ni base de datos: todo queda en el navegador del estudiante.
- Borrar los datos del sitio en el navegador reinicia el progreso.
- Recomendación para el estudiante: no compartir datos personales en Gemini.

## Fuentes

- Temario: https://osia.com.sv/preparacion/
- Calendario y modalidad: https://osia.com.sv/convocatoria
