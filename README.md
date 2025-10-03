### Tarea *"Manipulación y visualización avanzada de datos"*
Módulo 2 - Tarea 2
- *INICIO 00:00 25/09/2025 - CIERRE 23:59 04/10/2025*

### Materia
Programación avanzada para ciencia de datos.

### Alumno  
*Juan Pablo Dongo Huaman*

### Docente  
*Ing. Juan Carlos Cifuentes Durán*

> [!NOTE]
> ### Dataset  
> [*https://www.kaggle.com/datasets/khushikyad001/teen-phone-addiction-and-lifestyle-survey*](https://www.kaggle.com/datasets/khushikyad001/teen-phone-addiction-and-lifestyle-survey)
> 
> ### Motor de base de datos  
> *SQLite*

> [!IMPORTANT]
> ## **Extensiones necesarias para *Visual Studio Code***
> ```bash
>   Jupyter
>   Jupyter Cell Tags
>   Jupyter Keymap
>   Jupyter Notebook Renderers
>   Jupyter Slide Show
>   Pylance
>   Python
>   Python Debugger
>   Python Environments
>   (OPCIONAL) Black Formatter
> ```
> ## **Pasos para ejecutar la notebook desde *Visual Studio Code***  
> **Paso 1** - *Clonar repositorio.*  
> - **Comando** → *git clone [url_repositorio]*  
> ```bash
>   git clone https://github.com/JuanPablo-DH/PACD_M2_T2.git
> ```
> **Paso 2** - *Abrir la terminal del sistema operativo *CMD/SHELL*.*  
> - Ubicarse con el comando **CD** en la carpeta del proyecto *(donde se clonó el repositorio)*.  
> **Comando** → *cd "[path_proyecto]"*  
> ```bash
>    cd "C:\user\...\PACD_M2_T2"
> ```
> 
> **Paso 3** - *Crear un entorno virtual *(VENV)* para el proyecto.*  
> - Ejecutar desde la terminal *CMD/SHELL* **ubicada en la carpeta del proyecto**.   
> **Comando** → *py -m venv [nombre_venv]*  
> ```bash
>   py -m venv venv_M2T2
> ```
> 
> **Paso 4** - *Activar el *VENV* del proyecto. **¡¡¡ IMPORTANTE !!!***
> - Ejecutar desde la terminal CMD/SHELL ubicada en la carpeta del proyecto. 
> - Windows  
> **Comando** → *[nombre_venv]\Scripts\activate*  
> ```bash
>   venv_M2T2\Scripts\activate
> ```
> - Linux  
> **Comando** → *[nombre_venv]\bin\activate*  
> ```bash
>    venv_M2T2\bin\activate
> ```
> - Para **desactivar** el *VENV* en Windows y Linux  
> ```bash
>   deactivate
> ```
> 
> **Paso 5** - *Instalar dependencias/módulos.*  
> - Ejecutar desde la terminal *CMD/SHELL* **ubicada en la carpeta del proyecto**.
> ```bash
>   pip install -r requirements_vscode.txt
> ```
>
> **Paso 6** - *Seleccionar el kernel de la notebook.*
> - Abrir la carpeta del proyecto con **VSCode**.
> - Seleccionar el archivo **notebook_M2T2.ipynb**.
>   - Hacer click en la opción **"Select Kernel"** *(arriba a la derecha)*.
>   - Seleccionar la opción **"Python Environments..."**.
>   - Seleccionar el kernel del VENV **"venv_M2T2 (Python 3.13.7)"**. 
> ```
>   Select Kernel ⇒ Python Environments... ⇒ venv_M2T2 (Python 3.13.7)
> ```
> **Paso 7** - *Descargar el dataset.*
> - Una vez descargado el dataset.csv desde Kaggle, **ubicarlo en la carpeta del proyecto**.
>
> **Paso 8** - *Explorar la notebook mediante Visual Studio Code*.

> [!NOTE]
> ### **¿Cómo saber si está activado el *VENV*?**  
> En la terminal *CMD/SHELL* del lado izquierdo aparece entre paréntesis el nombre del *VENV*.  
> - *VSCode en la terminal powershell lo resalta de color verde.*
> 
> *VENV* Activado
> ```bash
>   (venv_M2T2) PS C:\Users\...\PACD_M2_T2> ... [comandos]
> ```
> *VENV* Desactivado
> ```bash
>   PS C:\Users\...\PACD_M2_T2> ... [comandos]
> ```

> [!CAUTION]
> ### **Posible error**  
> No se puede activar el *VENV*, porque *"El sistema tiene deshabilitado la ejecucion de scripts"*.
> ```bash
> venv_M2T2\Scripts\activate : No se puede cargar el archivo C:\Users\...\PACD_M2_T2\venv_M2T2\Scripts\Activate.ps1 porque
> la ejecución  de scripts está deshabilitada en este sistema. Para obtener más información, consulta el
> tema about_Execution_Policies en https:/go.microsoft.com/.../... .
> En línea: 1 Carácter: 1
> + venv_M2T2\Scripts\activate
> + ~~~~~~~~~~~~~~~~~~~~~~~~~~
>     + CategoryInfo          : SecurityError: (:) [], PSSecurityException
>     + FullyQualifiedErrorId : UnauthorizedAccess
> ```

> [!TIP]
> ### **Solución**  
> Ejecutar desde la terminal *CMD/SHELL* **ubicada en la carpeta del proyecto**.
> ```bash
>   Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process
> ```
> Teóricamente luego de ejecutar el comando, se debería poder activar el *VENV*.

> [!CAUTION]
> ### **Posible error**  
> A pesar de haber ejecutado el comando pip install, siguen sin reconocerse los módulos.

> [!TIP]
> ### **Solución**  
> Seleccionar el kernel del *VENV* para ejecutar las celdas de código de la notebook.
> - Se menciona en el **Paso 6**.
