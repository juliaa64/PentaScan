# PentaScan: Digitalización y Reproducción de Partituras

PentaScan es un proyecto de Reconocimiento Óptico de Música (**OMR**) que utiliza modelos de *Deep Learning* para **digitalizar partituras** a partir de una imagen y convertirlas en un formato estructurado (XML y MID) para su posterior uso o reproducción.

---

## 🚀 Estructura del Repositorio

| Archivo/Carpeta | Descripción |
| :--- | :--- |
| `dataset/` | **Conjunto de datos** de imágenes (e.g., `redonda la`, `clave de sol`, `tempo cuatro por cuatro`) esencial para el entrenamiento del modelo OMR. |
| `PentaScan.ipynb` | Cuaderno Jupyter para procesar las imágenes del *dataset*, analizar una nueva imagen de partitura, digitalizarla y reproducir el audio. |
| `partitura_analizar.png` | Partitura que se quiere procesar para transcribirla y reproducirla. |
| `mi_partitura.xml` | Archivo para editar desde programas como MuseScore la partitura generada. |
| `mi_partitura.mid` | Archivo de audio que reproduce la partitura generada. |
| `embeddings.npz` | Embeddings generados en el procesamiento de datos, incluyendo nuestro *dataset* y el *data augmentation*. |
| `requirements.txt` | Lista de dependencias necesarias (TensorFlow, OpenCV, music21, etc.). |
| `README.md` | Este documento. |
| `LICENSE` | Licencia del proyecto PentaScan. |

---

## ⚙️ Configuración del Entorno

Para garantizar que todas las librerías de *Deep Learning* y procesamiento de audio funcionen correctamente, es fundamental crear un entorno virtual aislado.

### 1\. Requisitos Previos

Asegúrate de tener instalado en tu sistema:

*   **Python 3.10** o superior.
*   **Git**.

### 2\. Clonar el Repositorio

```bash
git clone https://github.com/juliaa64/PentaScan.git
cd PentaScan
```

### 3\. Crear un entorno virtual

Es fundamental aislar las dependencias del proyecto. Ejecuta el siguiente comando en la raíz:

```bash
python -m venv venv
```

### 4\. Activar el entorno virtual

El comando varía según tu sistema operativo:

* **macOS / Linux:**
  ```bash
  source venv/bin/activate
  ```

* **Windows (PowerShell):**
  ```powershell
  .\venv\Scripts\Activate.ps1
  ```

* **Windows (CMD):**
  ```cmd
  venv\Scripts\activate
  ```

> **Nota:** Deberías ver `(venv)` al inicio de tu línea de comandos indicando que está activo.

### 5\. Instalar dependencias

Instala todas las librerías necesarias:

```bash
pip install -r requirements.txt
```

## 💻 Ejecución del programa

Una vez instalado todo, ejecuta el programa desde el archivo PentaScan.ipynb.

