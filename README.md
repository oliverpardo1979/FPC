# Finanzas Públicas Colombianas

Presentación integrada del curso de Finanzas Públicas Colombianas. El archivo maestro fusiona cuatro conjuntos de láminas: `FCP_Intro`, `FCP_GG`, `FCP_Ciclo` y `FiscalBookPresentation`.

## Entregables

- `main.tex`: archivo maestro Beamer.
- `modules/`: módulos extraídos de los tres primeros conjuntos.
- `slides/`: láminas de `FiscalBookPresentation`, incluidas las que estaban comentadas o ubicadas después del cierre original.
- `graficas/` y `assets/`: recursos gráficos.
- `output/pdf/Finanzas_Publicas_Colombianas_2026.pdf`: presentación compilada, 193 páginas.

## Actualización de cifras

Las series con información disponible se actualizaron con los libros del MFMP 2026 suministrados en la carpeta local `Data`. Las referencias principales son:

- Capítulo 1: tablas 1.2, 1.3 y 1.4; gráficos 1.5, 1.7 y 1.9.
- Capítulo 3: tabla 3.1 y gráfico 3.10.
- Apéndice 2: tabla A.2.1.

El MFMP 2026 no publica cortes 2025 comparables para reservas presupuestales, composición de tenedores de TES, balance ajustado por causación del FEPC ni gasto tributario por actividad económica. En esos casos se conserva el último dato verificable y la limitación aparece en la lámina correspondiente.

## Compilación

La presentación usa LaTeX Beamer y puede compilarse con Tectonic:

```powershell
tectonic --keep-logs --outdir output/pdf main.tex
```