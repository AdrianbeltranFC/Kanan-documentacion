# AI-Based Mobile App for Diabetic Foot Ulcer Analysis 
**Para citar:**   
> Maldonado-Oclica, A. et al. (2025). AI-Based Mobile App for Segmentation and Tissue Classification on Diabetic Foot Ulcer: A Step Forward in Patient Care. In: Bellazzi, R., Juarez Herrero, J.M., Sacchi, L., Zupan, B. (eds) Artificial Intelligence in Medicine. AIME 2025. Lecture Notes in Computer Science, vol 15735. Springer, Cham. <https://doi.org/10.1007/978-3-031-95841-0_47>

[![Licencia](https://img.shields.io/badge/licencia-Todos%20los%20derechos%20reservados-blue.svg)](#licencia)
[![Estado](https://img.shields.io/badge/estado-En%20progreso-orange.svg)](#estado)

---

## 📑 Contenidos
1. [Descripción General](#descripción-general)
2. [Ejecución de la API (API_Kanan)](#ejecucion-de-la-api-apikanan)
3. [Ejecución de la App Móvil](#ejecucion-de-la-app-movil)
4. [Estructura de Carpetas](#estructura-de-carpetas)
5. [Métricas de Rendimiento](#métricas-de-rendimiento)
6. [Resultados de la App Móvil](#resultados-de-la-app-movil)
7. [Licencia](#licencia)

---

## 📝 Descripción General
Este repositorio contiene la documentación y el código fuente de **Kanan**, que integra dos componentes principales:

1. **API_Kanan**: backend en Flask para segmentación y clasificación de tejidos en úlceras de pie diabético.  
2. **App_Móvil**: interfaz Android que se conecta con la API para mostrar los resultados en tiempo real.

---

## Ejecución de la API (API_Kanan)

> **Nota importante:** La API de Kanan se encuentra en un submódulo externo.  
> Para poder utilizarla correctamente, primero debes clonar este repositorio con la opción de submódulos:

```bash
# Clonar el repositorio principal con submódulos
git clone --recurse-submodules https://github.com/AdrianbeltranFC/Kanan-documentacion.git

# Entrar en la carpeta del repositorio
cd Kanan-documentacion

# Si ya clonaste sin --recurse-submodules, inicializa y actualiza los submódulos manualmente
git submodule init
git submodule update
```

La documentación completa y los pasos de ejecución de la API se encuentran en su propio archivo.

---

## Ejecución de la APP Móvil
En construcción. Pronto estará disponible la documentación.
---

## 🚀 Características Principales
- Segmentación con **U-Net**, **ResUnet**, **U-Net++** y **DeepLabV3+**.  
- Clasificación de tejidos (granulación, fibrinoso, calloso).  
- Cálculo de métricas (área, perímetro) usando marcadores ArUco.  
- Endpoints documentados y ejemplos JSON de la API.
- Almacenamiento en Firebase.

---

## 📂 Estructura de Carpetas
```text
/                                  # Raíz
├─ API_Kanan/                      # Código de la API (con su propio README)
│   ├─ models/
│   ├─ predicted_images/
│   ├─ sample_images/
│   ├─ utils/
│   ├─ venv/
│   ├─ .gitignore
│   ├─ README.md                   # Documentación detallada de la API
│   └─ requirements.txt
├─ docs/                           # documentación técnica
├─ src/app/                        # (Submódulo) Código de la App Móvil
├─ tests/                          # Pruebas unitarias e integración
├─ examples/                       # Capturas de pantalla y ejemplos JSON
├─ .gitignore
├─ LICENSE                         # © 2025 FootLab Project. All Rights Reserved.
└─ README.md                       # (Este archivo)
```
---

## 📊 Métricas de Rendimiento
| Modelo | IoU (%) | Dice (%) | Precisión (%) | Recall (%) |
|:-------|:--------|:---------|:--------------|:-----------|
| U-Net | 84.2 | 90.1 | 88.5 | 91.0 |
| ResUnet | 85.7 | 91.3 | 89.7 | 92.4 |
| U-Net++ | 86.5 | 92.0 | 90.2 | 93.1 |
| DeepLabV3+ | 88.1 | 93.8 | 91.5 | 94.6 |

---

## 📷 Resultados de la App Móvil
<p float="left"> <img src="examples/app_result1.jpeg" alt="Interfaz: resultados de la clasificación con los porcentajes de coloración, tamaño de la herida, perímetro y la imagen anotada" width="48%" /> <img src="examples/app_result2.jpeg" alt="Interfaz: Resultados de la segmentación con los porcentajes de cada tejido respecto a la fotografía y el tamaño de cada uno en unidades reales" width="48%" /> </p>
Figuras 1 y 2. Interfaz de la app mostrando:

Resultados de la clasificación de la úlcera (izquierda). 
Resultados de la segmentación (derecha). 

---

## 🔗 Licencia
Estado: En progreso.
Este proyecto es privado y se distribuye bajo All Rights Reserved.
© 2025 Kanan Project. Todos los derechos reservados.