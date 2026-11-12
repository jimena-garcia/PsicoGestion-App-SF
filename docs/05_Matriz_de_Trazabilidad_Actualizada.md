# Actualización de la Matriz de Trazabilidad

## Control de documentación

### Control de configuración

| Campo | Valor |
| --- | --- |
| Título | Actualización de la Matriz de Trazabilidad |
| Proyecto | PsicoGestión |
| Cliente | Servicio Externo de Apoyo Psicológico (SEAP), Facultad de Psicología, Universidad Autónoma de Yucatán (UADY) |
| Representante del cliente | Psic. José de Jesús León Pérez |
| Referencia | PG-CRN-001 EDT 2.2 (matriz de trazabilidad requerimiento–prueba); Planeacion_Iteracion1 a 3; PlanPruebas_Iteracion1 a 3; ActaAceptacion_Iteracion1 a 3; docs/MATRIZ-TRAZABILIDAD.md |
| Autoras | Mariana Caballero Beltrán<br>Jimena Guadalupe García Ríos<br>Jaqueline Góngora Tun<br>Luisa Cristina Villanueva Díaz |
| Elabora | Equipo de Desarrollo (Mariana Caballero Beltrán, Jimena Guadalupe García Ríos) |
| Consolida | Líder de Proyecto (Jaqueline Góngora Tun) |
| Recibe / autoriza | Administradora de Proyecto (Luisa Cristina Villanueva Díaz) |
| Rol de elaboración | Project Manager Senior / QA |
| Fecha de emisión | 10 de noviembre de 2026 |
| Versión | 0.1.0 |
| Estado | B (Borrador) |
| Código de referencia ACS | [PENDIENTE: código PG-xxx-nnn asignado por el Encargado SQA/ACS] |

### Histórico de versiones

| Versión | Fecha | Estado | Responsable | Nombre de archivo |
| --- | --- | --- | --- | --- |
| 0.1.0 | 10/Nov/2026 | B | Jaqueline Góngora Tun (consolidación) | 05_Matriz_de_Trazabilidad_Actualizada.md |

Estado: (B)orrador, (R)evisión, (A)probado.

### Histórico de cambios

| Versión | Fecha | Cambios |
| --- | --- | --- |
| 0.1.0 | 10/Nov/2026 | Primera versión borrador. Mapeo RF/RNF → criterio de aceptación → caso de prueba de las Iteraciones 1 a 3, brechas de cobertura y evidencia de la Iteración 4. |

### Convenciones de este documento

| Convención | Significado |
| --- | --- |
| `[PENDIENTE: dato]` | Dato no disponible en el paquete de documentación ni en el repositorio entregado; requiere captura o confirmación. |
| Fuente | Archivo del paquete `documentacion_psicogestion.zip` o del repositorio `PsicoGestion-main.zip` del que proviene el dato. |
| Horas reales | Ninguno de los archivos entregados contiene registro de horas efectivamente trabajadas; todo valor real de esfuerzo se declara `[PENDIENTE]`. |
| Horas planificadas (derivadas) | Calculadas a partir de PG-PPR-001 §4 (asignación de recursos) con el modelo de 6 h por persona por día hábil asignado, sin doble conteo de tareas simultáneas de una misma persona. |
| Semanas | Semana 1 = 21/09/2026 (convención de `Reportes_de_Estado.xlsx`). Semana 5 = 19–23/10; semana 6 = 26–30/10; semana 7 = 02–06/11 (02/11 inhábil); semana 8 = 09–13/11. |


## 1. Método y alcance

| Elemento | Descripción |
| --- | --- |
| Objetivo | Garantizar que cada requerimiento funcional (RF) y no funcional (RNF) referenciado tenga criterio de aceptación (CA), caso de prueba (CP) y resultado verificable. |
| Universo | Los 147 requerimientos individuales referenciados en las planeaciones y planes de prueba de las Iteraciones 1 a 3 (109 RF y 38 RNF), con los rangos expandidos (p. ej. "RF 1.1.1-1.1.18" equivale a 18 RF). |
| Fuente de CA | `Planeacion_Iteracion1.docx`, `Planeacion_Iteracion2.docx`, `Planeacion_Iteracion3.docx` (CA-01 a CA-78). |
| Fuente de CP | `PlanPruebas_Iteracion1.xlsx` (CP-INT-01 a 29), `PlanPruebas_Iteracion2.xlsx` (CP2-INT-01 a 32), `PlanPruebas_Iteracion3.xlsx` (CP3-INT-01 a 54): 115 casos. |
| Fuente de resultado | Resultado de CA en `ActaAceptacion_IteracionN.docx`; estado de CP en la columna "Estado" del plan de pruebas. |
| Regla de vínculo CA–CP | Un CP se vincula a un CA cuando comparten al menos un RF o RNF dentro de la misma iteración. Los CP que cubren seis o más requerimientos (flujo completo) se muestran en columna aparte. |
| Documento fuente de RF | El ERS no forma parte del paquete entregado; los textos de RF no se transcriben. [PENDIENTE: ERS aprobado para validar la numeración RF 1.x a 5.x y definir RF 6.x] |
| Matriz anterior | `docs/MATRIZ-TRAZABILIDAD.md` del repositorio (12 filas de calidad y seguridad), integrada en la sección 8. |

## 2. Resumen de cobertura

| Indicador | Valor |
| --- | --- |
| Requerimientos referenciados | 147 (109 RF, 38 RNF) |
| Con CA y CP | 121 |
| Con CA y sin CP | 15 (todos RNF de las Iteraciones 1 y 2) |
| Con CP y sin CA explícito | 11 |
| Criterios de aceptación | 78 (CA-01 a CA-78); 78/78 con resultado "Sí" en actas |
| Casos de prueba | 115; 115 "Pasa"; 0 con observación registrada |
| CA sin CP directo ni de flujo completo | 13 (sección 6.3) |
| Requerimientos de la Iteración 4 | [PENDIENTE: RF 6.x, CA-79 en adelante y CP de la Iteración 4] |

### 2.1 Cobertura por iteración y módulo

| Iteración | Módulo | CA | CP | Resultado actas | Resultado pruebas |
| --- | --- | --- | --- | --- | --- |
| 1 | Registro de usuarios | CA-01 a 09 | CP-INT-01 a 10, 29 (parcial) | 9/9 Sí | Pasa |
| 1 | Inicio de sesión | CA-10 a 13 | CP-INT-11 a 20 | 4/4 Sí | Pasa |
| 1 | Cierre de sesión | CA-14 a 17 | CP-INT-21 a 23 | 4/4 Sí | Pasa |
| 1 | Recuperación de cuenta | CA-18 a 22 | CP-INT-24 a 29 | 5/5 Sí | Pasa |
| 2 | Registro de terapeutas | CA-23 a 31 | CP2-INT-01 a 09 | 9/9 Sí | Pasa |
| 2 | Visualización y actualización de terapeutas | CA-32 a 36 | CP2-INT-10 a 15 | 5/5 Sí | Pasa |
| 2 | Registro de pacientes | CA-37 a 43 | CP2-INT-16 a 23 | 7/7 Sí | Pasa |
| 2 | Visualización y actualización de pacientes | CA-44 a 47 | CP2-INT-24 a 30 | 4/4 Sí | Pasa |
| 2 | Eliminación de pacientes | CA-48 a 50 | CP2-INT-31, 32 | 3/3 Sí | Pasa |
| 3 | Creación de salas | CA-51 a 55 | CP3-INT-01 a 06 | 5/5 Sí | Pasa |
| 3 | Eliminación de salas | CA-56, 57 | CP3-INT-07 a 10 | 2/2 Sí | Pasa |
| 3 | Visualización de salas | CA-58 a 61 | CP3-INT-11 a 14 | 4/4 Sí | Pasa |
| 3 | Creación de citas | CA-62 a 68 | CP3-INT-15 a 29 | 7/7 Sí | Pasa |
| 3 | Visualización de citas | CA-69 a 71 | CP3-INT-30 a 35 | 3/3 Sí | Pasa |
| 3 | Edición de citas | CA-72 a 75 | CP3-INT-36 a 44 | 4/4 Sí | Pasa |
| 3 | Cancelación de citas | CA-76 a 78 | CP3-INT-45 a 50 | 3/3 Sí | Pasa |
| 3 | Integración transversal | Sin CA | CP3-INT-51 a 54 | No aplica | Pasa |
| 4 | Agenda, impresión, ARCO, roles | [PENDIENTE: CA-79 en adelante] | [PENDIENTE] | [PENDIENTE: acta] | Ver sección 8 |

## 3. Matriz RF/RNF → CA → CP (requerimiento por requerimiento)

| Requerimiento | Iteración | CA vinculados | CP vinculados | Resultado en acta | Resultado en pruebas | Cobertura |
| --- | --- | --- | --- | --- | --- | --- |
| RF 1.1.1 | 1 | — | CP-INT-01 | — | Pasa | Solo CP: falta CA explícito |
| RF 1.1.2 | 1 | CA-01 | CP-INT-01, CP-INT-02 | Sí | Pasa | Completa |
| RF 1.1.3 | 1 | CA-01 | CP-INT-01, CP-INT-02 | Sí | Pasa | Completa |
| RF 1.1.4 | 1 | CA-02 | CP-INT-01, CP-INT-03, CP-INT-04 | Sí | Pasa | Completa |
| RF 1.1.5 | 1 | CA-02 | CP-INT-01, CP-INT-03 | Sí | Pasa | Completa |
| RF 1.1.6 | 1 | CA-03 | CP-INT-01, CP-INT-05, CP-INT-06 | Sí | Pasa | Completa |
| RF 1.1.7 | 1 | CA-03 | CP-INT-01, CP-INT-06 | Sí | Pasa | Completa |
| RF 1.1.8 | 1 | CA-03 | CP-INT-01, CP-INT-05 | Sí | Pasa | Completa |
| RF 1.1.9 | 1 | CA-04 | CP-INT-01, CP-INT-07, CP-INT-08, CP-INT-20 | Sí | Pasa | Completa |
| RF 1.1.10 | 1 | CA-04 | CP-INT-01, CP-INT-07, CP-INT-08 | Sí | Pasa | Completa |
| RF 1.1.11 | 1 | CA-05 | CP-INT-01, CP-INT-07, CP-INT-08 | Sí | Pasa | Completa |
| RF 1.1.12 | 1 | CA-06 | CP-INT-01, CP-INT-09, CP-INT-29 | Sí | Pasa | Completa |
| RF 1.1.13 | 1 | CA-06 | CP-INT-01, CP-INT-09, CP-INT-29 | Sí | Pasa | Completa |
| RF 1.1.14 | 1 | CA-06 | CP-INT-01, CP-INT-09, CP-INT-29 | Sí | Pasa | Completa |
| RF 1.1.15 | 1 | CA-06 | CP-INT-01, CP-INT-09, CP-INT-29 | Sí | Pasa | Completa |
| RF 1.1.16 | 1 | CA-06 | CP-INT-01, CP-INT-09, CP-INT-29 | Sí | Pasa | Completa |
| RF 1.1.17 | 1 | CA-07 | CP-INT-01, CP-INT-10, CP-INT-29 | Sí | Pasa | Completa |
| RF 1.1.18 | 1 | CA-07 | CP-INT-01, CP-INT-10, CP-INT-29 | Sí | Pasa | Completa |
| RF 1.2.1 | 1 | CA-10, CA-11 | CP-INT-19, CP-INT-20 | Sí | Pasa | Completa |
| RF 1.2.2 | 1 | CA-10 | CP-INT-12, CP-INT-18 | Sí | Pasa | Completa |
| RF 1.2.3 | 1 | CA-10 | CP-INT-12, CP-INT-14, CP-INT-16 | Sí | Pasa | Completa |
| RF 1.2.4 | 1 | CA-11 | CP-INT-11, CP-INT-17 | Sí | Pasa | Completa |
| RF 1.2.5 | 1 | CA-11 | CP-INT-11, CP-INT-13, CP-INT-15 | Sí | Pasa | Completa |
| RF 1.3.1 | 1 | CA-14 | CP-INT-21 | Sí | Pasa | Completa |
| RF 1.3.2 | 1 | CA-14 | CP-INT-21, CP-INT-22 | Sí | Pasa | Completa |
| RF 1.3.3 | 1 | — | CP-INT-23 | — | Pasa | Solo CP: falta CA explícito |
| RF 1.3.4 | 1 | CA-15 | CP-INT-22 | Sí | Pasa | Completa |
| RF 1.3.5 | 1 | CA-16 | CP-INT-21 | Sí | Pasa | Completa |
| RF 1.3.6 | 1 | CA-16 | CP-INT-21 | Sí | Pasa | Completa |
| RF 1.4.1 | 1 | CA-18 | CP-INT-24 | Sí | Pasa | Completa |
| RF 1.4.2 | 1 | CA-18 | CP-INT-24 | Sí | Pasa | Completa |
| RF 1.4.3 | 1 | CA-18 | CP-INT-24, CP-INT-25 | Sí | Pasa | Completa |
| RF 1.4.4 | 1 | CA-19 | CP-INT-25, CP-INT-26 | Sí | Pasa | Completa |
| RF 1.4.5 | 1 | CA-20 | CP-INT-24 | Sí | Pasa | Completa |
| RF 2.1.1 | 2 | — | CP2-INT-01 | — | Pasa | Solo CP: falta CA explícito |
| RF 2.1.2 | 2 | CA-23 | CP2-INT-01, CP2-INT-02 | Sí | Pasa | Completa |
| RF 2.1.3 | 2 | CA-23 | CP2-INT-01, CP2-INT-02 | Sí | Pasa | Completa |
| RF 2.1.4 | 2 | CA-24 | CP2-INT-01, CP2-INT-03 | Sí | Pasa | Completa |
| RF 2.1.5 | 2 | CA-24 | CP2-INT-01, CP2-INT-03 | Sí | Pasa | Completa |
| RF 2.1.6 | 2 | CA-25 | CP2-INT-01, CP2-INT-04 | Sí | Pasa | Completa |
| RF 2.1.7 | 2 | CA-25 | CP2-INT-01, CP2-INT-04 | Sí | Pasa | Completa |
| RF 2.1.8 | 2 | CA-26 | CP2-INT-01, CP2-INT-05 | Sí | Pasa | Completa |
| RF 2.1.9 | 2 | CA-26 | CP2-INT-01, CP2-INT-05 | Sí | Pasa | Completa |
| RF 2.1.10 | 2 | CA-27 | CP2-INT-01 | Sí | Pasa | Completa |
| RF 2.1.11 | 2 | CA-28 | CP2-INT-07 | Sí | Pasa | Completa |
| RF 2.1.12 | 2 | CA-28 | CP2-INT-07 | Sí | Pasa | Completa |
| RF 2.1.13 | 2 | CA-28 | CP2-INT-07 | Sí | Pasa | Completa |
| RF 2.2.2 | 2 | CA-32 | CP2-INT-10 | Sí | Pasa | Completa |
| RF 2.2.3 | 2 | CA-33 | CP2-INT-11, CP2-INT-13 | Sí | Pasa | Completa |
| RF 2.2.4 | 2 | CA-33, CA-34 | CP2-INT-11, CP2-INT-12 | Sí | Pasa | Completa |
| RF 2.2.5 | 2 | CA-33 | CP2-INT-11 | Sí | Pasa | Completa |
| RF 3.1.1 | 2 | — | CP2-INT-16 | — | Pasa | Solo CP: falta CA explícito |
| RF 3.1.2 | 2 | CA-37 | CP2-INT-16, CP2-INT-17 | Sí | Pasa | Completa |
| RF 3.1.3 | 2 | CA-37 | CP2-INT-16, CP2-INT-17 | Sí | Pasa | Completa |
| RF 3.1.4 | 2 | CA-38 | CP2-INT-16, CP2-INT-18 | Sí | Pasa | Completa |
| RF 3.1.5 | 2 | CA-38 | CP2-INT-16, CP2-INT-18, CP2-INT-23 | Sí | Pasa | Completa |
| RF 3.1.6 | 2 | — | CP2-INT-16 | — | Pasa | Solo CP: falta CA explícito |
| RF 3.1.7 | 2 | CA-39 | CP2-INT-16, CP2-INT-19 | Sí | Pasa | Completa |
| RF 3.1.8 | 2 | CA-39 | CP2-INT-16, CP2-INT-19 | Sí | Pasa | Completa |
| RF 3.1.9 | 2 | CA-39 | CP2-INT-16, CP2-INT-20 | Sí | Pasa | Completa |
| RF 3.1.10 | 2 | CA-40 | CP2-INT-16, CP2-INT-21 | Sí | Pasa | Completa |
| RF 3.1.11 | 2 | CA-40 | CP2-INT-16, CP2-INT-21 | Sí | Pasa | Completa |
| RF 3.1.12 | 2 | CA-41 | CP2-INT-16 | Sí | Pasa | Completa |
| RF 3.2.1 | 2 | CA-44 | CP2-INT-24 | Sí | Pasa | Completa |
| RF 3.2.3 | 2 | CA-45 | CP2-INT-25 | Sí | Pasa | Completa |
| RF 3.2.4 | 2 | CA-46 | CP2-INT-26, CP2-INT-28 | Sí | Pasa | Completa |
| RF 3.2.5 | 2 | CA-46 | CP2-INT-26, CP2-INT-27 | Sí | Pasa | Completa |
| RF 3.2.6 | 2 | CA-46 | CP2-INT-26 | Sí | Pasa | Completa |
| RF 3.3.1 | 2 | CA-48 | CP2-INT-31 | Sí | Pasa | Completa |
| RF 3.3.2 | 2 | CA-48, CA-49 | CP2-INT-31, CP2-INT-32 | Sí | Pasa | Completa |
| RF 3.3.3 | 2 | CA-48 | CP2-INT-31 | Sí | Pasa | Completa |
| RF 4.1.1 | 3 | CA-53 | CP3-INT-01 | Sí | Pasa | Completa |
| RF 4.1.2 | 3 | CA-51 | CP3-INT-02 | Sí | Pasa | Completa |
| RF 4.1.3 | 3 | CA-51 | CP3-INT-02 | Sí | Pasa | Completa |
| RF 4.1.4 | 3 | CA-52 | CP3-INT-04 | Sí | Pasa | Completa |
| RF 4.2.1 | 3 | CA-57 | CP3-INT-08, CP3-INT-10 | Sí | Pasa | Completa |
| RF 4.2.2 | 3 | CA-56 | CP3-INT-07 | Sí | Pasa | Completa |
| RF 4.2.3 | 3 | CA-56 | CP3-INT-07 | Sí | Pasa | Completa |
| RF 4.2.4 | 3 | CA-57 | CP3-INT-08, CP3-INT-09 | Sí | Pasa | Completa |
| RF 4.2.5 | 3 | CA-57 | CP3-INT-08 | Sí | Pasa | Completa |
| RF 4.3.1 | 3 | CA-58 | CP3-INT-11 | Sí | Pasa | Completa |
| RF 4.3.2 | 3 | CA-58 | CP3-INT-11, CP3-INT-51, CP3-INT-52, CP3-INT-53 | Sí | Pasa | Completa |
| RF 4.3.3 | 3 | CA-58 | CP3-INT-11 | Sí | Pasa | Completa |
| RF 5.1.2 | 3 | CA-62 | CP3-INT-15, CP3-INT-24, CP3-INT-26, CP3-INT-54 | Sí | Pasa | Completa |
| RF 5.1.3 | 3 | CA-62 | CP3-INT-15, CP3-INT-21, CP3-INT-22, CP3-INT-23 | Sí | Pasa | Completa |
| RF 5.1.4 | 3 | CA-63 | CP3-INT-16, CP3-INT-21, CP3-INT-25 | Sí | Pasa | Completa |
| RF 5.1.5 | 3 | CA-63 | CP3-INT-16 | Sí | Pasa | Completa |
| RF 5.1.6 | 3 | CA-63 | CP3-INT-16 | Sí | Pasa | Completa |
| RF 5.1.7 | 3 | CA-63 | CP3-INT-16 | Sí | Pasa | Completa |
| RF 5.1.8 | 3 | CA-63 | CP3-INT-16 | Sí | Pasa | Completa |
| RF 5.1.9 | 3 | CA-63 | CP3-INT-16 | Sí | Pasa | Completa |
| RF 5.1.10 | 3 | CA-64 | CP3-INT-17 | Sí | Pasa | Completa |
| RF 5.1.11 | 3 | CA-65 | CP3-INT-18, CP3-INT-52 | Sí | Pasa | Completa |
| RF 5.1.12 | 3 | CA-65 | CP3-INT-18, CP3-INT-19 | Sí | Pasa | Completa |
| RF 5.1.13 | 3 | CA-65 | CP3-INT-18 | Sí | Pasa | Completa |
| RF 5.1.14 | 3 | CA-66 | CP3-INT-20 | Sí | Pasa | Completa |
| RF 5.2.1 | 3 | CA-69 | CP3-INT-30 | Sí | Pasa | Completa |
| RF 5.2.2 | 3 | CA-69 | CP3-INT-30 | Sí | Pasa | Completa |
| RF 5.2.3 | 3 | CA-70 | CP3-INT-31, CP3-INT-32, CP3-INT-33, CP3-INT-34 | Sí | Pasa | Completa |
| RF 5.3.1 | 3 | CA-72 | CP3-INT-36 | Sí | Pasa | Completa |
| RF 5.3.2 | 3 | CA-72 | CP3-INT-36 | Sí | Pasa | Completa |
| RF 5.3.3 | 3 | CA-73 | CP3-INT-37, CP3-INT-53 | Sí | Pasa | Completa |
| RF 5.3.4 | 3 | CA-73 | CP3-INT-37, CP3-INT-40, CP3-INT-41, CP3-INT-42 | Sí | Pasa | Completa |
| RF 5.3.5 | 3 | CA-73 | CP3-INT-37, CP3-INT-39 | Sí | Pasa | Completa |
| RF 5.3.6 | 3 | CA-74 | CP3-INT-38 | Sí | Pasa | Completa |
| RF 5.4.1 | 3 | CA-76 | CP3-INT-45 | Sí | Pasa | Completa |
| RF 5.4.2 | 3 | CA-76 | CP3-INT-45, CP3-INT-46 | Sí | Pasa | Completa |
| RF 5.4.3 | 3 | CA-76 | CP3-INT-45, CP3-INT-48 | Sí | Pasa | Completa |
| RF 5.4.4 | 3 | CA-77 | CP3-INT-47, CP3-INT-51 | Sí | Pasa | Completa |
| RNF 1.1.2 | 1 | CA-08 | — | Sí | — | Solo CA: falta CP |
| RNF 1.1.3 | 1 | CA-09 | — | Sí | — | Solo CA: falta CP |
| RNF 1.2.2 | 1 | CA-12 | — | Sí | — | Solo CA: falta CP |
| RNF 1.2.3 | 1 | CA-13 | — | Sí | — | Solo CA: falta CP |
| RNF 1.3.1 | 1 | CA-17 | — | Sí | — | Solo CA: falta CP |
| RNF 1.3.3 | 1 | CA-17 | — | Sí | — | Solo CA: falta CP |
| RNF 1.4.1 | 1 | CA-20 | CP-INT-24 | Sí | Pasa | Completa |
| RNF 1.4.2 | 1 | CA-21 | CP-INT-27 | Sí | Pasa | Completa |
| RNF 1.4.3 | 1 | CA-19 | — | Sí | — | Solo CA: falta CP |
| RNF 1.4.4 | 1 | CA-22 | CP-INT-28, CP-INT-29 | Sí | Pasa | Completa |
| RNF 2.1.1 | 2 | — | CP2-INT-06 | — | Pasa | Solo CP: falta CA explícito |
| RNF 2.1.2 | 2 | CA-29 | — | Sí | — | Solo CA: falta CP |
| RNF 2.1.3 | 2 | — | CP2-INT-08, CP2-INT-09, CP2-INT-14 | — | Pasa | Solo CP: falta CA explícito |
| RNF 2.1.4 | 2 | CA-30 | — | Sí | — | Solo CA: falta CP |
| RNF 2.1.6 | 2 | CA-26 | CP2-INT-05 | Sí | Pasa | Completa |
| RNF 2.1.7 | 2 | CA-31 | — | Sí | — | Solo CA: falta CP |
| RNF 2.2.1 | 2 | CA-35 | — | Sí | — | Solo CA: falta CP |
| RNF 2.2.5 | 2 | CA-34 | CP2-INT-12 | Sí | Pasa | Completa |
| RNF 2.2.7 | 2 | CA-36 | CP2-INT-15 | Sí | Pasa | Completa |
| RNF 3.1.1 | 2 | — | CP2-INT-22 | — | Pasa | Solo CP: falta CA explícito |
| RNF 3.1.3 | 2 | CA-42 | — | Sí | — | Solo CA: falta CP |
| RNF 3.1.5 | 2 | CA-39 | CP2-INT-20 | Sí | Pasa | Completa |
| RNF 3.1.6 | 2 | CA-43 | — | Sí | — | Solo CA: falta CP |
| RNF 3.2.1 | 2 | CA-47 | — | Sí | — | Solo CA: falta CP |
| RNF 3.2.6 | 2 | — | CP2-INT-29 | — | Pasa | Solo CP: falta CA explícito |
| RNF 3.2.7 | 2 | — | CP2-INT-30 | — | Pasa | Solo CP: falta CA explícito |
| RNF 3.2.8 | 2 | CA-50 | — | Sí | — | Solo CA: falta CP |
| RNF 4.1.1 | 3 | — | CP3-INT-03 | — | Pasa | Solo CP: falta CA explícito |
| RNF 4.1.2 | 3 | CA-54 | CP3-INT-05 | Sí | Pasa | Completa |
| RNF 4.1.4 | 3 | CA-55 | CP3-INT-06 | Sí | Pasa | Completa |
| RNF 4.2.1 | 3 | CA-59 | CP3-INT-12 | Sí | Pasa | Completa |
| RNF 4.2.3 | 3 | CA-60 | CP3-INT-13 | Sí | Pasa | Completa |
| RNF 4.2.5 | 3 | CA-61 | CP3-INT-14 | Sí | Pasa | Completa |
| RNF 5.1.1 | 3 | CA-67 | CP3-INT-27 | Sí | Pasa | Completa |
| RNF 5.1.2 | 3 | CA-68 | CP3-INT-28 | Sí | Pasa | Completa |
| RNF 5.1.3 | 3 | CA-75 | CP3-INT-43, CP3-INT-49 | Sí | Pasa | Completa |
| RNF 5.1.4 | 3 | CA-71 | CP3-INT-35 | Sí | Pasa | Completa |
| RNF 5.1.5 | 3 | CA-78 | CP3-INT-29, CP3-INT-44, CP3-INT-50 | Sí | Pasa | Completa |

## 4. Matriz CA → RF/RNF → CP

| CA | Iteración | Módulo | Criterio de aceptación | Requerimientos | CP directos | CP de flujo completo | Resultado en acta | Cobertura |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| CA-01 | 1 | Registro de usuarios | DADO que un miembro del personal clínico con credenciales institucionales UADY accede a la pantalla de registro, CUANDO ingresa un nombre completo de más de 50 caracteres, ENTONCES el sistema muestra un mensaje de error claro y no permite continuar. | RF 1.1.2, RF 1.1.3 | CP-INT-02 | CP-INT-01 | Sí | Completa |
| CA-02 | 1 | Registro de usuarios | DADO que el usuario está llenando el formulario de registro, CUANDO ingresa un número telefónico ya registrado en el sistema, ENTONCES el sistema rechaza el dato y solicita uno diferente. | RF 1.1.4, RF 1.1.5 | CP-INT-03, CP-INT-04 | CP-INT-01 | Sí | Completa |
| CA-03 | 1 | Registro de usuarios | DADO que el usuario está llenando el formulario de registro, CUANDO ingresa un correo que no cumple el formato institucional UADY o que ya está registrado, ENTONCES el sistema muestra un mensaje de error y no permite avanzar. | RF 1.1.6, RF 1.1.7, RF 1.1.8 | CP-INT-05, CP-INT-06 | CP-INT-01 | Sí | Completa |
| CA-04 | 1 | Registro de usuarios | DADO que el usuario ingresó un correo institucional válido y no registrado, CUANDO confirma ser el titular de dicho correo, ENTONCES el sistema envía un código de verificación a ese correo. | RF 1.1.9, RF 1.1.10 | CP-INT-07, CP-INT-08, CP-INT-20 | CP-INT-01 | Sí | Completa |
| CA-05 | 1 | Registro de usuarios | DADO que el usuario recibió el código de verificación, CUANDO lo ingresa correctamente en el sistema, ENTONCES el sistema le permite continuar con la definición de su contraseña. | RF 1.1.11 | CP-INT-07, CP-INT-08 | CP-INT-01 | Sí | Completa |
| CA-06 | 1 | Registro de usuarios | DADO que el usuario está definiendo su contraseña, CUANDO ingresa una contraseña que no cumple con el mínimo de 8 ni el máximo de 25 caracteres, o que carece de número, carácter especial o mayúscula, ENTONCES el sistema muestra un mensaje de error y no acepta la contraseña. | RF 1.1.12, RF 1.1.13, RF 1.1.14, RF 1.1.15, RF 1.1.16 | CP-INT-09 | CP-INT-01, CP-INT-29 | Sí | Completa |
| CA-07 | 1 | Registro de usuarios | DADO que el usuario ingresó una contraseña válida, CUANDO la confirma por segunda vez con un valor diferente al ingresado inicialmente, ENTONCES el sistema muestra un mensaje de error indicando que las contraseñas no coinciden. | RF 1.1.17, RF 1.1.18 | CP-INT-10 | CP-INT-01, CP-INT-29 | Sí | Completa |
| CA-08 | 1 | Registro de usuarios | DADO que el usuario completó correctamente todos los datos y la confirmación de contraseña, CUANDO envía el formulario de registro, ENTONCES el sistema valida los datos en menos de 2 segundos y confirma el registro exitoso. | RNF 1.1.2 | — | — | Sí | Sin CP: falta caso de prueba |
| CA-09 | 1 | Registro de usuarios | DADO que un usuario inicia el proceso de registro, CUANDO completa todas las validaciones y la confirmación por correo, ENTONCES el tiempo total del proceso no excede los 3 minutos. | RNF 1.1.3 | — | — | Sí | Sin CP: falta caso de prueba |
| CA-10 | 1 | Inicio de sesión | DADO que un usuario registrado se encuentra en la pantalla de inicio de sesión, CUANDO ingresa su teléfono y contraseña correctos, ENTONCES el sistema valida los datos en menos de 3 segundos y le da acceso al panel principal. | RF 1.2.1, RF 1.2.2, RF 1.2.3 | CP-INT-12, CP-INT-14, CP-INT-16, CP-INT-18, CP-INT-19, CP-INT-20 | — | Sí | Completa |
| CA-11 | 1 | Inicio de sesión | DADO que un usuario registrado se encuentra en la pantalla de inicio de sesión, CUANDO ingresa su correo electrónico y contraseña correctos, ENTONCES el sistema valida los datos en menos de 3 segundos y le da acceso al panel principal. | RF 1.2.1, RF 1.2.4, RF 1.2.5 | CP-INT-11, CP-INT-13, CP-INT-15, CP-INT-17, CP-INT-19, CP-INT-20 | — | Sí | Completa |
| CA-12 | 1 | Inicio de sesión | DADO que un usuario intenta iniciar sesión, CUANDO ingresa una credencial incorrecta (correo/teléfono o contraseña), ENTONCES el sistema muestra un mensaje de error genérico sin indicar cuál de los dos datos es incorrecto. | RNF 1.2.2 | — | — | Sí | Sin CP: falta caso de prueba |
| CA-13 | 1 | Inicio de sesión | DADO que un usuario inicia el proceso de autenticación bajo condiciones normales de red, CUANDO ingresa sus credenciales correctas, ENTONCES el tiempo total de autenticación es inferior a 1 minuto. | RNF 1.2.3 | — | — | Sí | Sin CP: falta caso de prueba |
| CA-14 | 1 | Cierre de sesión | DADO que un usuario tiene una sesión activa, CUANDO selecciona la opción de cerrar sesión, ENTONCES el sistema le solicita una confirmación antes de proceder. | RF 1.3.1, RF 1.3.2 | CP-INT-21, CP-INT-22 | — | Sí | Completa |
| CA-15 | 1 | Cierre de sesión | DADO que el sistema solicitó confirmación de cierre de sesión, CUANDO el usuario elige no cerrarla, ENTONCES el sistema continúa operando en la pantalla actual sin interrumpir la sesión. | RF 1.3.4 | CP-INT-22 | — | Sí | Completa |
| CA-16 | 1 | Cierre de sesión | DADO que el sistema solicitó confirmación de cierre de sesión, CUANDO el usuario acepta cerrarla, ENTONCES el sistema cierra la sesión y redirige al usuario a la pantalla de inicio de sesión. | RF 1.3.5, RF 1.3.6 | CP-INT-21 | — | Sí | Completa |
| CA-17 | 1 | Cierre de sesión | DADO que un usuario confirmó el cierre de sesión, CUANDO el sistema procesa la solicitud, ENTONCES elimina de inmediato los datos de sesión y completa la operación en menos de 2 segundos. | RNF 1.3.1, RNF 1.3.3 | — | — | Sí | Sin CP: falta caso de prueba |
| CA-18 | 1 | Recuperación de cuenta | DADO que un usuario olvidó su contraseña, CUANDO selecciona la opción de recuperar cuenta, ENTONCES el sistema le solicita ingresar su correo electrónico. | RF 1.4.1, RF 1.4.2, RF 1.4.3 | CP-INT-24, CP-INT-25 | — | Sí | Completa |
| CA-19 | 1 | Recuperación de cuenta | DADO que el usuario ingresó un correo con formato inválido, CUANDO envía la solicitud de recuperación, ENTONCES el sistema muestra un mensaje de error sin indicar si el correo existe o no en el sistema. | RF 1.4.4, RNF 1.4.3 | CP-INT-25, CP-INT-26 | — | Sí | Completa |
| CA-20 | 1 | Recuperación de cuenta | DADO que el usuario ingresó un correo con formato válido, CUANDO envía la solicitud de recuperación, ENTONCES el sistema envía un enlace de restablecimiento a ese correo en menos de 2 minutos. | RF 1.4.5, RNF 1.4.1 | CP-INT-24 | — | Sí | Completa |
| CA-21 | 1 | Recuperación de cuenta | DADO que el sistema envió un enlace de restablecimiento, CUANDO transcurren 10 minutos sin que el usuario lo utilice, ENTONCES el enlace caduca automáticamente. | RNF 1.4.2 | CP-INT-27 | — | Sí | Completa |
| CA-22 | 1 | Recuperación de cuenta | DADO que el usuario accede al enlace de restablecimiento dentro del tiempo válido, CUANDO ingresa y confirma su nueva contraseña, ENTONCES el sistema la valida en menos de 2 segundos y la almacena cifrada de inmediato. | RNF 1.4.4 | CP-INT-28 | CP-INT-29 | Sí | Completa |
| CA-23 | 2 | Registro de terapeutas | DADO que el usuario está llenando el formulario de registro de terapeuta, CUANDO ingresa un nombre completo de más de 50 caracteres, ENTONCES el sistema muestra un mensaje de error claro y no permite continuar. | RF 2.1.2, RF 2.1.3 | CP2-INT-02 | CP2-INT-01 | Sí | Completa |
| CA-24 | 2 | Registro de terapeutas | DADO que el usuario está llenando el formulario de registro de terapeuta, CUANDO ingresa un número telefónico ya registrado en el sistema, ENTONCES el sistema rechaza el dato y muestra un mensaje de error. | RF 2.1.4, RF 2.1.5 | CP2-INT-03 | CP2-INT-01 | Sí | Completa |
| CA-25 | 2 | Registro de terapeutas | DADO que el usuario está llenando el formulario de registro de terapeuta, CUANDO ingresa un correo electrónico ya registrado en el sistema, ENTONCES el sistema rechaza el dato y muestra un mensaje de error. | RF 2.1.6, RF 2.1.7 | CP2-INT-04 | CP2-INT-01 | Sí | Completa |
| CA-26 | 2 | Registro de terapeutas | DADO que el usuario está llenando el formulario de registro de terapeuta, CUANDO ingresa una fecha de nacimiento igual o posterior a la fecha actual, ENTONCES el sistema notifica el error de forma inmediata y no permite continuar. | RF 2.1.8, RF 2.1.9, RNF 2.1.6 | CP2-INT-05 | CP2-INT-01 | Sí | Completa |
| CA-27 | 2 | Registro de terapeutas | DADO que el usuario completó correctamente todos los datos del terapeuta, CUANDO envía el formulario de registro, ENTONCES el sistema guarda los datos del nuevo terapeuta. | RF 2.1.10 | — | CP2-INT-01 | Sí | Solo CP de flujo completo |
| CA-28 | 2 | Registro de terapeutas | DADO que el usuario está cargando la foto de perfil del terapeuta, CUANDO la imagen tiene dimensiones menores a 200x200 píxeles, ENTONCES el sistema la rechaza y muestra un mensaje de error. | RF 2.1.11, RF 2.1.12, RF 2.1.13 | CP2-INT-07 | — | Sí | Completa |
| CA-29 | 2 | Registro de terapeutas | DADO que el usuario envió el formulario de registro de terapeuta, CUANDO el sistema procesa los datos, ENTONCES los valida en menos de 4 segundos. | RNF 2.1.2 | — | — | Sí | Sin CP: falta caso de prueba |
| CA-30 | 2 | Registro de terapeutas | DADO que el usuario ingresó el correo electrónico y el teléfono del terapeuta, CUANDO el sistema verifica su unicidad, ENTONCES completa la validación en menos de 2 segundos. | RNF 2.1.4 | — | — | Sí | Sin CP: falta caso de prueba |
| CA-31 | 2 | Registro de terapeutas | DADO que un usuario inicia el registro de un terapeuta, CUANDO completa todas las validaciones, ENTONCES el tiempo total del proceso no excede los 3 minutos. | RNF 2.1.7 | — | — | Sí | Sin CP: falta caso de prueba |
| CA-32 | 2 | Visualización y actualización de terapeutas | DADO que el usuario selecciona un terapeuta registrado, CUANDO accede a la vista "Nombre Terapeuta", ENTONCES el sistema muestra nombre completo, fecha de nacimiento, cédula profesional, teléfono, correo electrónico y foto de perfil. | RF 2.2.2 | CP2-INT-10 | — | Sí | Completa |
| CA-33 | 2 | Visualización y actualización de terapeutas | DADO que el usuario está editando el perfil de un terapeuta, CUANDO modifica uno o más campos con datos válidos y guarda, ENTONCES el sistema revalida la unicidad y almacena los cambios exitosamente. | RF 2.2.3, RF 2.2.4, RF 2.2.5 | CP2-INT-11, CP2-INT-12, CP2-INT-13 | — | Sí | Completa |
| CA-34 | 2 | Visualización y actualización de terapeutas | DADO que el usuario está editando el perfil de un terapeuta, CUANDO modifica el correo o el teléfono a un valor ya usado por otro terapeuta, ENTONCES el sistema impide el guardado y muestra el error de forma clara e inmediata. | RF 2.2.4, RNF 2.2.5 | CP2-INT-11, CP2-INT-12 | — | Sí | Completa |
| CA-35 | 2 | Visualización y actualización de terapeutas | DADO que el usuario selecciona un terapeuta registrado, CUANDO el sistema carga la vista detallada, ENTONCES la muestra en menos de 2 segundos. | RNF 2.2.1 | — | — | Sí | Sin CP: falta caso de prueba |
| CA-36 | 2 | Visualización y actualización de terapeutas | DADO que el usuario guarda cambios en el perfil de un terapeuta, CUANDO ocurre un error de conexión durante el guardado, ENTONCES el sistema informa al usuario e impide la pérdida de los cambios introducidos. | RNF 2.2.7 | CP2-INT-15 | — | Sí | Completa |
| CA-37 | 2 | Registro de pacientes | DADO que el usuario está llenando el formulario de registro de paciente, CUANDO ingresa un nombre completo de más de 50 caracteres, ENTONCES el sistema muestra un mensaje de error claro y no permite continuar. | RF 3.1.2, RF 3.1.3 | CP2-INT-17 | CP2-INT-16 | Sí | Completa |
| CA-38 | 2 | Registro de pacientes | DADO que el usuario está llenando el formulario de registro de paciente, CUANDO ingresa un CURP ya registrado en el sistema, ENTONCES el sistema rechaza el dato y muestra un mensaje de error. | RF 3.1.4, RF 3.1.5 | CP2-INT-18, CP2-INT-23 | CP2-INT-16 | Sí | Completa |
| CA-39 | 2 | Registro de pacientes | DADO que el usuario está llenando el formulario de registro de paciente, CUANDO ingresa una fecha de nacimiento que corresponde a una edad menor a 7 años, ENTONCES el sistema muestra un mensaje de error y no permite continuar. | RF 3.1.7, RF 3.1.8, RF 3.1.9, RNF 3.1.5 | CP2-INT-19, CP2-INT-20 | CP2-INT-16 | Sí | Completa |
| CA-40 | 2 | Registro de pacientes | DADO que el usuario está llenando el formulario de registro de paciente, CUANDO ingresa un número telefónico ya registrado en el sistema, ENTONCES el sistema rechaza el dato y muestra un mensaje de error. | RF 3.1.10, RF 3.1.11 | CP2-INT-21 | CP2-INT-16 | Sí | Completa |
| CA-41 | 2 | Registro de pacientes | DADO que el usuario completó correctamente todos los datos del paciente, CUANDO envía el formulario de registro, ENTONCES el sistema guarda los datos ingresados. | RF 3.1.12 | — | CP2-INT-16 | Sí | Solo CP de flujo completo |
| CA-42 | 2 | Registro de pacientes | DADO que el usuario ingresó el CURP y el teléfono del paciente, CUANDO el sistema verifica su unicidad, ENTONCES completa la validación en menos de 2 segundos. | RNF 3.1.3 | — | — | Sí | Sin CP: falta caso de prueba |
| CA-43 | 2 | Registro de pacientes | DADO que un usuario inicia el registro de un paciente, CUANDO completa todas las validaciones, ENTONCES el tiempo total del proceso no excede los 3 minutos. | RNF 3.1.6 | — | — | Sí | Sin CP: falta caso de prueba |
| CA-44 | 2 | Visualización y actualización de pacientes | DADO que existen pacientes registrados en el sistema, CUANDO el usuario accede al listado de pacientes, ENTONCES el sistema muestra los perfiles registrados. | RF 3.2.1 | CP2-INT-24 | — | Sí | Completa |
| CA-45 | 2 | Visualización y actualización de pacientes | DADO que el usuario selecciona un paciente registrado, CUANDO accede a la vista "Nombre Paciente", ENTONCES el sistema muestra nombre completo, fecha de nacimiento, CURP y teléfono. | RF 3.2.3 | CP2-INT-25 | — | Sí | Completa |
| CA-46 | 2 | Visualización y actualización de pacientes | DADO que el usuario está editando el perfil de un paciente, CUANDO modifica uno o más campos con datos válidos y guarda, ENTONCES el sistema revalida la unicidad y almacena los cambios exitosamente. | RF 3.2.4, RF 3.2.5, RF 3.2.6 | CP2-INT-26, CP2-INT-27, CP2-INT-28 | — | Sí | Completa |
| CA-47 | 2 | Visualización y actualización de pacientes | DADO que el usuario accede al listado de pacientes bajo condiciones de red óptimas, CUANDO el sistema carga la lista, ENTONCES lo hace en menos de 2 segundos. | RNF 3.2.1 | — | — | Sí | Sin CP: falta caso de prueba |
| CA-48 | 2 | Eliminación de pacientes | DADO que el usuario selecciona la opción de eliminar el perfil de un paciente, CUANDO confirma la eliminación, ENTONCES el sistema elimina el perfil y muestra un mensaje de confirmación. | RF 3.3.1, RF 3.3.2, RF 3.3.3 | CP2-INT-31, CP2-INT-32 | — | Sí | Completa |
| CA-49 | 2 | Eliminación de pacientes | DADO que el sistema solicitó confirmación para eliminar el perfil de un paciente, CUANDO el usuario no confirma la eliminación, ENTONCES el perfil del paciente se conserva sin cambios. | RF 3.3.2 | CP2-INT-31, CP2-INT-32 | — | Sí | Completa |
| CA-50 | 2 | Eliminación de pacientes | DADO que el usuario confirmó la eliminación del perfil de un paciente, CUANDO el sistema procesa la solicitud, ENTONCES completa la eliminación en menos de 3 segundos. | RNF 3.2.8 | — | — | Sí | Sin CP: falta caso de prueba |
| CA-51 | 3 | Creación de salas | DADO que el usuario está llenando el formulario para agregar una nueva sala, CUANDO ingresa un nombre de más de 10 caracteres, ENTONCES el sistema muestra un mensaje de error claro y no permite continuar. | RF 4.1.2, RF 4.1.3 | CP3-INT-02 | — | Sí | Completa |
| CA-52 | 3 | Creación de salas | DADO que el usuario está llenando el formulario para agregar una nueva sala, CUANDO ingresa un nombre que ya está registrado en el sistema, ENTONCES el sistema rechaza el dato y muestra un mensaje de error. | RF 4.1.4 | CP3-INT-04 | — | Sí | Completa |
| CA-53 | 3 | Creación de salas | DADO que el usuario completó el nombre de la sala con un valor válido y único, CUANDO envía el formulario, ENTONCES el sistema guarda la nueva sala exitosamente. | RF 4.1.1 | CP3-INT-01 | — | Sí | Completa |
| CA-54 | 3 | Creación de salas | DADO que el usuario ingresó el nombre de una nueva sala, CUANDO el sistema verifica su unicidad, ENTONCES completa la validación en menos de 2 segundos. | RNF 4.1.2 | CP3-INT-05 | — | Sí | Completa |
| CA-55 | 3 | Creación de salas | DADO que un usuario inicia el registro de una sala, CUANDO completa todas las validaciones, ENTONCES el tiempo total del proceso no excede 1 minuto. | RNF 4.1.4 | CP3-INT-06 | — | Sí | Completa |
| CA-56 | 3 | Eliminación de salas | DADO que el usuario accede a la opción de eliminar sala, CUANDO el sistema muestra el listado de salas existentes, ENTONCES el usuario puede seleccionar una de ellas. | RF 4.2.2, RF 4.2.3 | CP3-INT-07 | — | Sí | Completa |
| CA-57 | 3 | Eliminación de salas | DADO que el usuario seleccionó una sala para eliminar, CUANDO confirma la eliminación, ENTONCES el sistema la elimina y muestra un mensaje de confirmación. | RF 4.2.1, RF 4.2.4, RF 4.2.5 | CP3-INT-08, CP3-INT-09, CP3-INT-10 | — | Sí | Completa |
| CA-58 | 3 | Visualización de salas | DADO que existen salas registradas en el sistema, CUANDO el usuario accede al listado de salas, ENTONCES el sistema muestra cada sala junto con su estado (reservada o libre) para el día consultado. | RF 4.3.1, RF 4.3.2, RF 4.3.3 | CP3-INT-11, CP3-INT-51, CP3-INT-52, CP3-INT-53 | — | Sí | Completa |
| CA-59 | 3 | Visualización de salas | DADO que el usuario accede al listado de salas bajo condiciones de red óptimas, CUANDO el sistema carga la lista, ENTONCES lo hace en menos de 2 segundos. | RNF 4.2.1 | CP3-INT-12 | — | Sí | Completa |
| CA-60 | 3 | Visualización de salas | DADO que el usuario está editando los datos de una sala, CUANDO los datos no pasan las validaciones de unicidad o formato, ENTONCES el sistema impide el guardado y muestra el error de forma clara e inmediata. | RNF 4.2.3 | CP3-INT-13 | — | Sí | Completa |
| CA-61 | 3 | Visualización de salas | DADO que el usuario guarda cambios en una sala, CUANDO ocurre un error de conexión durante el guardado, ENTONCES el sistema informa al usuario e impide la pérdida de los cambios introducidos. | RNF 4.2.5 | CP3-INT-14 | — | Sí | Completa |
| CA-62 | 3 | Creación de citas | DADO que el usuario está agendando una nueva cita, CUANDO selecciona un paciente y un terapeuta de las listas registradas, ENTONCES el sistema muestra los horarios y fechas de salas disponibles. | RF 5.1.2, RF 5.1.3 | CP3-INT-15, CP3-INT-21, CP3-INT-22, CP3-INT-23, CP3-INT-24, CP3-INT-26, CP3-INT-54 | — | Sí | Completa |
| CA-63 | 3 | Creación de citas | DADO que el sistema muestra los horarios y fechas disponibles, CUANDO el usuario selecciona una sala en un horario y fecha específicos, ENTONCES el sistema asigna el estatus "Pendiente" y muestra el horario, la fecha, el paciente y el terapeuta seleccionados. | RF 5.1.4, RF 5.1.5, RF 5.1.6, RF 5.1.7, RF 5.1.8, RF 5.1.9 | CP3-INT-21, CP3-INT-25 | CP3-INT-16 | Sí | Completa |
| CA-64 | 3 | Creación de citas | DADO que el usuario completó los datos de la cita, CUANDO el sistema muestra el resumen correspondiente, ENTONCES el usuario puede revisar los datos antes de guardar. | RF 5.1.10 | CP3-INT-17 | — | Sí | Completa |
| CA-65 | 3 | Creación de citas | DADO que el usuario confirmó los datos de la cita, CUANDO el sistema la guarda, ENTONCES genera un folio y muestra un mensaje confirmando que la cita fue agendada con éxito. | RF 5.1.11, RF 5.1.12, RF 5.1.13 | CP3-INT-18, CP3-INT-19, CP3-INT-52 | — | Sí | Completa |
| CA-66 | 3 | Creación de citas | DADO que una cita fue agendada exitosamente, CUANDO el sistema procesa la confirmación, ENTONCES envía un correo al paciente con su nombre, fecha, hora, folio, terapeuta y sala. | RF 5.1.14 | CP3-INT-20 | — | Sí | Completa |
| CA-67 | 3 | Creación de citas | DADO que el usuario solicita ver los horarios disponibles de las salas, CUANDO el sistema procesa la solicitud, ENTONCES los muestra en menos de 3 segundos. | RNF 5.1.1 | CP3-INT-27 | — | Sí | Completa |
| CA-68 | 3 | Creación de citas | DADO que el usuario confirmó el guardado de una cita, CUANDO el sistema genera el folio, ENTONCES lo hace en menos de 2 segundos. | RNF 5.1.2 | CP3-INT-28 | — | Sí | Completa |
| CA-69 | 3 | Visualización de citas | DADO que existen citas registradas, CUANDO el usuario accede al listado de citas, ENTONCES el sistema las muestra categorizadas por estatus (pendientes, canceladas, vencidas). | RF 5.2.1, RF 5.2.2 | CP3-INT-30 | — | Sí | Completa |
| CA-70 | 3 | Visualización de citas | DADO que el usuario accede al listado de citas, CUANDO aplica un filtro por sala, terapeuta, día, semana o mes, ENTONCES el sistema muestra únicamente las citas que corresponden a ese filtro. | RF 5.2.3 | CP3-INT-31, CP3-INT-32, CP3-INT-33, CP3-INT-34 | — | Sí | Completa |
| CA-71 | 3 | Visualización de citas | DADO que el usuario realiza una búsqueda de citas por estado, terapeuta, sala o periodo, CUANDO el sistema procesa la búsqueda, ENTONCES muestra los resultados en menos de 5 segundos. | RNF 5.1.4 | CP3-INT-35 | — | Sí | Completa |
| CA-72 | 3 | Edición de citas | DADO que el usuario selecciona una cita existente para modificar, CUANDO el sistema muestra sus datos, ENTONCES despliega el paciente, terapeuta, sala, fecha, hora y estatus actuales. | RF 5.3.1, RF 5.3.2 | CP3-INT-36 | — | Sí | Completa |
| CA-73 | 3 | Edición de citas | DADO que el usuario modifica uno o más campos de una cita con datos válidos, CUANDO solicita guardar el cambio, ENTONCES el sistema valida los nuevos datos y solicita confirmación antes de aplicarlos. | RF 5.3.3, RF 5.3.4, RF 5.3.5 | CP3-INT-37, CP3-INT-39, CP3-INT-40, CP3-INT-41, CP3-INT-42, CP3-INT-53 | — | Sí | Completa |
| CA-74 | 3 | Edición de citas | DADO que el usuario confirmó la modificación de una cita, CUANDO el sistema guarda los cambios, ENTONCES muestra un mensaje de modificación exitosa. | RF 5.3.6 | CP3-INT-38 | — | Sí | Completa |
| CA-75 | 3 | Edición de citas | DADO que una cita fue modificada, CUANDO el sistema aplica el cambio, ENTONCES éste se refleja en la agenda en menos de 1 segundo sin necesidad de recargar la página. | RNF 5.1.3 | CP3-INT-43, CP3-INT-49 | — | Sí | Completa |
| CA-76 | 3 | Cancelación de citas | DADO que el usuario desea cancelar una cita, CUANDO ingresa el folio correspondiente, ENTONCES el sistema localiza la cita y solicita confirmación antes de cancelarla. | RF 5.4.1, RF 5.4.2, RF 5.4.3 | CP3-INT-45, CP3-INT-46, CP3-INT-48 | — | Sí | Completa |
| CA-77 | 3 | Cancelación de citas | DADO que el usuario confirmó la cancelación de una cita, CUANDO el sistema procesa la solicitud, ENTONCES cambia el estatus de la cita a "Cancelada" y muestra un mensaje de confirmación. | RF 5.4.4 | CP3-INT-47, CP3-INT-51 | — | Sí | Completa |
| CA-78 | 3 | Cancelación de citas | DADO que el usuario está registrando, modificando o cancelando una cita, CUANDO ocurre un error de conexión durante la operación, ENTONCES el sistema informa al usuario e impide la pérdida de los datos introducidos. | RNF 5.1.5 | CP3-INT-29, CP3-INT-44, CP3-INT-50 | — | Sí | Completa |

## 5. Matriz CP → RF/RNF → CA

| CP | Iteración | Módulo | Caso de prueba | Requerimientos (según plan) | CA vinculados | Estado | Fecha de ejecución | Responsable |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| CP-INT-01 | 1 | Registro de usuarios | Registro exitoso con todos los datos válidos | RF 1.1.1-1.1.18 | CA-01, CA-02, CA-03, CA-04, CA-05, CA-06, CA-07 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-02 | 1 | Registro de usuarios | Nombre con formato inválido | RF 1.1.2, RF 1.1.3 | CA-01 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-03 | 1 | Registro de usuarios | Número telefónico ya registrado | RF 1.1.4, RF 1.1.5 | CA-02 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-04 | 1 | Registro de usuarios | Número telefónico con formato incorrecto | RF 1.1.4 | CA-02 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-05 | 1 | Registro de usuarios | Correo institucional ya registrado | RF 1.1.6, RF 1.1.8 | CA-03 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-06 | 1 | Registro de usuarios | Correo institucional con formato incorrecto | RF 1.1.6, RF 1.1.7 | CA-03 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-07 | 1 | Registro de usuarios | Código de verificación inválido | RF 1.1.9-1.1.11 | CA-04, CA-05 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-08 | 1 | Registro de usuarios | Código de verificación expirado | RF 1.1.9-1.1.11 | CA-04, CA-05 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-09 | 1 | Registro de usuarios | Contraseña con formato inválido | RF 1.1.12-1.1.16 | CA-06 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-10 | 1 | Registro de usuarios | Contraseñas no coinciden | RF 1.1.17, RF 1.1.18 | CA-07 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-11 | 1 | Inicio de sesión | Inicio de sesión con correo y contraseña correctos | RF 1.2.4, RF 1.2.5 | CA-11 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-12 | 1 | Inicio de sesión | Inicio de sesión con teléfono y contraseña correctos | RF 1.2.2, RF 1.2.3 | CA-10 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-13 | 1 | Inicio de sesión | Inicio de sesión con correo no registrado | RF 1.2.5 | CA-11 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-14 | 1 | Inicio de sesión | Inicio de sesión con teléfono no registrado | RF 1.2.3 | CA-10 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-15 | 1 | Inicio de sesión | Correo correcto, contraseña incorrecta | RF 1.2.5 | CA-11 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-16 | 1 | Inicio de sesión | Teléfono correcto, contraseña incorrecta | RF 1.2.3 | CA-10 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-17 | 1 | Inicio de sesión | Intento sin llenar campo correo | RF 1.2.4 | CA-11 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-18 | 1 | Inicio de sesión | Intento sin llenar campo teléfono | RF 1.2.2 | CA-10 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-19 | 1 | Inicio de sesión | Intento sin llenar campo contraseña | RF 1.2.1 | CA-10, CA-11 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-20 | 1 | Inicio de sesión | Inicio de sesión con correo no validado | RF 1.1.9, RF 1.2.1 | CA-04, CA-10, CA-11 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-21 | 1 | Cierre de sesión | Cerrar sesión exitosamente | RF 1.3.1, RF 1.3.2, RF 1.3.5, RF 1.3.6 | CA-14, CA-16 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-22 | 1 | Cierre de sesión | Cancelar cierre de sesión | RF 1.3.2, RF 1.3.4 | CA-14, CA-15 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-23 | 1 | Cierre de sesión | Cierre de sesión con acción en curso | RF 1.3.3 | — | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-24 | 1 | Recuperación de cuenta | Recuperación exitosa con correo registrado | RF 1.4.1-1.4.3, RF 1.4.5, RNF 1.4.1 | CA-18, CA-20 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-25 | 1 | Recuperación de cuenta | Recuperación con correo de formato inválido | RF 1.4.3, RF 1.4.4 | CA-18, CA-19 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-26 | 1 | Recuperación de cuenta | Recuperación con correo no registrado | RF 1.4.4 | CA-19 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-27 | 1 | Recuperación de cuenta | Caducidad del enlace de restablecimiento | RNF 1.4.2 | CA-21 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-28 | 1 | Recuperación de cuenta | Restablecimiento exitoso de la contraseña | RNF 1.4.4 | CA-22 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP-INT-29 | 1 | Recuperación de cuenta | Contraseña con formato inválido al restablecer | RF 1.1.12-1.1.18, RNF 1.4.4 | CA-06, CA-07, CA-22 | Pasa | 2026-09-18 | Mariana Caballero Beltrán |
| CP2-INT-01 | 2 | Registro de terapeutas | Registro exitoso de terapeuta | RF 2.1.1-2.1.10 | CA-23, CA-24, CA-25, CA-26, CA-27 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-02 | 2 | Registro de terapeutas | Nombre con formato inválido | RF 2.1.2, RF 2.1.3 | CA-23 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-03 | 2 | Registro de terapeutas | Teléfono ya registrado | RF 2.1.4, RF 2.1.5 | CA-24 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-04 | 2 | Registro de terapeutas | Correo electrónico ya registrado | RF 2.1.6, RF 2.1.7 | CA-25 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-05 | 2 | Registro de terapeutas | Fecha de nacimiento igual o posterior a la actual | RF 2.1.8, RF 2.1.9, RNF 2.1.6 | CA-26 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-06 | 2 | Registro de terapeutas | Campo obligatorio vacío en el registro | RNF 2.1.1 | — | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-07 | 2 | Registro de terapeutas | Foto de perfil con dimensiones menores a 200x200 px | RF 2.1.11-2.1.13 | CA-28 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-08 | 2 | Registro de terapeutas | Foto de perfil con formato no soportado (creación) | RNF 2.1.3 | — | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-09 | 2 | Registro de terapeutas | Foto de perfil que excede el peso máximo (creación) | RNF 2.1.3 | — | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-10 | 2 | Vis./act. de terapeutas | Vista 'Nombre Terapeuta' muestra todos los datos | RF 2.2.2 | CA-32 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-11 | 2 | Vis./act. de terapeutas | Edición exitosa del perfil de un terapeuta | RF 2.2.3-2.2.5 | CA-33, CA-34 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-12 | 2 | Vis./act. de terapeutas | Edición con teléfono o correo duplicado | RF 2.2.4, RNF 2.2.5 | CA-33, CA-34 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-13 | 2 | Vis./act. de terapeutas | Edición con nombre o fecha de nacimiento inválidos | RF 2.2.3 | CA-33 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-14 | 2 | Vis./act. de terapeutas | Edición de foto de perfil con formato o peso inválido | RNF 2.1.3 | — | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-15 | 2 | Vis./act. de terapeutas | Error de conexión durante el guardado | RNF 2.2.7 | CA-36 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-16 | 2 | Registro de pacientes | Registro exitoso de paciente | RF 3.1.1-3.1.12 | CA-37, CA-38, CA-39, CA-40, CA-41 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-17 | 2 | Registro de pacientes | Nombre con formato inválido | RF 3.1.2, RF 3.1.3 | CA-37 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-18 | 2 | Registro de pacientes | CURP ya registrado | RF 3.1.4, RF 3.1.5 | CA-38 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-19 | 2 | Registro de pacientes | Fecha de nacimiento posterior a la fecha de registro | RF 3.1.7, RF 3.1.8 | CA-39 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-20 | 2 | Registro de pacientes | Edad menor a 7 años | RF 3.1.9, RNF 3.1.5 | CA-39 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-21 | 2 | Registro de pacientes | Teléfono ya registrado | RF 3.1.10, RF 3.1.11 | CA-40 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-22 | 2 | Registro de pacientes | Campo obligatorio vacío en el registro | RNF 3.1.1 | — | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-23 | 2 | Registro de pacientes | Registrar paciente con el CURP de un paciente dado de baja | RF 3.1.5 | CA-38 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-24 | 2 | Vis./act. de pacientes | Listado de pacientes registrados | RF 3.2.1 | CA-44 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-25 | 2 | Vis./act. de pacientes | Vista 'Nombre Paciente' muestra los datos | RF 3.2.3 | CA-45 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-26 | 2 | Vis./act. de pacientes | Edición exitosa del perfil de un paciente | RF 3.2.4-3.2.6 | CA-46 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-27 | 2 | Vis./act. de pacientes | Edición con CURP o teléfono duplicado | RF 3.2.5 | CA-46 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-28 | 2 | Vis./act. de pacientes | Edición con nombre o fecha de nacimiento inválidos | RF 3.2.4 | CA-46 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-29 | 2 | Vis./act. de pacientes | Error de conexión durante el guardado | RNF 3.2.6 | — | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-30 | 2 | Vis./act. de pacientes | Confidencialidad de los datos del paciente | RNF 3.2.7 | — | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-31 | 2 | Eliminación de pacientes | Eliminación exitosa con confirmación | RF 3.3.1-3.3.3 | CA-48, CA-49 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP2-INT-32 | 2 | Eliminación de pacientes | Cancelar la eliminación | RF 3.3.2 | CA-48, CA-49 | Pasa | 2026-10-07 | Jimena Guadalupe García Ríos |
| CP3-INT-01 | 3 | Registro de salas | Registro exitoso de sala | RF 4.1.1 | CA-53 | Pasa | 2026-10-20 | Jimena Guadalupe García Ríos |
| CP3-INT-02 | 3 | Registro de salas | Nombre con más de 10 caracteres | RF 4.1.2, RF 4.1.3 | CA-51 | Pasa | 2026-10-20 | Jimena Guadalupe García Ríos |
| CP3-INT-03 | 3 | Registro de salas | Nombre de sala vacío | RNF 4.1.1 | — | Pasa | 2026-10-20 | Jimena Guadalupe García Ríos |
| CP3-INT-04 | 3 | Registro de salas | Sala con nombre ya registrado | RF 4.1.4 | CA-52 | Pasa | 2026-10-20 | Jimena Guadalupe García Ríos |
| CP3-INT-05 | 3 | Registro de salas | Validación de unicidad en menos de 2 segundos | RNF 4.1.2 | CA-54 | Pasa | 2026-10-20 | Jimena Guadalupe García Ríos |
| CP3-INT-06 | 3 | Registro de salas | Registro completo de sala en menos de 1 minuto | RNF 4.1.4 | CA-55 | Pasa | 2026-10-20 | Jimena Guadalupe García Ríos |
| CP3-INT-07 | 3 | Eliminación de salas | Selección de sala a eliminar | RF 4.2.2, RF 4.2.3 | CA-56 | Pasa | 2026-10-20 | Jimena Guadalupe García Ríos |
| CP3-INT-08 | 3 | Eliminación de salas | Eliminación exitosa de sala con confirmación | RF 4.2.1, RF 4.2.4, RF 4.2.5 | CA-57 | Pasa | 2026-10-20 | Jimena Guadalupe García Ríos |
| CP3-INT-09 | 3 | Eliminación de salas | Cancelar la eliminación de una sala | RF 4.2.4 | CA-57 | Pasa | 2026-10-20 | Jimena Guadalupe García Ríos |
| CP3-INT-10 | 3 | Eliminación de salas | Eliminar sala que tiene citas asignadas | RF 4.2.1 | CA-57 | Pasa | 2026-10-20 | Jimena Guadalupe García Ríos |
| CP3-INT-11 | 3 | Visualización de salas | Listado de salas con su estado del día | RF 4.3.1-4.3.3 | CA-58 | Pasa | 2026-10-20 | Jimena Guadalupe García Ríos |
| CP3-INT-12 | 3 | Visualización de salas | Lista de salas en menos de 2 segundos | RNF 4.2.1 | CA-59 | Pasa | 2026-10-20 | Jimena Guadalupe García Ríos |
| CP3-INT-13 | 3 | Visualización de salas | Edición de sala con datos inválidos o duplicados | RNF 4.2.3 | CA-60 | Pasa | 2026-10-20 | Jimena Guadalupe García Ríos |
| CP3-INT-14 | 3 | Visualización de salas | Error de conexión al guardar cambios de una sala | RNF 4.2.5 | CA-61 | Pasa | 2026-10-20 | Jimena Guadalupe García Ríos |
| CP3-INT-15 | 3 | Agendar cita | Horarios disponibles tras elegir paciente y terapeuta | RF 5.1.2, RF 5.1.3 | CA-62 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-16 | 3 | Agendar cita | Selección de sala, fecha y hora asigna estatus Pendiente | RF 5.1.4-5.1.9 | CA-63 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-17 | 3 | Agendar cita | Resumen de confirmación antes de guardar | RF 5.1.10 | CA-64 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-18 | 3 | Agendar cita | Agendar cita exitosamente con folio | RF 5.1.11-5.1.13 | CA-65 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-19 | 3 | Agendar cita | Folios distintos para citas distintas | RF 5.1.12 | CA-65 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-20 | 3 | Agendar cita | Correo de confirmación al paciente | RF 5.1.14 | CA-66 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-21 | 3 | Agendar cita | Crear cita en una sala ya ocupada | RF 5.1.3, RF 5.1.4 | CA-62, CA-63 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-22 | 3 | Agendar cita | Crear cita cuando el terapeuta está ocupado | RF 5.1.3 | CA-62 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-23 | 3 | Agendar cita | Crear cita en horario no disponible | RF 5.1.3 | CA-62 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-24 | 3 | Agendar cita | Crear cita con campos obligatorios sin seleccionar | RF 5.1.2 | CA-62 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-25 | 3 | Agendar cita | Crear cita en una fecha u hora ya pasada | RF 5.1.4 | CA-63 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-26 | 3 | Agendar cita | Crear cita para un paciente que ya tiene otra cita a la misma hora | RF 5.1.2 | CA-62 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-27 | 3 | Agendar cita | Horarios disponibles en menos de 3 segundos | RNF 5.1.1 | CA-67 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-28 | 3 | Agendar cita | Generación del folio en menos de 2 segundos | RNF 5.1.2 | CA-68 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-29 | 3 | Agendar cita | Error de conexión al agendar una cita | RNF 5.1.5 | CA-78 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-30 | 3 | Visualización de citas | Listado de citas categorizado por estatus | RF 5.2.1, RF 5.2.2 | CA-69 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-31 | 3 | Visualización de citas | Filtrado de citas por sala | RF 5.2.3 | CA-70 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-32 | 3 | Visualización de citas | Filtrado de citas por terapeuta | RF 5.2.3 | CA-70 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-33 | 3 | Visualización de citas | Filtrado de citas por día, semana o mes | RF 5.2.3 | CA-70 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-34 | 3 | Visualización de citas | Filtrado de citas con fecha inválida | RF 5.2.3 | CA-70 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-35 | 3 | Visualización de citas | Búsqueda de citas en menos de 5 segundos | RNF 5.1.4 | CA-71 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-36 | 3 | Edición de citas | Mostrar los datos actuales de la cita | RF 5.3.1, RF 5.3.2 | CA-72 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-37 | 3 | Edición de citas | Modificación válida solicita confirmación | RF 5.3.3-5.3.5 | CA-73 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-38 | 3 | Edición de citas | Modificación exitosa de cita | RF 5.3.6 | CA-74 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-39 | 3 | Edición de citas | Cancelar la modificación de una cita | RF 5.3.5 | CA-73 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-40 | 3 | Edición de citas | Modificar la cita a una sala u horario ocupado | RF 5.3.4 | CA-73 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-41 | 3 | Edición de citas | Modificar la cita al terapeuta ocupado en ese horario | RF 5.3.4 | CA-73 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-42 | 3 | Edición de citas | Modificar la cita con un campo vacío | RF 5.3.4 | CA-73 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-43 | 3 | Edición de citas | Cambio de una cita reflejado en la agenda en menos de 1 segundo | RNF 5.1.3 | CA-75 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-44 | 3 | Edición de citas | Error de conexión al modificar una cita | RNF 5.1.5 | CA-78 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-45 | 3 | Cancelación de citas | Localizar la cita por folio y solicitar confirmación | RF 5.4.1-5.4.3 | CA-76 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-46 | 3 | Cancelación de citas | Cancelar con un folio inexistente | RF 5.4.2 | CA-76 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-47 | 3 | Cancelación de citas | Cancelación exitosa de la cita | RF 5.4.4 | CA-77 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-48 | 3 | Cancelación de citas | No confirmar la cancelación | RF 5.4.3 | CA-76 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-49 | 3 | Cancelación de citas | Cancelación reflejada en la agenda en menos de 1 segundo | RNF 5.1.3 | CA-75 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-50 | 3 | Cancelación de citas | Error de conexión al cancelar una cita | RNF 5.1.5 | CA-78 | Pasa | 2026-10-21 | Mariana Caballero Beltrán |
| CP3-INT-51 | 3 | Citas + Salas + Terapeutas | Liberación de sala y terapeuta tras cancelar una cita | RF 5.4.4, RF 4.3.2 | CA-58, CA-77 | Pasa | 2026-10-21 | Jimena Guadalupe García Ríos |
| CP3-INT-52 | 3 | Citas + Salas | Sala reservada tras agendar una cita | RF 5.1.11, RF 4.3.2 | CA-58, CA-65 | Pasa | 2026-10-21 | Jimena Guadalupe García Ríos |
| CP3-INT-53 | 3 | Citas + Salas | Sala anterior liberada tras modificar la cita | RF 5.3.3, RF 4.3.2 | CA-58, CA-73 | Pasa | 2026-10-21 | Jimena Guadalupe García Ríos |
| CP3-INT-54 | 3 | Citas + Pacientes + Terapeutas | Agendar cita con paciente y terapeuta recién registrados | RF 5.1.2 | CA-62 | Pasa | 2026-10-21 | Jimena Guadalupe García Ríos |

## 6. Brechas de trazabilidad

### 6.1 Requerimientos con CA y sin caso de prueba (15)

| Requerimiento | CA vinculados | Iteración | Acción requerida |
| --- | --- | --- | --- |
| RNF 1.1.2 | CA-08 | 1 | Diseñar CP no funcional y ejecutarlo en EDT 6.4.3; [PENDIENTE: CP asignado] |
| RNF 1.1.3 | CA-09 | 1 | Diseñar CP no funcional y ejecutarlo en EDT 6.4.3; [PENDIENTE: CP asignado] |
| RNF 1.2.2 | CA-12 | 1 | Diseñar CP no funcional y ejecutarlo en EDT 6.4.3; [PENDIENTE: CP asignado] |
| RNF 1.2.3 | CA-13 | 1 | Diseñar CP no funcional y ejecutarlo en EDT 6.4.3; [PENDIENTE: CP asignado] |
| RNF 1.3.1 | CA-17 | 1 | Diseñar CP no funcional y ejecutarlo en EDT 6.4.3; [PENDIENTE: CP asignado] |
| RNF 1.3.3 | CA-17 | 1 | Diseñar CP no funcional y ejecutarlo en EDT 6.4.3; [PENDIENTE: CP asignado] |
| RNF 1.4.3 | CA-19 | 1 | Diseñar CP no funcional y ejecutarlo en EDT 6.4.3; [PENDIENTE: CP asignado] |
| RNF 2.1.2 | CA-29 | 2 | Diseñar CP no funcional y ejecutarlo en EDT 6.4.3; [PENDIENTE: CP asignado] |
| RNF 2.1.4 | CA-30 | 2 | Diseñar CP no funcional y ejecutarlo en EDT 6.4.3; [PENDIENTE: CP asignado] |
| RNF 2.1.7 | CA-31 | 2 | Diseñar CP no funcional y ejecutarlo en EDT 6.4.3; [PENDIENTE: CP asignado] |
| RNF 2.2.1 | CA-35 | 2 | Diseñar CP no funcional y ejecutarlo en EDT 6.4.3; [PENDIENTE: CP asignado] |
| RNF 3.1.3 | CA-42 | 2 | Diseñar CP no funcional y ejecutarlo en EDT 6.4.3; [PENDIENTE: CP asignado] |
| RNF 3.1.6 | CA-43 | 2 | Diseñar CP no funcional y ejecutarlo en EDT 6.4.3; [PENDIENTE: CP asignado] |
| RNF 3.2.1 | CA-47 | 2 | Diseñar CP no funcional y ejecutarlo en EDT 6.4.3; [PENDIENTE: CP asignado] |
| RNF 3.2.8 | CA-50 | 2 | Diseñar CP no funcional y ejecutarlo en EDT 6.4.3; [PENDIENTE: CP asignado] |

### 6.2 Requerimientos con caso de prueba y sin CA explícito (11)

| Requerimiento | CP vinculados | Iteración | Acción requerida |
| --- | --- | --- | --- |
| RF 1.1.1 | CP-INT-01 | 1 | Agregar el requerimiento al CA correspondiente o documentar cobertura implícita |
| RF 1.3.3 | CP-INT-23 | 1 | Agregar el requerimiento al CA correspondiente o documentar cobertura implícita |
| RF 2.1.1 | CP2-INT-01 | 2 | Agregar el requerimiento al CA correspondiente o documentar cobertura implícita |
| RF 3.1.1 | CP2-INT-16 | 2 | Agregar el requerimiento al CA correspondiente o documentar cobertura implícita |
| RF 3.1.6 | CP2-INT-16 | 2 | Agregar el requerimiento al CA correspondiente o documentar cobertura implícita |
| RNF 2.1.1 | CP2-INT-06 | 2 | Agregar el requerimiento al CA correspondiente o documentar cobertura implícita |
| RNF 2.1.3 | CP2-INT-08, CP2-INT-09, CP2-INT-14 | 2 | Agregar el requerimiento al CA correspondiente o documentar cobertura implícita |
| RNF 3.1.1 | CP2-INT-22 | 2 | Agregar el requerimiento al CA correspondiente o documentar cobertura implícita |
| RNF 3.2.6 | CP2-INT-29 | 2 | Agregar el requerimiento al CA correspondiente o documentar cobertura implícita |
| RNF 3.2.7 | CP2-INT-30 | 2 | Agregar el requerimiento al CA correspondiente o documentar cobertura implícita |
| RNF 4.1.1 | CP3-INT-03 | 3 | Agregar el requerimiento al CA correspondiente o documentar cobertura implícita |

### 6.3 Criterios de aceptación sin caso de prueba directo

| CA | Requerimientos | Observación |
| --- | --- | --- |
| CA-08 | RNF 1.1.2 | Sin CP directo ni de flujo completo |
| CA-09 | RNF 1.1.3 | Sin CP directo ni de flujo completo |
| CA-12 | RNF 1.2.2 | Sin CP directo ni de flujo completo |
| CA-13 | RNF 1.2.3 | Sin CP directo ni de flujo completo |
| CA-17 | RNF 1.3.1, RNF 1.3.3 | Sin CP directo ni de flujo completo |
| CA-29 | RNF 2.1.2 | Sin CP directo ni de flujo completo |
| CA-30 | RNF 2.1.4 | Sin CP directo ni de flujo completo |
| CA-31 | RNF 2.1.7 | Sin CP directo ni de flujo completo |
| CA-35 | RNF 2.2.1 | Sin CP directo ni de flujo completo |
| CA-42 | RNF 3.1.3 | Sin CP directo ni de flujo completo |
| CA-43 | RNF 3.1.6 | Sin CP directo ni de flujo completo |
| CA-47 | RNF 3.2.1 | Sin CP directo ni de flujo completo |
| CA-50 | RNF 3.2.8 | Sin CP directo ni de flujo completo |

### 6.4 Hallazgos adicionales de calidad

| ID | Hallazgo | Evidencia | Severidad | Acción |
| --- | --- | --- | --- | --- |
| H-01 | CA-60, CA-61, CP3-INT-13 y CP3-INT-14 describen la edición de una sala y figuran como "Sí" y "Pasa"; el router de salas no define modificación y la página de salas solo usa POST y DELETE. | `src/modules/salas/salas.routes.js`; `front/app/(app)/salas/page.tsx` | Alta | Verificar; registrar defecto o SCR (R-35). |
| H-02 | Los casos automatizados del repositorio usan identificadores propios (CP-INT-30 a 219, CP-UNI-01 a 48) distintos de los del plan (CP-INT, CP2-INT, CP3-INT). | `tests/*.test.js` | Media | Adoptar una sola numeración o mantener la tabla de la sección 7. |
| H-03 | `Hoja2` de `PlanPruebas_Iteracion1.xlsx` contiene CP-33 y CP-34 fuera de la hoja principal; CP-34 duplica el tema de CP-INT-08 y señala un vacío del ERS (el código de verificación no define vigencia). | `PlanPruebas_Iteracion1.xlsx` | Media | Integrar a la hoja principal o descartar; [PENDIENTE: vigencia del código definida en el ERS]. |
| H-04 | CP2-INT-23 registra "COMPORTAMIENTO SIN DEFINIR" (paciente con CURP de un paciente dado de baja) y figura como "Pasa". El repositorio rechaza la CURP de un paciente dado de baja (CP-INT-41). | `PlanPruebas_Iteracion2.xlsx`; `pacientes.test.js` | Media | Confirmar la regla con el SEAP y redactar el resultado esperado. |
| H-05 | Los CP de rendimiento (RNF de tiempo) de la Iteración 3 están en "Pasa" sin valor medido ni método. | `PlanPruebas_Iteracion3.xlsx` | Media | Registrar tiempos medidos. |
| H-06 | Las actas de las Iteraciones 1 a 3 aprueban RNF que no tienen CP (sección 6.1). | Actas | Media | Ejecutar CP no funcionales. |
| H-07 | La Iteración 4 no tiene Planeación, CA, plan de pruebas ni acta en el paquete. | Paquete | Alta | Entregar los documentos. |

## 7. Mapeo propuesto entre casos del plan y pruebas automatizadas del repositorio

El mapeo es temático y debe validarse con el Encargado SQA/ACS.

| Casos del plan | Tema | Pruebas automatizadas | Archivo |
| --- | --- | --- | --- |
| CP-INT-01 a 10 | Registro de usuarios | CP-UNI-01 a 10 | `auth.registro.test.js`, `auth.verificar.test.js` |
| CP-INT-11 a 20 | Inicio de sesión | CP-UNI-11 a 20 | `auth.login.test.js`, `auth.login-telefono.test.js` |
| CP-INT-21 a 23 | Cierre de sesión | CP-UNI-21 | `auth.logout.test.js` |
| CP-INT-24 a 29 | Recuperación y restablecimiento | CP-UNI-24 a 29 | `auth.recuperar.test.js`, `auth.restablecer.test.js` |
| CP2-INT-01 a 15 | Terapeutas | CP-INT-50 a 66 | `terapeutas.test.js` |
| CP2-INT-16 a 32 | Pacientes | CP-INT-30 a 48; CP-UNI-30 a 32 | `pacientes.test.js`, `lib.curp-fechas.test.js` |
| CP3-INT-01 a 14 | Salas | CP-INT-90 a 101 | `salas.test.js` |
| CP3-INT-15 a 29 | Creación de citas | CP-INT-110 a 123; 160 a 164 | `citas.test.js` |
| CP3-INT-20 | Correo de confirmación | CP-INT-190 a 201; CP-UNI-48 | `notificaciones.test.js` |
| CP3-INT-30 a 35 | Visualización de citas | CP-INT-130 a 135 | `citas.test.js` |
| CP3-INT-36 a 44 | Edición de citas | CP-INT-140 a 144 | `citas.test.js` |
| CP3-INT-45 a 50 | Cancelación de citas | CP-INT-150 a 153 | `citas.test.js` |
| CP3-INT-51 a 54 | Integración transversal | CP-INT-123, 170, 171, 219 | `citas.test.js`, `citas.concurrencia.test.js` |
| Sin CP en el plan | Concurrencia y anti-traslape | CP-INT-210 a 218 | `citas.concurrencia.test.js` |
| Sin CP en el plan | Seguridad, límites y migraciones | CP-INT-70 a 87; CP-UNI-33 a 39 | `auth.seguridad.test.js`, `auth.ratelimit.test.js`, `migraciones.test.js`, `middleware.test.js` |

## 8. Requerimientos de la Iteración 4 y transversales

Los identificadores de RF y CA de esta sección no existen en el paquete entregado.

| Área | Requisito | RF | CA | Implementación | Prueba o evidencia | Estado |
| --- | --- | --- | --- | --- | --- | --- |
| Agenda | Vista diaria | [PENDIENTE: RF 6.x] | [PENDIENTE: CA-79+] | `agenda.service.js` | `agenda.dashboard.test.js` | Cumple técnicamente |
| Agenda | Vista semanal | [PENDIENTE: RF 6.x] | [PENDIENTE] | `rangoDeFecha('semana')` | `CP-UNI-43`; `agenda-page.test.tsx` | Cumple técnicamente |
| Agenda | Vista mensual | [PENDIENTE: RF 6.x] | [PENDIENTE] | Conteo diario por mes | `agenda.dashboard.test.js` | Cumple técnicamente |
| Agenda | Bloques de 30 min | [PENDIENTE: RF 6.x] | [PENDIENTE] | `SLOT_MINUTOS: 30`; `slotIndex` | `CP-UNI-40`, `CP-UNI-41` | Cumple en vistas |
| Agenda | Impresión por bloques con espacios ocupados | [PENDIENTE: RF 6.x] | [PENDIENTE] | Tabla de citas | Sin prueba | No cumple |
| Agenda | Impresión con nombres ocultos | [PENDIENTE: RF 6.x] | [PENDIENTE] | Parámetro `privado` | `agenda.dashboard.test.js` (vista diaria privada) | Cumple |
| ARCO | Acceso (exportación) | [PENDIENTE: RF] | [PENDIENTE] | `GET /api/pacientes/:id/exportar` | `privacidad.admin.test.js` | Cumple |
| ARCO | Rectificación | RF 3.2.4 a 3.2.6 | CA-46 | `PUT /api/pacientes/:id` | CP2-INT-26 a 28; CP-INT-38, 39 | Cumple |
| ARCO | Cancelación (anonimización) | [PENDIENTE: RF] | [PENDIENTE] | `POST /api/pacientes/:id/anonimizar` | `privacidad.admin.test.js`; `patient-arco.test.tsx` | Cumple |
| ARCO | Oposición y revocación | [PENDIENTE: RF] | [PENDIENTE] | No encontrada | — | No cumple |
| ARCO | Consentimiento versionado | [PENDIENTE: RF] | [PENDIENTE] | `consentimiento_at`, `aviso_version` | CP-INT-44 | Cumple |
| ARCO | Aviso de privacidad | [PENDIENTE: RF] | [PENDIENTE] | `/privacidad` v1.0 | `page.test.tsx`; axe | Parcial |
| Roles | Sesión requerida en rutas privadas | RNF 3.2.7 (CP2-INT-30, confidencialidad) | [PENDIENTE] | `authenticateToken` | `router.authorization.test.js` | Cumple |
| Roles | Rol requerido para administración | [PENDIENTE: RF] | [PENDIENTE] | `requireRole`, `requirePermission` | `router.authorization.test.js`; `privacidad.admin.test.js` | Cumple |
| Roles | Registro por lista blanca | RF 1.1.6 a 1.1.8 (correo institucional) | CA-03 | `registroPolicy.js` | CP-INT-74, 75 | Cumple |
| Roles | Cambio de rol invalida sesiones | [PENDIENTE: RF] | [PENDIENTE] | `token_version` | `privacidad.admin.test.js` | Cumple |
| Roles | Baja de usuarios | [PENDIENTE: RF] | [PENDIENTE] | No encontrada | — | No cumple (R-23) |
| Auditoría | Bitácora exclusiva de administración sin PII | [PENDIENTE: RF] | [PENDIENTE] | `auditoria.routes.js` | `privacidad.admin.test.js` | Cumple |
| Calidad | Cobertura backend ≥ 85 % | [PENDIENTE: RNF] | [PENDIENTE] | Jest | 93.66 % / 94.18 % | Cumple |
| Calidad | Lógica crítica ≥ 95 % | [PENDIENTE: RNF] | [PENDIENTE] | `curp.js`, `slots.js`, `citas.service.js` | 95.34 % – 100 % | Cumple |
| Calidad | Cobertura frontend ≥ 70 % | [PENDIENTE: RNF] | [PENDIENTE] | Vitest | 31.03 % | No cumple |
| Calidad | Accesibilidad WCAG 2.1 AA | [PENDIENTE: RNF] | [PENDIENTE] | axe | `/privacidad`: 0 violaciones; resto sin auditar | Parcial |
| Calidad | Agenda con 42 citas < 500 ms | [PENDIENTE: RNF] | [PENDIENTE] | Benchmark | `agenda-page.test.tsx` | Cumple |
| Calidad | Lint y tipos sin errores | [PENDIENTE: RNF] | [PENDIENTE] | ESLint, TypeScript | `npm run lint`, `npm run typecheck` | Cumple |
| Calidad | Complejidad ciclomática ≤ 10 | [PENDIENTE: RNF] | [PENDIENTE] | ESLint | 6 funciones superiores; máximo 21 | Seguimiento |
| Calidad | Compatibilidad PostgreSQL | [PENDIENTE: RNF] | [PENDIENTE] | `scripts/test-postgres.js` | No ejecutada | Pendiente |
| Despliegue | Entorno de producción validado | [PENDIENTE: RNF] | [PENDIENTE] | Variables en `env.js` | Sin validar | Pendiente |

## 9. Plan de cierre de brechas

| ID | Acción | Brechas que cierra | Responsable | Fecha propuesta |
| --- | --- | --- | --- | --- |
| T-01 | Diseñar y ejecutar CP no funcionales para los RNF de la sección 6.1 | 6.1, H-05, H-06 | Equipo de Desarrollo | 12/11/2026 |
| T-02 | Incorporar a los CA los requerimientos de la sección 6.2 | 6.2 | Jaqueline Góngora Tun | 11/11/2026 |
| T-03 | Verificar la edición de salas | H-01 | Jaqueline Góngora Tun | 10/11/2026 |
| T-04 | Unificar numeración de CP o validar el mapeo de la sección 7 | H-02 | Jaqueline Góngora Tun | 12/11/2026 |
| T-05 | Entregar RF 6.x, CA-79 en adelante, plan de pruebas y acta de la Iteración 4 | H-07, sección 8 | Luisa Cristina Villanueva Díaz | 11/11/2026 |
| T-06 | Resolver la regla de CP2-INT-23 y la vigencia del código de verificación | H-03, H-04 | Jaqueline Góngora Tun | 11/11/2026 |
| T-07 | Definir mecanismos de oposición, revocación y baja de usuarios | Sección 8 | Jaqueline Góngora Tun | 11/11/2026 |

## 10. Aprobación

| Rol | Nombre | Firma | Fecha |
| --- | --- | --- | --- |
| Líder de Proyecto | Jaqueline Góngora Tun | [PENDIENTE: firma] | [PENDIENTE: fecha] |
| Administradora de Proyecto | Luisa Cristina Villanueva Díaz | [PENDIENTE: firma] | [PENDIENTE: fecha] |
