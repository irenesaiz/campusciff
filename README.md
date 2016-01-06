# Práctica GIT

### 2.1 REPOSITORIO CAMPUSCIFF
Crear un repositorio en vuestro GitHub llamado campusciff.

Clonar vuestro repositorio en local.

`git clone git@github.com:irenesaiz/campusciff.git`

### 2.3 README
Crear (si no lo habéis creado ya) en vuestro repositorio local un documento README.md.
Notas: en este documento tendréis que ir poniendo los comandos que habéis tenido que utilizar durante todos los ejercicios y las explicaciones y capturas de pantalla que consideréis necesarias.
 
### 2.4 COMMIT INICIAL
Añadir al README.md los comandos utilizados hasta ahora y hacer un commit inicial con el mensaje commit inicial.

`vim README.md`
 
### 2.5 PUSH INICIAL
Subir los cambios al repositorio remoto.
```
git add .
git commit -m "commit inicial"
git push origin master
```

### 2.6 IGNORAR ARCHIVOS
1. Crear en el repositorio local un fichero llamado privado.txt.
2. Crear en el repositorio local una carpeta llamada privada.
3. Realizar los cambios oportunos para que tanto el archivo como la carpeta sean ignorados por git.

```
touch privado.txt
mkdir privada
echo privado.txt > .gitignore
cat .gitignore
echo privada >> .gitignore
cat .gitignore
```

### 2.8 AÑADIR FICHERO 1.TXT
1. Añadir fichero 1.txt al repositorio local.
```
touch 1.txt
git add .
git commit -m "Añadido gitignore y 1.txt"
```

### 2.9 CREAR EL TAG V0.1
1. Crear un tag v0.1.
``` 
git tag v0.1
```
### 2.10 SUBIR EL TAG V0.1
1. Subir los cambios al repositorio remoto.
```
git push --tag origin master
```
 
### 2.11 CREAR UNA RAMA V0.2
1. Crear una rama v0.2.
2. Posiciona tu carpeta de trabajo en esta rama.

```
git branch v0.2
git checkout v0.2
```

### 2.12 AÑADIR FICHERO 1.TXT
1. Añadir un fichero 2.txt en la rama v0.2.
```
touch 2.txt
```
### 2.13 CREAR RAMA REMOTA V0.2
1. Subir los cambios al repositorio remoto.
```
git add .
git commit -m "Añadido 2.txt"
git push origin v0.2
```

### 2.14 MERGE DIRECTO
1. Posicionarse en la rama master.
2. Hacer un merge de la rama v0.2 en la rama master.
 
```
git checkout master
git merge v0.2
```

### 2.15 MERGE CON CONFLICTO
1. En la rama master poner Hola en el fichero 1.txt y hacer commit.
```
vim 1.txt
git add .
git commit -m "Hola en 1.txt"
```

1. Posicionarse en la rama v0.2 y poner Adios en el fichero "1.txt" y hacer commit.
```
git checkout v0.2
vi 1.txt
cat 1.txt
git add .
git commit -m "Adios en 1.txt"
```

1.	Posicionarse de nuevo en la rama master y hacer un merge con la rama v0.2
```
git checkout master
git merge v0.2
```

### 2.18 LISTADO DE RAMAS
1. Listar las ramas con merge y las ramas sin merge.
 
### 2.19 ARREGLAR CONFLICTO
1. Arreglar el conflicto anterior y hacer un commit.

 
 
### 2.20 BORRAR RAMA
1. Crear un tag v0.2
2. Borrar la rama v0.2
 
### 2.21 LISTADO DE CAMBIOS
1. Listar los distintos commits con sus ramas y sus tags.
 
### 2.22 CUENTA DE GITHUB

