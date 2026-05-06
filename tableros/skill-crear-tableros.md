---
name: crear-tableros
description: Crea tableros interactivos premium en HTML para analizar y visualizar datos de redes sociales, negocios, ventas, contenido y métricas ejecutivas.
---
## Crear tableros
Usar SIEMPRE que el usuario mencione: tablero, dashboard, visualizar métricas, analizar datos, KPIs, reporte visual, panel de control, métricas de negocio, estadísticas de redes sociales, datos de ventas, rendimiento de campañas, o cualquier solicitud de transformar datos en algo visual e interactivo. También activar cuando el usuario suba un CSV, XLSX, JSON o imagen con datos y quiera verlos de forma visual, aunque no diga explícitamente "tablero".

### Objetivo

Transformar datos en tableros interactivos premium: claros, compartibles y accionables.

### Lógica de acción directa

- Si el usuario ya proveyó datos + propósito claro → genera el tablero de inmediato.  
- Si faltan datos críticos (fuente o propósito), haz una sola pregunta concisa.  
- Si falta algo no crítico (audiencia, estilo), usa defaults y genera.  
- No hagas más de 2 preguntas antes de generar.

### Fuentes admitidas

- CSV, XLSX, JSON, PDF, TXT, MD  
- URL pública  
- Texto pegado  
- Imagen con datos (PNG/JPG/WEBP)

### Tipos de tablero y prioridades

**Tipo**  
**Métricas prioritarias**

- **Redes sociales**  
  Crecimiento, engagement, alcance, rendimiento de contenido  

- **Negocio / ventas**  
  Conversiones, ROI, revenue, embudo, desempeño por canal  

- **Ejecutivo**  
  Lectura breve, clara, orientada a decisiones  

- **Contenido**  
  Rendimiento por formato, canal, frecuencia y hora  

- **Personalizado**  
  Según lo que defina el usuario  

### Stack técnico

- Entregar siempre un archivo HTML único autocontenido (sin dependencias locales).  
- Vanilla JavaScript — nunca React ni frameworks que requieran compilación.  
- Gráficos: Chart.js 4.x desde CDN (cdn.jsdelivr.net).  
- Íconos opcionales: Lucide o Font Awesome desde CDN.  
- CSS embebido en `<style>` dentro del mismo archivo.  
- Sin llamadas a APIs externas ni `fetch` a recursos que requieran autenticación.  

### Default visual — Glassmorphism Premium

- Fondo oscuro con capas de vidrio translúcido y blur.  
- Tarjetas con `backdrop-filter`, bordes sutiles y sombras con profundidad.  
- Animaciones de entrada suaves (`fadeInUp`, `scaleIn`).  
- Microinteracciones en hover: glow, elevación, transiciones de color.  
- Tipografía limpia con jerarquía clara (título > subtítulo > dato > etiqueta).  
- Paleta: oscuros (`#0a0a1a`, `#111827`) + acentos (`#6366f1`, `#8b5cf6`, `#06b6d4`).  
- Gráficos con Chart.js: líneas, barras, donuts, gauges según contexto.  
- Mobile-first: columna única en móvil, grid en desktop.

### Principios de diseño

- Claridad primero — menos elementos, más impacto.  
- Mobile-first — layouts apilables que funcionan en pantalla chica.  
- Alta densidad controlada — tooltips y acordeones para no saturar.  
- Accesibilidad — contraste ≥4.5:1, legible para daltónicos.  
- Jerarquía visual — el ojo sigue: arriba‑abajo, izquierda‑derecha.

### Estructura de salida

- **Título del tablero** — nombre descriptivo y directo.  
- **Resumen ejecutivo** — 2–3 líneas con el hallazgo más importante.  
- **Tablero HTML interactivo** — responsive, con filtros y navegación.  
- **Hallazgos clave** — bullets concisos y accionables.  
- **Análisis valorativo** — solo si aporta; omitir si los datos hablan solos.

### Reglas absolutas

- No inventar datos; si la fuente es ambigua, indicarlo en el tablero.  
- No sobreexplicar el proceso ni agregar secciones innecesarias.  
- Si hay suficiente contexto, generar directo sin preguntar.
