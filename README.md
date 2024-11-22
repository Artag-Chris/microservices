
#### Dev ####

1. clonar el repositorio
2. crear o .env con base al .env.template
3. ejecutar el comando `docker compose up --build`

####

Pasos para crear los Git Submodules

    Crear un nuevo repositorio en GitHub
    Clonar el repositorio en la máquina local
    Añadir el submodule, donde repository_url es la url del repositorio y directory_name es el nombre de la carpeta donde quieres que se guarde el sub-módulo (no debe de existir en el proyecto)

git submodule add <repository_url> <directory_name>

    Añadir los cambios al repositorio (git add, git commit, git push) Ej:

git add .
git commit -m "Add submodule"
git push

    Inicializar y actualizar Sub-módulos, cuando alguien clona el repositorio por primera vez, debe de ejecutar el siguiente comando para inicializar y actualizar los sub-módulos

git submodule update --init --recursive

    Para actualizar las referencias de los sub-módulos

git submodule update --remote
