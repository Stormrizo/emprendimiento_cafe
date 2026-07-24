# ☕ Proyecto Coffee — Propuesta Técnica y Modelado Físico

Bienvenido al repositorio oficial del **Proyecto Coffee**, un desarrollo técnico e interdisciplinario para el diseño, dimensionamiento e inventario de una barra de café de especialidad basada en métodos de extracción por inmersión y presión.

---

## 📌 Descripción del Proyecto

Este proyecto aborda la preparación de café desde una perspectiva de **física aplicada y termodinámica de fluidos**, modelando fenómenos fisicoquímicos como:

- **Sistemas multifase:** Formación de soluciones acuosas, emulsiones lipídicas y suspensiones coloidales de finos ($d < 100\,\mu\text{m}$).
- **Efecto capilar en medios porosos:** Retención de líquido en la borra de café gobernada por la presión capilar de Young-Laplace ($P_c = \frac{2\gamma \cos\theta}{r}$).
- **Balance de masa y dosificación:** Determinación operacional de la masa de café ($x_c$) corregida por la merma capilar ($k_{\text{ret}} \approx 2.0\text{ mL/g}$):
  $$x_c = \frac{V_{\text{vaso}}}{R - k_{\text{ret}}}$$

---

## 📂 Estructura del Repositorio

- `emprendimiento_cafe.tex` — Archivo principal del documento en LaTeX.
- `colores.tex` — Definición de paletas de colores personalizadas para cajas y diagramas.
- `biblio.bib` — Archivo de bibliografía en formato BibTeX/BibLaTeX.
- `LogoFCFMBUAP (1).png` — Recursos gráficos para el encabezado/pie de página.

---

## 🛠️ Requisitos de Compilación

Para compilar el documento `.tex` localmente necesitas una distribución completa de TeX (como **TeX Live** o **MiKTeX**) con los siguientes motores y paquetes:

- **Motor:** `pdflatex` o `lualatex`
- **Procesador de bibliografía:** `biber`
- **Paquetes clave:** `tikz`, `pgfplots`, `tcolorbox`, `biblatex`, `siunitx`, `geometry`.

### Compilación desde terminal:

```bash
pdflatex emprendimiento_cafe.tex
biber emprendimiento_cafe
pdflatex emprendimiento_cafe.tex
pdflatex emprendimiento_cafe.tex
```
