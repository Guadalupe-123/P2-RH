# P2 RH (Excel, sin macros)

Proyecto realizado exclusivamente en **Excel** para estimar y explicar el **riesgo de fuga de talento** (People Analytics). Se trabaja con tablas, fórmulas y tablas dinámicas. **No utiliza macros**; el archivo conserva extensión `.xlsm` por compatibilidad.

## Estructura del archivo

- **raw**: datos originales (fuente en bruto). No editar fórmulas ni formatos.
- **datos**: datos limpios/normalizados a partir de *raw* (tipos corregidos, columnas derivadas).
- **analisis**: métricas y cálculos intermedios (segmentación por riesgo, comparativos por área/antigüedad, etc.).
- **dashboard**: indicadores y visualizaciones finales para lectura ejecutiva (distribución de riesgo y KPIs principales).

## Uso
1. Abrir `P2 RH.xlsm` *(no es necesario habilitar macros)*.
2. Actualizar/pegar nuevos registros en **raw** siguiendo el mismo esquema de columnas.
3. Revisar **datos** (validaciones) y **analisis** (cálculos y segmentaciones).
4. Si usas tablas dinámicas o conexiones: **Datos → Actualizar todo**.
5. Consultar el tablero en **dashboard** y el documento `Reporte_RH_Riesgo.docx`.

## KPIs (referenciales)
- **Riesgo total** y distribución **Bajo/Medio/Alto**.
- **Edad promedio** por segmento.
- **Ingreso promedio** por segmento.
- **Satisfacción** promedio y % con valores críticos (p. ej., ≤2).
- **Años desde última promoción** (puntos de corte).
- **Horas extra** promedio y su relación con el riesgo.

## KPIs (resumen)

- **Riesgo total de fuga**: __%  · **Distribución**: Bajo __% · Medio __% · Alto __%
- **Edad promedio (años)**: Estables __ · Riesgo Medio __ · Riesgo Alto __
- **Ingreso promedio**: Estables $__ · Riesgo Medio $__ · Riesgo Alto $__
- **Satisfacción**: promedio __/5 · % con ≤2: __%
- **Sin promoción (años)**: mediana __ · p90 __
- **Horas extra**: promedio __ h/sem · % con >10 h/sem: __%
- **Top 3 áreas con mayor riesgo**: 1) __  2) __  3) __
- **Antigüedad**: distribución 0–1: __% · 1–3: __% · 3–5: __% · 5+: __%


## Notas
- El repositorio ignora temporales de Office (`~$*`) y archivos de sistema.
- Si contiene datos reales/sensibles, mantener el repositorio **Privado**.
- Puedes renombrar el archivo a `.xlsx` si confirmas que no hay macros.

## Vistas
![Dashboard RH](docs/Dashboard%20RH.jpg)


📂 **Archivo principal:** [P2 RH.xlsm](./P2%20RH.xlsm)  
📄 **Informe ejecutivo:** [Reporte_RH_Riesgo.docx](./Reporte_RH_Riesgo.docx)
