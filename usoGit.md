# Aquí están los principales comandos de Git:

Aquí tienes una lista de los principales comandos de Git y sus usos, lo cual te servirá para gestionar repositorios y colaborar de forma efectiva en tus proyectos:

### 1. `git init`

Inicializa un nuevo repositorio en una carpeta existente. Crea una carpeta oculta `.git` para empezar a llevar el control de versiones.

```bash
git init
```

### 2. `git clone`

Clona un repositorio remoto y crea una copia local. Esto es útil para trabajar en un proyecto existente en GitHub o en otros servidores Git.

```bash
git clone <URL-del-repositorio>
```

### 3. `git add`

Añade archivos al área de preparación (staging area), es decir, los prepara para ser incluidos en el próximo commit.

```bash
git add <nombre-del-archivo>    # Añade un archivo específico
git add .                       # Añade todos los archivos modificados
```

### 4. `git commit`

Registra los cambios en el repositorio con un mensaje descriptivo que explique las modificaciones.

```bash
git commit -m "Mensaje que describe el cambio"
```

### 5. `git status`

Muestra el estado del repositorio, incluyendo archivos que están en el área de preparación, cambios que aún no se han preparado y archivos que no están siendo rastreados.

```bash
git status
```

### 6. `git log`

Muestra el historial de commits del repositorio, con detalles como el autor, fecha y mensaje de cada commit.

```bash
git log
```

### 7. `git branch`

Permite gestionar las ramas del repositorio. Las ramas son versiones separadas del proyecto donde puedes hacer cambios sin afectar la rama principal.

- Ver todas las ramas:

  ```bash
  git branch
  ```

- Crear una nueva rama:

  ```bash
  git branch <nombre-de-la-rama>
  ```

### 8. `git checkout`

Cambia de una rama a otra o restaura archivos en una versión específica.

- Cambiar a una rama específica:

  ```bash
  git checkout <nombre-de-la-rama>
  ```

- Crear y cambiar a una nueva rama al mismo tiempo:

  ```bash
  git checkout -b <nombre-de-la-nueva-rama>
  ```

### 9. `git merge`

Fusiona otra rama con la rama actual, integrando sus cambios. Esto se usa generalmente para combinar una rama de desarrollo con la rama principal (`main` o `master`).

```bash
git merge <nombre-de-la-rama>
```

### 10. `git pull`

Actualiza el repositorio local con los cambios del repositorio remoto. Combina `git fetch` (descargar los cambios) y `git merge` (fusionar esos cambios en la rama local).

```bash
git pull origin <nombre-de-la-rama>
```

### 11. `git push`

Sube los commits del repositorio local al repositorio remoto. Esto permite que otros colaboradores vean tus cambios.

```bash
git push origin <nombre-de-la-rama>
```

### 12. `git remote`

Gestiona las conexiones con repositorios remotos (como GitHub).

- Añadir un repositorio remoto:

  ```bash
  git remote add origin <URL-del-repositorio>
  ```

- Ver todos los repositorios remotos configurados:

  ```bash
  git remote -v
  ```

### 13. `git diff`

Muestra las diferencias entre los archivos modificados y el último commit. Esto es útil para ver exactamente qué cambios has hecho antes de confirmarlos.

```bash
git diff
```

### 14. `git stash`

Guarda temporalmente los cambios sin hacer un commit, y restaura el área de trabajo a un estado limpio. Es útil cuando necesitas cambiar de rama rápidamente pero no has terminado el trabajo actual.

- Guardar cambios:

  ```bash
  git stash
  ```

- Recuperar los cambios guardados:

  ```bash
  git stash pop
  ```

### 15. `git reset`

Revierte cambios en el historial de commits.

- Para deshacer un commit, manteniendo los cambios en el área de preparación:

  ```bash
  git reset --soft <ID-del-commit>
  ```

- Para deshacer un commit, eliminando los cambios del área de preparación:

  ```bash
  git reset --hard <ID-del-commit>
  ```

Estos comandos te permitirán trabajar en un flujo básico de Git, administrar cambios, y colaborar eficazmente en proyectos compartidos.
