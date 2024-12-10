# Curso para Importadores

## Instrucciones

1. Crear un entorno de python

   - PowerShell
  
    ```PowerShell
    PS C:\<carpeta projecto>python -m venv <nombre del entorno>
    ```

   - CMD

    ```cmd
    C:\Users\Usuario>python -m venv <nombre del entorno>
    ```

   - Linux - Mac

    ```bash
    user@pc:/home/<carpeta projecto>$ python3 -m venv <nombre del entorno>
    ```

2. Activar el entono

   - PowerShell
  
    ```PowerShell
    PS C:\user\Usuario\<carpeta> .\<entorno>\Script\activate.ps1

    (<entorno>)PS C:\user\Usuario\<carpeta>
    ```

   - CMD

    ```cmd
    C:\Users\Usuario\<carpeta>\<entorno>\Script\activate

    (entorno) C:\Users\Usuario\<carpeta>\<entorno>\Script>
    ```

   - Linux - Mac

    ```bash
    user@pc:/home/source ./<carpeta>/<entorno>/bin/activate

    (entorno) user@pc:/home$
    ```

3. Instalar Dependencias

    Con el entorno activado executar

    ```bash
    python -m pip install -r requirements.txt   
    ```

4. Executar el servicio

    ```PowerShell
    (entorno) PS F:\Curso importadores> python .\web.py
    * Serving Flask app 'web'
    * Debug mode: on
    Escribe 'salir' para apagar el servidor
    ```

    > Nota : No cerrar la ventana mientras se usa

   - Para terminar el proceso ingresar `salir`
   - Para desactivar el entorno en Cualquier caso usar `deactivate`

    ```PowerShell
    Escribe 'salir' para apagar el servidor: salir
    Apagando el servidor...
    (entorno) PS F:\Curso importadores> deactivate
    PS F:\Curso importadores>
    ```

> Nota Importante:
> Para que funcionen deben crear un archivo .env con la api key de openai

>```bash
>OPENAI_API_KEY = <Tu api key valida>
>```
