# Predicción de Eficacia del Candidato Vacunal Quimi-Vio® 11 en Adultos

Trabajo de diploma en opción al título de **Licenciada en Ciencia de Datos**, Facultad de Matemática y Computación, Universidad de La Habana, 2026.

Desarrollado en colaboración con el **Instituto Finlay de Vacunas**.

---

## Resumen

La enfermedad neumocócica, causada por *Streptococcus pneumoniae*, es una causa importante de mortalidad global. Tras la implementación de la vacuna heptavalente Quimi-Vio® 7 en niños en Cuba, se desarrolló el candidato vacunal **Quimi-Vio® 11** para adultos de 50 a 74 años.

Este trabajo predice la eficacia de Quimi-Vio® 11 mediante un **estudio de inmunopuente**, extrapolando la protección a partir de la eficacia observada de Quimi-Vio® 7. Se analizó la actividad opsonofagocítica (OPA) de 87 niños y 65 adultos un mes después de la vacunación, calculándose las Medias Geométricas de los Títulos (GMT) y su Razón (GMR) para nueve serotipos comunes.

Para el manejo de valores por debajo del límite de cuantificación (LLOQ) se compararon el **método de sustitución simple** y el **modelo de regresión Tobit (MLE)**. La no inferioridad del grupo adulto respecto al pediátrico se estableció cuando el límite inferior del IC 95% del GMR fue superior a 0,5.

Los resultados demostraron no inferioridad en **7 de los 9 serotipos** (1, 5, 6A, 19A, 6B, 18C y 19F). El método MLE redujo el sesgo y proporcionó intervalos más robustos ante la censura.

---

## 🗂️ Estructura del repositorio

```
Thesis/
├── document/
│   ├── FrontMatter/       # Portada, resumen, dedicatoria, agradecimientos
│   ├── MainMatter/        # Introducción, antecedentes, propuesta, implementación
│   ├── BackMatter/        # Conclusiones, recomendaciones, bibliografía, anexos
│   └── Graphics/          # Figuras e imágenes
├── Thesis.tex             # Documento principal
├── Thesis.pdf             # Documento final compilado
├── Bibliography.bib       # Referencias bibliográficas
├── uhthesis.cls           # Clase LaTeX de la UH
```

---

## Compilación

Con `pdflatex` + `bibtex`:

```bash
pdflatex Thesis.tex
bibtex Thesis
pdflatex Thesis.tex
pdflatex Thesis.tex
```

---

## Implementación

Para má detalles ver el repositorio de implementación:
[Pneumococcal-Immunobridging](https://github.com/mariandc18/Pneumococcal-Immunobridging)

## 👩‍💻 Autora
Marian Aguilar Tavier

## Tutora
- MsC. Yanet García Serrano

## Asesora
- DraC. Dagmar García Rivera