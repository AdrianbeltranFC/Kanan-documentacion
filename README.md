# AI-Based Mobile App for Diabetic Foot Ulcer Analysis
> Maldonado-Oclica, A. et al. (2025). AI-Based Mobile App for Segmentation and Tissue Classification on Diabetic Foot Ulcer: A Step Forward in Patient Care. In: Bellazzi, R., Juarez Herrero, J.M., Sacchi, L., Zupan, B. (eds) Artificial Intelligence in Medicine. AIME 2025. Lecture Notes in Computer Science, vol 15735. Springer, Cham. https://doi.org/10.1007/978-3-031-95841-0_47

[![License](https://img.shields.io/badge/license-All%20Rights%20Reserved-blue.svg)](#licencia)  
[![Status](https://img.shields.io/badge/status-In%20Progress-orange.svg)](#status)

---

## 📝 Descripción General
Este repositorio contiene la documentación y el código fuente de **FootLab**, la solución completa que integra:

1. **API_Kanan**: backend en Flask para segmentación y clasificación de tejidos en úlceras de pie diabético.  
2. **App Móvil**: interfaz Android/iOS que consume la API.

---

## 🚀 Características Principales
- Segmentación con **U-Net**, **ResUnet**, **U-Net++** y **DeepLabV3+**.  
- Clasificación de tejidos (granulación, fibrinoso, calloso).  
- Cálculo de métricas (área, perímetro) usando marcadores ArUco.  
- Endpoints REST documentados y ejemplos JSON.  
- Almacenamiento en Firebase (Storage y Firestore).

---

## 📂 Estructura de Carpetas
```text
/                                  # Raíz
├─ API_Kanan/                       # Código de la API (con su propio README)
│   ├─ models/
│   ├─ predicted_images/
│   ├─ sample_images/
│   ├─ utils/
│   ├─ venv/
│   ├─ .gitignore
│   ├─ README.md                    # Documentación detallada de la API
│   └─ requirements.txt
├─ docs/                            # Diagramas UML, flujogramas
├─ guide/                           # Guías de estilo y contribución
├─ src/app/                         # (Submódulo) Código de la App Móvil
├─ tests/                           # Pruebas unitarias e integración
├─ examples/                        # Capturas de pantalla y ejemplos JSON
├─ .gitignore
├─ LICENSE                          # © 2025 FootLab Project. All Rights Reserved.
└─ README.md                        # (Este archivo)
Enlace a la documentación de la API

markdown
Copiar
Editar
- **API_Kanan**: [Ver documentación completa](API_Kanan/README.md)
📊 Métricas de Rendimiento
Según Maldonado-Oclica et al. (2025):

Modelo	IoU (%)	Dice (%)	Precisión (%)	Recall (%)
U-Net	84.2	90.1	88.5	91.0
ResUnet	85.7	91.3	89.7	92.4
U-Net++	86.5	92.0	90.2	93.1
DeepLabV3+	88.1	93.8	91.5	94.6

⚙️ Instalación y Uso
Clonar el repositorio y submódulos

bash
Copiar
Editar
git clone https://github.com/AdrianbeltranFC/Kanan-documentacion.git
cd Kanan-documentacion
git submodule update --init --recursive
API_Kanan

bash
Copiar
Editar
cd API_Kanan
source venv/bin/activate
pip install -r requirements.txt
python app.py
App Móvil (si existe submódulo)

bash
Copiar
Editar
cd ../src/app
# instrucciones específicas de compilación/despliegue
Probar Endpoints

Imágenes de ejemplo: API_Kanan/sample_images/

Ejemplos de payload/respuesta: examples/

🛡️ Licencia
Este proyecto es privado y se distribuye bajo All Rights Reserved.
© 2025 FootLab Project. Todos los derechos reservados.