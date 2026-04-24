
# Informe de laboratorio: Diseño y construcción de una incubadora neonatal a escala

**Asignatura:** Instrumentación Biomédica y Biosensores   
**Universidad:** Universidad Militar Nueva Granada   
**Integrantes:** María Paula Fernandez Jiménez. Jhonathan Guevara- Juan Pablo Díaz Rocha


## 1. Introducción

Las incubadoras neonatales son dispositivos biomédicos diseñados para proporcionar un entorno controlado que favorezca la supervivencia y el desarrollo adecuado del recién nacido, especialmente en casos de prematurez o bajo peso. Una de las variables más importantes en este tipo de sistemas es la temperatura, la cual debe mantenerse cercana a los 37 °C, ya que alteraciones térmicas pueden comprometer la estabilidad fisiológica del neonato.

En esta práctica se abordó el diseño y construcción de una incubadora neonatal a escala, capaz de regular la temperatura interna en un rango entre 36 °C y 37,5 °C mediante un sistema de control térmico por convección. Además, se planteó la incorporación de un sistema de medición de peso , con el fin de representar de manera didáctica algunas de las funciones básicas de una incubadora neonatal.

La importancia de esta práctica radica en la aplicación de conceptos de electrónica, instrumentación biomédica y sistemas de control en un contexto clínico simulado, permitiendo comprender la relevancia de mantener condiciones ambientales seguras para el paciente neonatal.

## 2. Objetivos

### 2.1 Objetivo general

Reconocer la importancia de las incubadoras neonatales en la salud del neonato.

### 2.2 Objetivos específicos

- Identificar las partes principales que componen una incubadora neonatal.
- Desarrollar un sistema que emule el modo de operación de una incubadora neonatal.
- Evaluar cómo impacta el control de variables como temperatura.
- -Evaluar el peso mediante la galga extensiométrica.

## 3. Marco teórico

### 3.1 Incubadora neonatal

Una incubadora para bebés prematuros o neonatos es un equipo indispensable en una unidad de tratamiento intensivo neonatal. Consta de una cámara cerrada de material transparente que incluye un acolchado esterilizado para acostar al bebé, con calefacción por convección, filtro de aires exterior, ventanas para manipular al paciente, y diversos y sofisticados sistemas de monitoreo que incluyen control de peso, respiración, cardíaco y de actividad cerebral.

La cámara logra limitar la exposición del recién nacido a los gérmenes, y la complejidad de los equipos, permiten también diferentes tratamientos de cuidados intensivos, incluyendo terapia intravenosa, suplemento de oxígeno, soporte mecánico de la respiración y administración de fármacos.

Las incubadoras han resultado fundamentales a partir del siglo XX para lograr altas reducciones de la tasa de mortalidad infantil en todo el mundo, constituyendo uno de los parámetros claves que explican la diferencia de tasas entre países desarrollados y otros con menor nivel tecnológico.

En la actualidad existen posiciones alternativas que promueven el reemplazo de la incubadora por el llamado método canguro, incluyendo estudios efectuados en varios países que relativizan el uso de la incubadora salvo en el caso de patologías graves.

### 3.2 Termorregulación y termovigilancia

En comparación con un adulto, un bebé prematuro no dispone de mecanismos como la sudoración y los escalofríos y su metabolismo también es limitado. La única respuesta al estrés por frío es la vasoconstricción, que se observa con la Termo-monitorización. Por lo tanto, el objetivo de los cuidados de enfermería debe ser mantener al bebé dentro de su rango de "termoneutralidad" para proporcionar las mejores condiciones de crecimiento y maduración; para esto la incubadora neonatal tiene esta funci╬n de controlar la temperatura en una temperatura que vaya de 36-37.5 °C.

### 3.2.1 Control de temperatura
La medición de longitud es un indicador antropométrico de bienestar para neonatos en cuidados intensivos. Su medición precisa y seriada es clave para optimizar el diagnóstico e indicaciones nutricionales. Sin embargo, es un desafío en términos de precisión y confiabilidad.

### 3.3 Importancia de medición de peso en neonatos

La medición del peso en una incubadora neonatal es fundamental para el seguimiento clínico del recién nacido, ya que permite evaluar el crecimiento, detectar alteraciones del balance hídrico y ajustar con precisión la administración de líquidos, nutrición y medicamentos. En pacientes prematuros o de bajo peso, pequeñas variaciones ponderales pueden reflejar cambios clínicamente relevantes, por lo que el monitoreo del peso constituye un parámetro esencial de seguridad y de toma de decisiones

### 3.3.1 Medición de peso

La guía plantea la posibilidad de incorporar una galga extensiométrica o sensor de fuerza para estimar el peso del recién nacido, mostrando el resultado en una pantalla LCD , OLED o en displays de 7 segmentos. Esta variable es clínicamente importante debido a su utilidad en el seguimiento neonatal.

## 4. Materiales

### 4.1 Materiales del laboratorio

- Multímetro digital con sondas
  
- Osciloscopio digital
  
- Fuente de voltaje DC

### 4.2 Materiales del estudiante

- Computadores con conexión a internet
- Software de simulación de circuitos eléctricos
- Cable UTP
- Ventilador
- Transformador 502
- Puente rectificador
- Termistor
- Resistencias de varios valores
- Capacitores de 2200 µF
- Galga extensiometrica junto con módulo HX711.
- Bombillo
- Relé
- Pantalla OLED
- Arduino UNO
- ESP32
- Caja que asemeja incubadora.

## 5. Procedimiento

## 5.1 Parte A

1. Se realizó una revisión bibliográfica para identificar las partes principales de una incubadora neonatal y la función de cada una.
2. Se diseñó y simuló un circuito eléctrico a modo de sistema de control de lazo cerrado, capaz de mantener la temperatura entre 36 °C y 37,5 °C.
3. Se diseñó y simuló un circuito eléctrico para medir el peso y mostrarlo mediante una pantalla OLED.

## 5.2 Parte B

1. Se construyó un modelo de incubadora neonatal a escala con cubierta transparente, mecanismo de apertura y cierre, y dimensiones aproximadas acordes con la guía.
2. Se implementó un sistema de regulación térmica por convección, utilizando un ventilador y un elemento resistivo como fuente de calor.
3. Se incorporó un sistema básico de estimación de peso.
4. Se realizó una estimación del costo del sistema desarrollado.

## 6. Evidencia del desarrollo

### 6.1 Diseño y simulación del circuito de control de temperatura

n el prototipo de incubadora se empleó un controlador ON/OFF para regular la temperatura interna. El principio de funcionamiento consiste en encender la fuente de calor cuando la temperatura medida es menor al valor mínimo deseado, y apagarla cuando supera el valor máximo establecido. Así, el sistema no mantiene una temperatura exactamente constante en un solo punto, sino dentro de un intervalo de control. En este caso, por ejemplo, el calefactor se enciende cuando la temperatura baja de 35 °C y se apaga cuando supera los 37 °C, permitiendo conservar un ambiente térmico adecuado dentro de la incubadora.
A continuación, se encuentra el diagrama de bloques de la planta y el controlador:

<img width="766" height="493" alt="image" src="https://github.com/user-attachments/assets/8adfc4db-0db7-4b73-872b-d0fe43b8d389" />

**Figura 1.** Simulación del sistema de control de temperatura.

En la siguiente imagen puede observarse un diagrama que corresponde a la lógica de decisión del controlador térmico, donde la entrada u es la temperatura medida dentro de la incubadora.

A partir de esa señal se hacen tres evaluaciones:

Se compara si la temperatura es mayor o igual que Tmin

Se compara si la temperatura es menor o igual que Tmax

y luego ambas condiciones se combinan con una compuerta AND

Eso significa que el sistema está verificando si la temperatura está dentro de la banda de operación definida por los límites:

Tmin = temperatura mínima permitida

Tmax = temperatura máxima permitida

Qué sale del diagrama

El bloque genera tres salidas:

-Tmin

-Tmax

-Una señal lógica que vale 1 si la temperatura está dentro del rango y 0 si está fuera del rango

Los bloques double solo convierten esas señales al tipo numérico para poder visualizarlas o usarlas en Simulink sin problemas de tipo de dato.

## Interpretación física

Ese bloque no está calentando todavía por sí solo; más bien está diciendo:

si la temperatura está dentro del intervalo permitido, el sistema reconoce que la incubadora está en una condición aceptable,
si sale del intervalo, se detecta una condición de desviación térmica.

<img width="980" height="495" alt="image" src="https://github.com/user-attachments/assets/53fc0d4d-d56e-4c1c-a374-8cb37f68e15c" />


**Figura 2.** Simulación del sistema de control de temperatura.

En conjunto, los dos diagramas muestran un sistema de control de temperatura para incubadora neonatal basado en una estrategia ON/OFF. El primer diagrama se encarga de verificar si la temperatura medida permanece dentro de un rango definido entre Tmin y Tmax, mientras que el segundo integra esta lógica con el modelo dinámico térmico de la incubadora, considerando la referencia de temperatura, la acción del actuador y la influencia de la temperatura ambiente. De esta manera, el sistema permite mantener la temperatura interna en una banda adecuada de operación, evitando tanto el enfriamiento como el sobrecalentamiento.

<img width="696" height="623" alt="image" src="https://github.com/user-attachments/assets/cc5e24f6-b7dc-42cd-85b3-001b3bfd65e2" />

**Figura 3.** Resúesta de simulación del sistema de control de temperatura.

A continuación se puede observar el código utilizado donde están los parámetros del controlador:

```
%% PARAMETROS INCUBADORA - CONTROL ON/OFF CON RELAY

clear; clc;

% Requisitos de la guia
Tmin = 36.0;              % [°C]
Tmax = 37.5;              % [°C]
Tref = 37.0;              % [°C]

% Condiciones termicas
Tamb = 24.0;              % [°C]
T0   = 24.0;              % [°C]

% Planta termica de primer orden
tau  = 220;               % [s]
Kcal = 0.07;              % [°C/s] por unidad de control

% Entrada al Relay: e = Tref - T
% Enciende cuando T <= 36  -> e >= 1.0
% Apaga   cuando T >= 37.5 -> e <= -0.5
relay_on  = Tref - Tmin;   % = 1.0
relay_off = Tref - Tmax;   % = -0.5

% Salida del relay
u_on  = 1;                 % calefactor encendido
u_off = 0;                 % calefactor apagado

% Perturbacion externa
t_pert_ini = 900;          % [s]
t_pert_fin = 960;          % [s]
pert_amp   = -0.03;        % [°C/s]

% Simulacion
t_sim = 1800;              % [s]
```

### 6.2 Diseño y simulación del sistema de medición de peso

En la siguiente imagen puede observarse una simulación del circuito de medición de peso:

<img width="1024" height="359" alt="image" src="https://github.com/user-attachments/assets/712a7f59-ab80-4ffc-829c-fed1b15e4454" />


**Figura 4.** Respuesta de simulación del sistema de control de temperatura.

El código utilizado para realizar la sección de medición de peso fue el siguiente programado en ARDUINO IDE con un microcontrolador Arduino UNO. Se usó una galga extensiométrica de 5 kg junto con su módulo HX711 y los datos se visualizaron en una pantalla OLED.

```
include <Wire.h>
#include <Adafruit_GFX.h>
#include <Adafruit_SSD1306.h>
#include <DFRobot_HX711.h>

#define SCREEN_WIDTH 128
#define SCREEN_HEIGHT 64
#define OLED_RESET -1

Adafruit_SSD1306 display(SCREEN_WIDTH, SCREEN_HEIGHT, &Wire, OLED_RESET);
DFRobot_HX711 balanza(3, 2);   // DT=3, SCK=2

long offset = 0;
float calibracion = 1992.0;    // luego la ajustas fino

float pesoFiltrado = 0.0;
float alpha = 0.35;            // entre más alto, más rápido responde

float leerPesoRapido(int n) {
  float suma = 0;
  for (int i = 0; i < n; i++) {
    suma += balanza.readWeight();
    delay(8);
  }
  return suma / n;
}

void setup() {
  Serial.begin(9600);
  delay(1000);

  if (!display.begin(SSD1306_SWITCHCAPVCC, 0x3C)) {
    while (1);
  }

  display.clearDisplay();
  display.setTextColor(SSD1306_WHITE);
  display.setTextSize(1);
  display.setCursor(0, 20);
  display.println("Iniciando...");
  display.display();
  delay(1500);

  display.clearDisplay();
  display.setCursor(0, 10);
  display.println("Sin peso");
  display.println("Haciendo tara...");
  display.display();

  delay(3000);

  offset = balanza.averageValue(10);   // menos muestras = mas rapido
  balanza.setOffset(offset);
  balanza.setCalibration(calibracion);

  pesoFiltrado = 0.0;

  display.clearDisplay();
  display.setCursor(0, 20);
  display.println("Balanza lista");
  display.display();
  delay(1000);
}

void loop() {
  float peso = leerPesoRapido(3);

  // invierte solo si tu lectura esta al reves
  peso = -peso;

  // zona muerta cerca de cero para eliminar negativos pequenos
  if (peso > -3.0 && peso < 3.0) {
    peso = 0.0;
  }

  // filtro exponencial: estable pero mas rapido
  pesoFiltrado = alpha * peso + (1.0 - alpha) * pesoFiltrado;

  // evita que muestre basura cerca de cero
  if (pesoFiltrado > -2.0 && pesoFiltrado < 2.0) {
    pesoFiltrado = 0.0;
  }

  Serial.print("Peso: ");
  Serial.print(pesoFiltrado, 1);
  Serial.println(" g");

  display.clearDisplay();
  display.setTextSize(1);
  display.setCursor(0, 0);
  display.println("PESO");

  display.setTextSize(3);
  display.setCursor(8, 25);
  display.print(pesoFiltrado, 1);
  display.print(" g");

  display.display();

  delay(60);
}
```

<img width="900" height="1600" alt="image" src="https://github.com/user-attachments/assets/e27c6b1b-a6b1-44b3-808a-6e7b9c7b59e2" />

**Figura 5.** Circuito montado del sistema de medición de peso.

### 6.3 Prototipo construido

<img width="1280" height="960" alt="image" src="https://github.com/user-attachments/assets/7d7df6d4-5f64-439d-aedf-9b408e8390d2" />

**Figura 6.** Vista general de la incubadora neonatal a escala.


## 7. Resultados

### 7.1 Identificación de partes y funciones

Se identificaron como elementos principales del sistema: la cubierta, el sensor de temperatura, el sistema de calentamiento, el ventilador, el sistema de indicación visual y el sistema de medición de peso. Cada uno cumple una función específica dentro de la operación general de la incubadora.

| Componente | Función |
|---|---|
| Sensor de temeratura | cumple la función de medir continuamente la temperatura interna de la incubadora. Esta medición permite conocer el estado térmico del sistema en tiempo real y sirve como variable de entrada para el controlador, el cual decide si es necesario activar o desactivar el sistema de calentamiento.|
| Sistema de calentamiento | es el encargado de suministrar la energía térmica necesaria para elevar o mantener la temperatura dentro de los valores requeridos. Su función principal es compensar las pérdidas de calor hacia el ambiente y garantizar que el interior de la incubadora conserve condiciones adecuadas para el neonato. |
| Sistema de medición de peso | se encarga de determinar el peso del neonato o de la carga ubicada en la incubadora. Esta función es importante porque permite hacer seguimiento al crecimiento, controlar variaciones de masa y apoyar la vigilancia clínica del paciente sin retirarlo innecesariamente del entorno controlado. |
|Sistema de indicación visual |permite mostrar al usuario variables importantes del funcionamiento, como la temperatura y el peso medido. Su función es facilitar la supervisión del estado de la incubadora de manera rápida y directa, sin necesidad de equipos externos de monitoreo.|
|Ventilador|tiene como función distribuir de manera uniforme el aire caliente dentro de la incubadora. Esto evita zonas con temperaturas desiguales y mejora la homogeneidad térmica en todo el habitáculo, favoreciendo un ambiente más estable.|

### 7.2 Resultado del sistema de control de temperatura

En la siguiente imagen puede observarse las temperaturas medidas por el termistor dentro de la incubadora donde se puede ibservar que en los rangos se enciende el bonnbilllo, si pasa el ranfo se apagará.

<img width="739" height="646" alt="image" src="https://github.com/user-attachments/assets/a4c1f46f-90a5-4e22-8d5f-f193ba5ae28b" />

**Figura 7.** Valores en monitor serial.

- Temperatura mínima observada: 35.0
- Temperatura máxima observada: 38.6
- Temperatura promedio:36.8
  
### 7.3 Resultado del sistema de medición de peso

- Valor real: 250 g
- Valor medido: 200 g
- Error absoluto: 50g
- Error porcentual: 20%
  
Durante la prueba de calibración del sistema de medición de peso se utilizó un patrón de 250 g, obteniéndose una lectura de 200 g. Esto corresponde a un error absoluto de 50 g y un error porcentual del 20 %. Aunque el sistema logró detectar y registrar la carga aplicada, los resultados evidencian que aún existe una desviación considerable respecto al valor real, por lo que se hace necesario realizar un ajuste más preciso del factor de calibración y mejorar las condiciones mecánicas del montaje para aumentar la exactitud de la medición

<img width="960" height="1280" alt="image" src="https://github.com/user-attachments/assets/984feab1-005d-42fb-85d9-eacf95982a31" />

**Figura 8.** Valores en monitor serial.

### 7.4 Estimación de costos

## Estimado de costos del prototipo de incubadora neonatal

En la siguiente, se presenta un estimado aproximado de los costos de los materiales empleados en la construcción del prototipo:

| Material | Costo aproximado (COP) |
|---|---:|
| Software de simulación de circuitos eléctricos | Gratuito |
| Cable UTP | 5.000 – 10.000 |
| Ventilador | 15.000 – 30.000 |
| Transformador 502 | 12.000 – 25.000 |
| Puente rectificador | 2.000 – 6.000 |
| Termistor | 2.000 – 8.000 |
| Resistencias de varios valores | 3.000 – 10.000 |
| Capacitores de 2200 µF | 4.000 – 10.000 |
| Galga extensiométrica con módulo HX711 | 16.000 – 22.000 |
| Bombillo | 3.000 – 8.000 |
| Relé | 8.000 – 15.000 |
| Pantalla OLED | 15.000 – 20.000 |
| Arduino UNO | 37.000 – 48.000 |
| ESP32 | 25.000 – 40.000 |
| Caja que asemeja incubadora | 20.000 – 60.000 |

### Total estimado

- **Costo mínimo aproximado:** 167.000 COP  
- **Costo máximo aproximado:** 312.000 COP  

El costo total del prototipo puede variar dependiendo de la disponibilidad de los materiales, la tienda donde se adquieran los componentes y si algunos de ellos ya se encuentran disponibles previamente en el laboratorio o lugar de trabajo. Este presupuesto corresponde a un valor estimado para fines académicos y de desarrollo del montaje.

## 8. Análisis de resultados

## 8.1 Análisis del control de temperatura

Los resultados térmicos muestran que el prototipo logró cumplir de manera parcial el objetivo de mantener un ambiente cercano al rango requerido para una incubadora neonatal. El valor promedio de 36.8 °C indica que el sistema operó alrededor del intervalo deseado, lo cual evidencia que la estrategia ON/OFF fue funcional para una aplicación académica básica. Sin embargo, la presencia de una temperatura mínima de 35.0 °C y una máxima de 38.6 °C demuestra que la regulación aún presentó oscilaciones importantes y sobrepasos respecto al rango planteado. Este comportamiento era esperable, ya que el control ON/OFF no corrige de manera continua, sino que conmuta entre encendido y apagado, generando variaciones alrededor de la referencia. Además, la respuesta del sistema estuvo influenciada por la inercia térmica de la cámara, la capacidad del elemento calefactor, la circulación de aire y las pérdidas de calor hacia el ambiente. En consecuencia, aunque el prototipo representa adecuadamente el principio de termorregulación, su desempeño todavía está lejos de la estabilidad y precisión requeridas en una incubadora neonatal real.

## 8.2 Análisis del sistema de peso

En el sistema de medición de peso, el error porcentual del 20 % evidencia que el montaje fue funcional, pero todavía insuficiente en términos de exactitud. El hecho de que el sistema registrara 200 g para un patrón de 250 g confirma que la celda de carga, el módulo HX711 y la visualización en OLED operaron correctamente a nivel básico; sin embargo, la diferencia de 50 g revela problemas de calibración y posibles limitaciones mecánicas en el soporte de la galga. En este tipo de sistemas, la precisión depende no solo del factor de calibración programado, sino también de la rigidez estructural, la correcta fijación de la celda y la reducción de vibraciones o deformaciones parásitas. Por ello, el resultado obtenido debe interpretarse como una validación funcional del principio de medición, pero no como una medición suficientemente precisa para una aplicación clínica. Para mejorar el desempeño sería necesario repetir la calibración con varios patrones conocidos, ajustar el montaje mecánico y verificar la linealidad de la respuesta del sensor.

## 8.3 Comparación con incubadoras comerciales

Frente a una incubadora neonatal comercial, el prototipo desarrollado presenta un valor principalmente formativo y experimental. Su principal fortaleza es haber permitido integrar en un solo montaje conceptos de control térmico, instrumentación, sensado y visualización, utilizando componentes de bajo costo y fácil acceso. No obstante, las diferencias con un equipo clínico real son sustanciales. Mientras una incubadora comercial incorpora control térmico altamente preciso, sensores validados, alarmas, monitoreo continuo, control de humedad, materiales certificados y condiciones de seguridad biomédica, el prototipo construido se limita a reproducir de forma simplificada dos funciones básicas: regulación térmica y estimación de peso. Por tanto, el sistema desarrollado no puede considerarse un sustituto de una incubadora real, sino una aproximación académica útil para comprender sus principios de funcionamiento y reconocer las exigencias técnicas que implica su implementación en un contexto clínico.

## 9. Conclusiones

1.El desarrollo del prototipo permitió comprender que una incubadora neonatal no se limita a suministrar calor, sino que constituye un sistema biomédico en el que deben integrarse medición, control y supervisión de variables críticas para garantizar condiciones adecuadas de soporte al neonato.

2.El sistema de control térmico implementado mediante una estrategia ON/OFF logró mantener la temperatura de la incubadora en un entorno cercano al rango de operación propuesto, con un valor promedio de 36.8 °C. Sin embargo, las variaciones observadas entre 35.0 °C y 38.6 °C evidencian que, aunque el principio de regulación fue funcional, todavía existen oscilaciones y sobrepasos que limitan la precisión del sistema.

3.El sistema de medición de peso permitió detectar y visualizar la carga aplicada mediante una galga extensiométrica, un módulo HX711 y una pantalla OLED, lo que confirma la viabilidad de incorporar esta variable al prototipo. No obstante, la medición obtenida para el patrón de 250 g presentó un error porcentual del 20 %, por lo que el sistema aún requiere una calibración más rigurosa y mejoras mecánicas para aumentar su exactitud.

4.Desde el punto de vista académico, el montaje cumplió con el propósito de representar de forma didáctica las funciones básicas de una incubadora neonatal a escala, integrando conocimientos de electrónica, sensores, acondicionamiento de señal, microcontroladores y control térmico en una sola aplicación.

5.A pesar de su funcionalidad básica y de su bajo costo, el prototipo presenta limitaciones importantes frente a una incubadora neonatal comercial, especialmente en precisión, estabilidad, confiabilidad, alarmas, control de humedad y validación clínica. Por ello, debe entenderse como un desarrollo experimental y formativo, no como un dispositivo apto para uso médico real.

6.Como trabajo futuro, se recomienda optimizar la calibración del sistema de peso, mejorar el montaje estructural de la celda de carga, reducir las oscilaciones térmicas del control ON/OFF y complementar el prototipo con funciones adicionales como alarmas, monitoreo de humedad y una validación experimental más rigurosa de todas las variables medida

## 10. Preguntas para la discusión

### 10.1 ¿Qué otras variables, además de las mencionadas, son críticas en el monitoreo neonatal?

Además de la temperatura y el peso, son relevantes la humedad relativa, la saturación de oxígeno, la frecuencia respiratoria, la frecuencia cardíaca y la concentración de oxígeno en el ambiente. Estas variables permiten una supervisión más completa del estado fisiológico del neonato.

### 10.2 ¿Qué haría falta para convertir el sistema desarrollado en una incubadora neonatal real?

Sería necesario incorporar sensores clínicamente validados, alarmas de seguridad, control de humedad, monitoreo continuo, fuentes de alimentación seguras, respaldo energético, materiales certificados, aislamiento térmico adecuado y cumplimiento de normativas biomédicas.

### 10.3 ¿Qué semejanzas hay entre una incubadora neonatal y una servo-cuna?

Ambos sistemas buscan mantener condiciones térmicas adecuadas para el neonato mediante mecanismos de control. La diferencia principal es que la incubadora ofrece un entorno cerrado con mayor control del microambiente, mientras que la servo-cuna suele operar en una estructura más abierta en el que se puede dar manejos en el caso de realizar reanimación o algún procedimiento donde se necesite tener acceso completo al neonato.

## 11. Bibliografía

[1] C. G. K. Tran, A. Gibson, D. Wong, D. Tilahun, N. Selock, T. Good, et al., “Designing a low-cost multifunctional infant incubator,” *J. Lab. Autom.*, vol. 19, no. 3, pp. 332–337, Jun. 2014. https://doi.org/10.1177/2211068214530391

[2] L. Restrepo-Pérez, N. Durango-Londoño, N. E. Gómez-Suárez, F. González-Ramírez y N. Rivera-Bonilla, “Prototipo de incubadora neonatal,” *Revista Ingeniería Biomédica*, vol. 1, no. 1, pp. 55–59, 2007. Disponible en: http://www.scielo.org.co/pdf/rinbi/v1n1/v1n1a12.pdf

[3] M. van Leeuwen, O. Frauenfelder, M. Oude-Reimer, F. Camba, M. Ceccatelli, I. Hankes-Drielsma, A. Kalbér, T. Kühn y E. Silva, *European Standards of Care for Newborn Health: Temperature management in newborn infants*. European Foundation for the Care of Newborn Infants (EFCNI), Nov. 2018. Disponible en: https://newborn-health-standards.org/standards/standards-english/care-procedures/temperature-management-in-newborn-infants/

[4] R. B. Knobel-Dail, “Role of effective thermoregulation in premature neonates,” *Research and Reports in Neonatology*, vol. 4, pp. 147–156, 2014. https://doi.org/10.2147/RRN.S52377

[5] R. E. Black, S. Cousens, H. L. Johnson et al., “Global, regional, and national causes of child mortality in 2008: a systematic analysis,” *Lancet*, vol. 375, pp. 1969–1987, Jun. 2010. https://doi.org/10.1016/S0140-6736(10)60549-1
