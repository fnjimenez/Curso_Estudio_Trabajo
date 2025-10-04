# PLANTILLA EXCEL - CURVAS DE APRENDIZAJE (RESUELTA)

## Instrucciones: Copia estas tablas con los resultados calculados

---

## CASO 1: PRODUCCIÓN DE CELDAS SOLARES

### Datos del problema
```
a (tiempo 1ª unidad):    50
r (tasa):                0.80
b (exponente):           -0.3219
```

### Tabla de resultados
| Unidad | Tiempo (min) |
|--------|--------------|
| 1      | 50.00        |
| 2      | 40.00        |
| 4      | 32.00        |
| 8      | 25.60        |

**Total:** 147.60 min  
**Promedio:** 36.90 min  
**Reducción:** 48.8% (unidad 1 vs 8)

### Fórmulas utilizadas
```
B4: =LN(B3)/LN(2)
B7: =$B$2*A7^$B$4
Total: =SUMA(B7:B10)
Promedio: =PROMEDIO(B7:B10)
```

---

## CASO 2: ENSAMBLE DE DRONES AGRÍCOLAS

### Datos del problema
```
a (tiempo 1ª unidad):    120
r (tasa 85%):            0.85
b (exponente 85%):       -0.2345
r (tasa 80%):            0.80
b (exponente 80%):       -0.3219
```

### Tabla de resultados
| Unidad | Tiempo 85% (min) | Tiempo 80% (min) |
|--------|------------------|------------------|
| 1      | 120.00           | 120.00           |
| 2      | 102.00           | 96.00            |
| 4      | 86.70            | 76.80            |
| 8      | 73.70            | 61.44            |

**Total 85%:** 382.40 min  
**Total 80%:** 354.24 min  
**Diferencia:** 28.16 min (7.4%)

### Interpretación
Una tasa del 80% (aprendizaje más rápido) ahorra casi 30 minutos en las primeras 8 unidades comparado con 85%.

---

## CASO 3: IMPRESIÓN 3D DE PRÓTESIS

### Datos del problema
```
a (tiempo 1ª unidad):    300
r (tasa):                0.90
b (exponente):           -0.1520
```

### Tabla de resultados
| Unidad | Tiempo (min) |
|--------|--------------|
| 1      | 300.00       |
| 2      | 270.00       |
| 3      | 254.85       |
| 4      | 243.00       |
| 6      | 226.52       |

**Total:** 1,294.37 min (21.6 horas)  
**Reducción:** 24.5% (unidad 1 vs 6)

### Interpretación
Tasa del 90% indica aprendizaje lento, típico de procesos complejos como impresión 3D personalizada.

---

## CASO 4: BATERÍAS PARA AUTOS ELÉCTRICOS

### Datos del problema
```
a (tiempo 1ª unidad):    600 min (10 h)
r (tasa):                0.75
b (exponente):           -0.4150
```

### Tabla de resultados
| Unidad | Tiempo (min) | Tiempo (h) |
|--------|--------------|------------|
| 1      | 600.00       | 10.00      |
| 2      | 450.00       | 7.50       |
| 4      | 337.50       | 5.63       |
| 8      | 253.13       | 4.22       |
| 16     | 189.84       | 3.16       |

**Total:** 1,830.47 min = 30.51 horas  
**Promedio:** 6.10 horas por batería  
**Ahorro (1 vs 16):** 6.84 horas  
**Ahorro económico ($500/h):** $3,418

### Interpretación
Tasa del 75% (aprendizaje rápido) es típica de procesos aeronáuticos y alta tecnología. El ahorro económico es muy significativo.

---

## CASO 5: DESARROLLO DE SOFTWARE CON IA

### Datos del problema
```
a (tiempo 1ª unidad):    40 h
r (tasa):                0.85
b (exponente):           -0.2345
```

### Tabla de resultados
| Implementación | Tiempo (h) |
|----------------|------------|
| 1              | 40.00      |
| 2              | 34.00      |
| 4              | 28.90      |
| 8              | 24.57      |

**Total:** 127.47 horas  
**Promedio:** 31.87 horas por módulo  
**Reducción:** 38.6% (módulo 1 vs 8)

### Comparación con tasa 80%
Si la tasa fuera 80% en lugar de 85%:
- Implementación 8: 20.48 h (vs 24.57 h)
- Ahorro: 4.09 horas por implementación

---

## ANÁLISIS COMPARATIVO DE LOS 5 CASOS

| Caso | T1 | Tasa | Exponente b | Reducción % |
|------|-----|------|-------------|-------------|
| Celdas Solares | 50 min | 80% | -0.3219 | 48.8% |
| Drones | 120 min | 85% | -0.2345 | 38.6% |
| Prótesis 3D | 300 min | 90% | -0.1520 | 24.5% |
| Baterías EV | 600 min | 75% | -0.4150 | 68.4% |
| Software IA | 40 h | 85% | -0.2345 | 38.6% |

### Conclusiones

1. **Tasas más bajas = Aprendizaje más rápido**
   - Tasa 75% (Baterías): Reducción del 68.4%
   - Tasa 90% (Prótesis): Reducción del 24.5%

2. **Exponente b siempre negativo**
   - Más negativo = curva más pronunciada = mayor ahorro

3. **Aplicaciones prácticas**
   - Planeación: Proyectar tiempos futuros
   - Costos: Calcular mano de obra total
   - Capacitación: Medir efectividad
   - Estrategia: Decidir cuándo tercerizar vs. producir

---

## GRÁFICAS RECOMENDADAS

### Para cada caso, crear:

**Gráfica 1: Curva básica**
- Eje X: Unidad
- Eje Y: Tiempo
- Tipo: Dispersión con líneas suaves
- Mostrar la reducción progresiva

**Gráfica 2: Comparación de tasas** (Caso 2)
- Comparar 80% vs 85%
- Mostrar el impacto visual de la diferencia

**Gráfica 3: Ahorro económico** (Caso 4)
- Visualizar ahorro en dinero
- Gráfico de barras: Costo unidad 1 vs unidad 16

---

## VERIFICACIÓN DE RESULTADOS

### Método rápido de verificación:

**Regla de duplicación:**
Si la unidad se duplica, el tiempo debe multiplicarse por la tasa.

Ejemplo Caso 1 (tasa 80%):
- Unidad 1: 50 min
- Unidad 2: 50 × 0.80 = 40 min ✓
- Unidad 4: 40 × 0.80 = 32 min ✓
- Unidad 8: 32 × 0.80 = 25.6 min ✓

**Si tus resultados no coinciden:**
1. Verifica que b = ln(tasa)/ln(2)
2. Revisa referencias absolutas ($B$2, $B$4)
3. Confirma que la tasa sea decimal (0.80, no 80)

---

**Nota para el docente:** Estos son los resultados esperados. Usa esta plantilla para verificar rápidamente el trabajo de los estudiantes durante la clase.