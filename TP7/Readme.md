# Análisis del Audio – Práctica

Este proyecto corresponde a la práctica de **Técnicas para el Análisis del Audio**   
El objetivo es analizar un archivo de audio (`AnalisisTextos.mp3`) utilizando **MediaInfo**, **ffmpeg** y **Python**, aplicando transformaciones y verificando sus efectos.

---

## 📖 Contenido

1. **Análisis inicial con MediaInfo**  
   - Formato: MP3  
   - Tasa de bits: 256 kb/s  
   - Canales: 1 canal (mono)  
   - Frecuencia de muestreo: 48 kHz  

2. **Sampleo con ffmpeg**  
   - Comando utilizado:  
     ```powershell
     .\ffmpeg.exe -i AnalisisTextos.mp3 -ar 22050 sampleo.wav
     ```
   - Resultado: archivo WAV (`sampleo.wav`) con frecuencia de muestreo de 22,05 kHz.

3. **Nuevo análisis con MediaInfo**  
   - Formato: PCM  
   - Tasa de bits: 352,8 kb/s  
   - Canales: 1 canal (mono)  
   - Frecuencia de muestreo: 22,05 kHz  
   - Profundidad de bits: 16 bits  
   - Duración: 7 s  

4. **Análisis con Python**  
   - Vector de la señal segmentada  
   - Cantidad de elementos de la muestra  
   - Frecuencia de muestreo  
   - Duración en segundos  
   - Gráfico de la forma de onda  
   - Reproducción del audio original  

5. **Transformaciones con Python**  
   - Cambio de frecuencia de muestreo:  
     - 11.025 Hz → audio más lento y grave  
     - 44.1 kHz → audio más rápido y agudo  
   - Reducción de calidad:  
     - Conversión a 8 bits (`uint8`) → sonido con más ruido y menor fidelidad  

---

## 📌 Requisitos

- Python 3.10+  
- Librerías:  
  - `numpy`  
  - `matplotlib`  
  - `scipy`  
  - `wave`  
  - `IPython.display`  

- Herramientas externas:  
  - [FFmpeg](https://ffmpeg.org/download.html)  
  - [MediaInfo](https://mediaarea.net/en/MediaInfo)

---

## 🚀 Ejecución

1. Analizar el archivo original con MediaInfo.  
2. Generar el archivo `sampleo.wav` con ffmpeg.  
3. Ejecutar el notebook en Jupyter para:  
   - Leer parámetros del WAV.  
   - Graficar la forma de onda.  
   - Reproducir el audio.  
   - Aplicar transformaciones de frecuencia y calidad.  

---

## 📖 Conclusiones

- **MediaInfo** permite obtener parámetros técnicos del audio.  
- **ffmpeg** transforma la frecuencia de muestreo y el formato.  
- **Python** permite analizar la señal, graficar, reproducir y modificar el audio.  
- Cambiar la frecuencia de muestreo altera la velocidad y el tono.  
- Reducir la calidad (bitrate o profundidad de bits) genera pérdida de fidelidad y más ruido.  

