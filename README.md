# Recreacion de algoritmos cuanticos

Este repositorio reúne los notebooks que he ido escribiendo mientras aprendo computación cuántica con Qiskit.

Los algoritmos que aparecen aquí no son de mi autoría. Son algoritmos públicos y bien conocidos que recreé paso a paso con fines de estudio. Mi objetivo es aprender, y subo mis notas por si a alguien más le sirven. Si quieres aprender conmigo, eres bienvenido.

Al ser material de estudio, puede contener errores o explicaciones incompletas. Si encuentras alguno, puedes abrir un issue.

## Contenido

| Notebook | Tema |
|---|---|
| `01_bell.ipynb` | Estado de Bell: superposición y entrelazamiento |
| `02_compuertas.ipynb` | Compuertas básicas y esfera de Bloch |
| `03_teletransportacion.ipynb` | Teletransportación cuántica |
| `04_superdenso.ipynb` | Codificación superdensa |
| `05_deutsch_jozsa.ipynb` | Algoritmo de Deutsch-Jozsa |
| `06_bernstein_vazirani.ipynb` | Algoritmo de Bernstein-Vazirani |
| `07_grover.ipynb` | Algoritmo de Grover |
| `08_qft.ipynb` | Transformada cuántica de Fourier |
| `09_qpe.ipynb` | Estimación de fase cuántica |

## Requisitos

- Python 3.10 o superior
- Git

Todo se ejecuta en el simulador local (Qiskit Aer), así que no necesitas cuenta ni acceso a hardware cuántico.

## Preparar el entorno

1. Descarga el repositorio:

```bash
git clone https://github.com/sanickg/Recreacion-algoritmos-cuanticos.git
cd Recreacion-algoritmos-cuanticos
```

2. Crea un entorno virtual para no mezclar las librerías con otros proyectos:

```bash
python -m venv .venv
```

3. Actívalo:

```powershell
# Windows (PowerShell)
.venv\Scripts\Activate.ps1
```

```bash
# Linux o macOS
source .venv/bin/activate
```

Si PowerShell bloquea la ejecución de scripts, ejecuta esto una sola vez y vuelve a intentar:

```powershell
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
```

En Windows con CMD, el comando de activación es `.venv\Scripts\activate.bat`.

4. Instala las librerías:

```bash
pip install -r requirements.txt
```

## Ejecutar los notebooks

Con el entorno activo, dentro de la carpeta del proyecto:

```bash
jupyter lab
```

Se abrirá en el navegador. Abre el notebook que quieras y ejecuta las celdas en orden (menú Run > Run All Cells).

Los notebooks también se pueden leer directamente en GitHub, ya que guardan sus resultados y gráficas.

## Nota sobre versiones

Este código usa Qiskit 2.x. Muchos tutoriales antiguos usan `execute()` o `from qiskit import Aer`, que ya no existen en esta versión. En su lugar se utiliza `AerSimulator().run(...)`. Por eso `requirements.txt` fija las versiones con las que se probó todo.

## Recursos para seguir aprendiendo

- [IBM Quantum Learning](https://quantum.cloud.ibm.com/learning)
- [Documentación de Qiskit](https://docs.quantum.ibm.com)