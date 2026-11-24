# Eliminador de Zumbido de 60 Hz

**Universidad de El Salvador**  
**Facultad de Ingeniería y Arquitectura**  
**Asignatura:** Tratamiento Digital de la Señal - TDS115

### Integrantes

* Melvin Antonio Hernández Patriz
* Brian Alexander Mártir Fraile
* Donato Isaac Surio Guevara

\---

## Descripción del Proyecto

La red eléctrica en El Salvador opera a una frecuencia de 60 Hz, lo que frecuentemente induce un "zumbido" (*hum*) electromagnético en equipos de grabación de audio e instrumentos sin aislamiento o puesta a tierra adecuados\[cite: 1, 3]. Este proyecto consiste en el diseño e implementación de un filtro digital de rechazo de banda (*notch* IIR) en Python para eliminar esta interferencia específica en grabaciones de voz y música sin alterar significativamente el espectro útil del audio\[cite: 1].

## Objetivos

### Objetivo General

Eliminar la interferencia electromagnética de 60 Hz en señales de audio mediante el diseño e implementación de un filtro digital *notch* IIR en Python\[cite: 1].

### Objetivos Específicos

1. Diseñar y simular un filtro *notch* IIR centrado en 60 Hz, logrando una atenuación teórica mínima de 40 dB\[cite: 1, 3].
2. Procesar al menos 2 señales de audio (una sintética y una real) validando el comportamiento del algoritmo en Python\[cite: 1].
3. Medir la efectividad del filtrado comprobando una reducción de al menos 95% de la amplitud del pico de 60 Hz en el análisis espectral (FFT)\[cite: 1, 3].

## Alcance

* **Nivel Mínimo:** Contaminación de un audio limpio con un tono sintético de 60 Hz generado en Python, diseño del filtro *notch* y verificación de su espectro y atenuación\[cite: 1, 4].
* **Nivel Esperado:** Aplicación del algoritmo a una grabación real con zumbido inducido, mostrando el contraste del antes y después\[cite: 1, 4].
* **Extra:** Análisis del factor de calidad ($Q$)\[cite: 4].
* **Fuera de alcance:** Procesamiento en tiempo real con hardware dedicado; todo el procesamiento se realizará en diferido y 100% por software\[cite: 1, 4, 5].

## Especificaciones Técnicas y Herramientas

* **Rango de frecuencias:** Señal de audio estándar, banda vocal (20 Hz a 20 kHz)\[cite: 1].
* **Parámetros de muestreo:** Frecuencia de muestreo ($f\_s$) de 44.1 kHz y resolución de 16 bits en formato `.wav`\[cite: 1, 4].
* **Algoritmo DSP:** Filtro IIR *Notch* (biquad)\[cite: 1].
* **Software y librerías:** Python 3, `numpy`, `scipy` (`scipy.signal`) y `matplotlib`\[cite: 1, 2].

## Cronograma de Trabajo

|Fase / Semana|Actividades Principales|Estado|
|-|-|-|
|**Semana 1**|Propuesta, alcance, implicaciones, creación de repositorio y recolección de señales\[cite: 2, 5].|En progreso|
|**Semana 2**|Teoría, estado del arte, métodos y simulación inicial en Python\[cite: 2, 5].|Pendiente|
|**Semana 3**|Pruebas con grabaciones reales, mediciones finales, redacción de resultados y video\[cite: 2, 5].|Pendiente|



