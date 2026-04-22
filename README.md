
# Informe de laboratorio: Diseño y construcción de una incubadora neonatal a escala

**Asignatura:** Instrumentación Biomédica y Biosensores  
**Programa:** Ingeniería Biomédica  
**Universidad:** Universidad Militar Nueva Granada  
**Práctica:** Laboratorio 4  
**Integrantes:** [Nombre 1], [Nombre 2], [Nombre 3]  
**Docente:** [Nombre del docente]  
**Fecha:** [Fecha]

## 1. Introducción

Las incubadoras neonatales son dispositivos biomédicos diseñados para proporcionar un entorno controlado que favorezca la supervivencia y el desarrollo adecuado del recién nacido, especialmente en casos de prematurez o bajo peso. Una de las variables más importantes en este tipo de sistemas es la temperatura, la cual debe mantenerse cercana a los 37 °C, ya que alteraciones térmicas pueden comprometer la estabilidad fisiológica del neonato.

En esta práctica se abordó el diseño y construcción de una incubadora neonatal a escala, capaz de regular la temperatura interna en un rango entre 36 °C y 37,5 °C mediante un sistema de control térmico por convección. Además, se planteó la incorporación de un sistema de medición de peso y una señalización visual mediante LEDs, con el fin de representar de manera didáctica algunas de las funciones básicas de una incubadora neonatal.

La importancia de esta práctica radica en la aplicación de conceptos de electrónica, instrumentación biomédica y sistemas de control en un contexto clínico simulado, permitiendo comprender la relevancia de mantener condiciones ambientales seguras para el paciente neonatal.

## 2. Objetivos

### 2.1 Objetivo general

Reconocer la importancia de las incubadoras neonatales en la salud del neonato.

### 2.2 Objetivos específicos

- Identificar las partes principales que componen una incubadora neonatal.
- Desarrollar un sistema que emule el modo de operación de una incubadora neonatal.
- Evaluar cómo impacta el control de variables como temperatura, humedad y flujo de aire en la salud del neonato.

## 3. Marco teórico

### 3.1 Incubadora neonatal

La incubadora neonatal es un dispositivo médico cuya función es recrear un ambiente controlado que reduzca el riesgo fisiológico en recién nacidos, en especial en prematuros. Esto implica mantener condiciones estables de temperatura y, en sistemas más avanzados, humedad, oxigenación y monitoreo continuo.

### 3.2 Control de temperatura

La regulación térmica puede implementarse mediante un sistema de lazo cerrado. En este esquema, un sensor mide la temperatura interna, dicha lectura se compara con un valor o rango de referencia, y con base en ello se activa o desactiva un actuador térmico. En esta práctica, el rango de interés se estableció entre 36 °C y 37,5 °C.

### 3.3 Medición de peso

La guía plantea la posibilidad de incorporar una galga extensiométrica o sensor de fuerza para estimar el peso del recién nacido, mostrando el resultado en una pantalla LCD o en displays de 7 segmentos. Esta variable es clínicamente importante debido a su utilidad en el seguimiento neonatal.

## 4. Materiales

### 4.1 Materiales del laboratorio

- Multímetro digital con sondas
- Osciloscopio digital
- Fuente de voltaje DC

### 4.2 Materiales del estudiante

- Computador con conexión a internet
- Software de simulación de circuitos eléctricos
- Regleta de protoboard
- Cable UTP
- Ventilador
- LM317 y LM337
- Diodo 1N4007
- Transformador 502
- Fusible e interruptor
- Puente rectificador
- Termistor
- Diodos LED
- Resistencias de varios valores
- Capacitores de 2200 µF

## 5. Procedimiento

## 5.1 Parte A

1. Se realizó una revisión bibliográfica para identificar las partes principales de una incubadora neonatal y la función de cada una.
2. Se diseñó y simuló un circuito eléctrico a modo de sistema de control de lazo cerrado, capaz de mantener la temperatura entre 36 °C y 37,5 °C.
3. Se diseñó y simuló un circuito eléctrico para medir el peso y mostrarlo mediante una pantalla LCD o displays de 7 segmentos.

## 5.2 Parte B

1. Se construyó un modelo de incubadora neonatal a escala con cubierta transparente, mecanismo de apertura y cierre, y dimensiones aproximadas acordes con la guía.
2. Se implementó un sistema de regulación térmica por convección, utilizando un ventilador y un elemento resistivo como fuente de calor.
3. Se integró un panel de tres LEDs para indicar si la temperatura se encontraba por debajo del rango, dentro del rango o por encima del rango establecido.
4. Se incorporó un sistema básico de estimación de peso.
5. Se realizó una estimación del costo del sistema desarrollado.

## 6. Evidencia del desarrollo

### 6.1 Diseño y simulación del circuito de control de temperatura

**[Insertar aquí captura de la simulación del circuito de control de temperatura]**

**Figura 1.** Simulación del sistema de control de temperatura.

### 6.2 Diseño y simulación del sistema de medición de peso

**[Insertar aquí captura de la simulación del sistema de medición de peso]**

**Figura 2.** Simulación del sistema de medición de peso.

### 6.3 Prototipo construido

**[Insertar aquí fotografía general del prototipo]**

**Figura 3.** Vista general de la incubadora neonatal a escala.

### 6.4 Detalles del montaje

**[Insertar aquí fotografías adicionales del ventilador, sistema térmico, LEDs, sensor de peso, cableado, etc.]**

**Figura 4.** Detalles internos del prototipo.

## 7. Resultados

### 7.1 Identificación de partes y funciones

Se identificaron como elementos principales del sistema: la cubierta, el sensor de temperatura, el sistema de calentamiento, el ventilador, el sistema de indicación visual y el sistema de medición de peso. Cada uno cumple una función específica dentro de la operación general de la incubadora.

| Componente | Función |
|---|---|
| [Completar] | [Completar] |
| [Completar] | [Completar] |
| [Completar] | [Completar] |

### 7.2 Resultado del sistema de control de temperatura

**[Insertar aquí la descripción de lo observado en la simulación o en el montaje]**

- Temperatura mínima observada: **[Completar]**
- Temperatura máxima observada: **[Completar]**
- Temperatura promedio: **[Completar]**
- Estado del sistema: **[Completar]**

**[Insertar aquí gráfica o tabla de temperatura vs tiempo, si la tienen]**

### 7.3 Resultado del sistema de medición de peso

**[Insertar aquí la descripción del comportamiento del sistema de peso]**

- Patrón utilizado: **[Completar]**
- Valor real: **[Completar]**
- Valor medido: **[Completar]**
- Error absoluto: **[Completar]**
- Error porcentual: **[Completar]**

### 7.4 Estimación de costos

| Componente | Cantidad | Costo unitario | Costo total |
|---|---:|---:|---:|
| [Completar] | [ ] | [ ] | [ ] |
| [Completar] | [ ] | [ ] | [ ] |
| [Completar] | [ ] | [ ] | [ ] |
| **Total** |  |  | **[Completar]** |

## 8. Análisis de resultados

### 8.1 Análisis del control de temperatura

El sistema desarrollado fue planteado para mantener la temperatura interna de la cabina dentro del intervalo de 36 °C a 37,5 °C. De manera conceptual, el prototipo representa adecuadamente el principio de control térmico en una incubadora neonatal. Sin embargo, como en esta etapa no se cuenta con mediciones experimentales completas, el análisis se basa principalmente en la lógica de funcionamiento propuesta y en la observación preliminar del montaje y la simulación.

En caso de presentarse oscilaciones o variaciones fuera del rango, estas podrían atribuirse a la respuesta del sensor, la inercia térmica del sistema, el aislamiento de la cabina o la estrategia de control utilizada. Por ello, queda pendiente una validación cuantitativa más rigurosa.

### 8.2 Análisis del sistema de peso

La medición de peso fue concebida como una funcionalidad complementaria del prototipo. Su precisión depende directamente de la calibración del sensor, el acondicionamiento de señal y la estabilidad mecánica del soporte. Dado que aún no se realizaron mediciones comparativas con un patrón conocido, este resultado debe considerarse preliminar.

### 8.3 Comparación con incubadoras comerciales

Frente a una incubadora comercial, el prototipo desarrollado presenta como principal ventaja su bajo costo y valor didáctico. No obstante, también presenta limitaciones importantes en términos de precisión, confiabilidad, alarmas, monitoreo integral, materiales certificados y cumplimiento normativo.

| Criterio | Prototipo desarrollado | Incubadora comercial |
|---|---|---|
| Control de temperatura | Básico / preliminar | Preciso y validado |
| Medición de peso | Básica / preliminar | Integrada y calibrada |
| Alarmas | No implementadas | Sí |
| Control de humedad | No implementado | Sí |
| Certificación clínica | No | Sí |
| Costo | Bajo | Alto |

## 9. Conclusiones

1. La práctica permitió comprender que la incubadora neonatal es un sistema biomédico que requiere control preciso de variables críticas, especialmente la temperatura.
2. El diseño y construcción del prototipo a escala permitió integrar conocimientos de electrónica, instrumentación y control en una aplicación biomédica concreta.
3. El sistema planteado reproduce de forma didáctica el principio básico de funcionamiento de una incubadora neonatal, aunque todavía no cuenta con la validación necesaria para comparar su desempeño con un equipo clínico real.
4. Para fortalecer el desarrollo realizado, es necesario complementar el trabajo con mediciones experimentales, calibración del sistema de peso y análisis cuantitativo del comportamiento térmico.

## 10. Preguntas para la discusión

### 10.1 ¿Qué otras variables, además de las mencionadas, son críticas en el monitoreo neonatal?

Además de la temperatura y el peso, son relevantes la humedad relativa, la saturación de oxígeno, la frecuencia respiratoria, la frecuencia cardíaca y la concentración de oxígeno en el ambiente. Estas variables permiten una supervisión más completa del estado fisiológico del neonato.

### 10.2 ¿Qué haría falta para convertir el sistema desarrollado en una incubadora neonatal real?

Sería necesario incorporar sensores clínicamente validados, alarmas de seguridad, control de humedad, monitoreo continuo, fuentes de alimentación seguras, respaldo energético, materiales certificados, aislamiento térmico adecuado y cumplimiento de normativas biomédicas.

### 10.3 ¿Qué semejanzas hay entre una incubadora neonatal y una servo-cuna?

Ambos sistemas buscan mantener condiciones térmicas adecuadas para el neonato mediante mecanismos de control. La diferencia principal es que la incubadora ofrece un entorno cerrado con mayor control del microambiente, mientras que la servo-cuna suele operar en una estructura más abierta.

## 11. Bibliografía

[1] C. G. K. Tran, A. Gibson, D. Wong, D. Tilahun, N. Selock, T. Good, et al., “Designing a low-cost multifunctional infant incubator,” *J. Lab. Autom.*, vol. 19, no. 3, pp. 332–337, Jun. 2014. https://doi.org/10.1177/2211068214530391

[2] L. Restrepo-Pérez, N. Durango-Londoño, N. E. Gómez-Suárez, F. González-Ramírez y N. Rivera-Bonilla, “Prototipo de incubadora neonatal,” *Revista Ingeniería Biomédica*, vol. 1, no. 1, pp. 55–59, 2007. Disponible en: http://www.scielo.org.co/pdf/rinbi/v1n1/v1n1a12.pdf

[3] M. van Leeuwen, O. Frauenfelder, M. Oude-Reimer, F. Camba, M. Ceccatelli, I. Hankes-Drielsma, A. Kalbér, T. Kühn y E. Silva, *European Standards of Care for Newborn Health: Temperature management in newborn infants*. European Foundation for the Care of Newborn Infants (EFCNI), Nov. 2018. Disponible en: https://newborn-health-standards.org/standards/standards-english/care-procedures/temperature-management-in-newborn-infants/

[4] R. B. Knobel-Dail, “Role of effective thermoregulation in premature neonates,” *Research and Reports in Neonatology*, vol. 4, pp. 147–156, 2014. https://doi.org/10.2147/RRN.S52377

[5] R. E. Black, S. Cousens, H. L. Johnson et al., “Global, regional, and national causes of child mortality in 2008: a systematic analysis,” *Lancet*, vol. 375, pp. 1969–1987, Jun. 2010. https://doi.org/10.1016/S0140-6736(10)60549-1
