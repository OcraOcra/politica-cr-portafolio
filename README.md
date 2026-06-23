# Cultura Política en Costa Rica — Proyecto en R

**Autor:** Marco Artavia Pacheco  
**Fuente principal:** LAPOP AmericasBarometer Costa Rica 2016 (vía PEN)  
**Tema:** Confianza institucional y cultura democrática en Costa Rica

## Estructura del proyecto

```
politica-cr-portafolio/
├── README.md
├── .gitignore
├── scripts/
│   └── 01-install-packages.R
├── datos/
│   └── raw/
│       ├── costarica_lapop_2016.csv   # LAPOP 2016 (1514 obs, 198 vars)
│       └── indicadores_regionales_anuales.xlsx  # PEN
├── output/
│   └── analisis.html       # reporte HTML (knitted)
└── analisis.Rmd            # R Markdown principal
```

## Datasets usados

1. **LAPOP AmericasBarometer Costa Rica 2016** — Encuesta de opinión pública sobre democracia y gobernanza (PEN)
2. **Indicadores Regionales Anuales** — Indicadores socioeconómicos por región (PEN)

## Hallazgos principales

- Partidos políticos tienen la **menor confianza** (3.0/7)
- Gobierno gozaba de **alta confianza** en 2016 (5.2/7), con 49% en niveles 6-7
- **Sin brecha urbano-rural** significativa (5.1 vs 5.2)
- Educación muestra relación **no lineal** con confianza en el gobierno (U-shaped)
- Confianza en partidos **decrece con educación** (3.2 primaria → 2.9 universitaria)

## Cómo reproducir

1. Clonar el repo
2. Abrir `analisis.Rmd` en RStudio
3. Instalar paquetes con `scripts/01-install-packages.R`
4. Darle "Knit to HTML"
