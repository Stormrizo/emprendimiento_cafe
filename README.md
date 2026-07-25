# ☕ Proyecto Coffee — propuesta técnica y modelado físico

Bienvenido al repositorio oficial del **Proyecto Coffee**, un desarrollo técnico e interdisciplinario para el diseño, dimensionamiento e inventario de una barra de café de especialidad basada en métodos de extracción por inmersión y presión.

---

## 📌 Descripción del proyecto

Este proyecto aborda la preparación de café desde una perspectiva de **física aplicada y termodinámica de fluidos**, modelando fenómenos fisicoquímicos como:

- **Sistemas multifase:** formación de soluciones acuosas, emulsiones lipídicas y suspensiones coloidales de finos ($d < 100\ \mathrm{\mu m}$).
- **Efecto capilar en medios porosos:** retención de líquido en la borra de café gobernada por la presión capilar de Young-Laplace ($P_c = \frac{2\gamma \cos\theta}{r}$).
- **Balance de masa y dosificación:** determinación operacional de la masa de café ($x_c$) corregida por la merma capilar ($k_{\mathrm{ret}} \approx 2.0\ \mathrm{mL/g}$):

$$
x_c = \frac{V_{\mathrm{vaso}}}{R - k_{\mathrm{ret}}}
$$

---

## 📂 Estructura del repositorio

- `emprendimiento_cafe.tex` — archivo principal del documento en LaTeX.
- `colores.tex` — definición de paletas de colores personalizadas para cajas y diagramas.
- `biblio.bib` — archivo de bibliografía en formato BibTeX/BibLaTeX.
- `LogoFCFMBUAP (1).png` — recursos gráficos para el encabezado y pie de página.

---

## 🛠️ Requisitos de compilación

Para compilar el documento `.tex` localmente necesitas una distribución completa de TeX (como **TeX Live** o **MiKTeX**) con los siguientes motores y paquetes:

- **Motor:** `pdflatex` o `lualatex`
- **Procesador de bibliografía:** `biber`
- **Paquetes clave:** `tikz`, `pgfplots`, `tcolorbox`, `biblatex`, `siunitx`, `geometry`.
