# Comandos GIT

### Inicializa el repositorio

- ` git init `

### Clonar repositorio

- `git clone <https://link-con-nombre-del-repositorio>`

### Información necesaria sobre la rama actual

- `git status`

### Ver los commits

- `git log`

### Incluir los cambios del o de los archivos en tu siguiente commit

- `git add <archivo>`

### Establecer un punto de control del desarrollo

- `git commit -m "mensaje de confirmación"`
- `git commit -am "mensaje de confirmación" (Agregar todo y commit)`

### Historial de todo lo ocurrido del repositorio
- `git reflog`

###  Viajar por el tiempo

-  Sin eliminar pero está en el stage
    - `git reset --soft HEAD^` (Una posición antes del primero)
    - `git reset --soft <Hash>` (Posición del hash sacado del log)

- Sin eliminar sacando del stage
    - `git reset --mixed <hash>`

- Eliminar cambios
    - `git reset --hard <hash>`

- Regresar un cambio eliminado
    - `git reset --hard <Hash a viajar>`(Posición del Hash sacado del historial - reflog)

### Cambiar el nombre de un archivo
- `git mv <archivo.extension> <archivo.extension>`

### Eliminar archivo

-   Eliminar archivo pero sigue en el stage
    - `git rm <archivo.extension>`

### Regresar al ultimo cambio
- `git reset --hard`
- `git checkout -- .`