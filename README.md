# aprendiendogit

Tutorial de comandos básicos y workflow en equipo

<span style="display:block;text-align:center">![image](https://user-images.githubusercontent.com/49002900/140984964-8beffbf0-d941-431a-8c71-46083a042aeb.png)</span>

# Primeros pasos

Configurar el Nombre que sale en los commits
```ssh
	git config --global user.name "michaelsordo"
```
Configurar Email
```ssh	
	git config --global user.email michaelsordoseijo@gmail.com
```
Marco de colores para los comandos
```ssh
	git config --global color.ui true
```

# Iniciar repositorio

Iniciamos git en la carpeta donde está el proyecto
```ssh
	git init
```

Clonar repositorio
```ssh
	git clone <url>
```

Asegurarse siempre de estar trabajando con la última versión
```ssh
	git pull origin master
```

# Hacer commit

Añadimos todos los archivos para el commit
```ssh
	git add .
```

Hacemos el primer commit
```ssh
	git commit -m "Aprendiendo git"
```

Si solo queremos añadir un archivo
```ssh
	git add <archivo>
```

Ver las diferencias de las modificaciones en local respecto al repositorio remoto
```ssh
	git diff 
```

# Trabajando con ramas

Crear una branch
```ssh
	git branch <nameBranch>
```

Cambiarnos de branch
```ssh
	git checkout <nameBranch>
```

Listar branch
```ssh
	git branch 
```
Listar todas las branch en local y remoto
```ssh
	git branch -a
```

# Ver las diferencias entre los cambios

Te permite ver las diferencias en local respecto al repositorio remoto
```ssh
	git diff
```

# Subiendo el código

Subir == PUSH
```ssh
	git push origin master
```

# Descargando código

Descargar == PULL
```ssh
	git pull origin master
```


# Workflow en equipo

1.Asegurarnos de que tenemos la ultima version
```ssh
	git pull origin master
```

2.Crear una branch
```ssh
	git branch <nameBranch>
```
3.Pasarnos a esa branch
```ssh
	git checkout <nameBranch>
```
4.Modificamos código

5.Añadimos todos los archivos para el commit o el archivo en cuestión
```ssh
	git add .
```
6.Hacemos commit
```ssh
	git commit -m "Modificando aprendiendogit"
```
7.Subirlo a mi branch 
```ssh
	git push -u origin <miBranch>
```
8.Unir nuestra branch a master. Para eso nos pasamos a master
```ssh
	git checkout master
```
9.Mostrar las branch que hemos "mergeado" hasta ahora(No obligatorio).
```ssh
	git branch --merged
```
10.Ahora "mergeamos" nuestra branch
```ssh
	git merge <miBranchconlaquetrabaje>
```
11.Metió los cambios ya,pero todavía está en nuestra máquina.Lo subimos.
```ssh
	git push origin <master>
```
Es una buena práctica limpiar las branch(No obligatorio)
```ssh
	git push origin --delete <miBranch>
```

# Arreglando errores y fallos

Teniendo ya las modificaciones realizadas y añadidos los archivos
que hemos modificado a la working area. Luego con el comando 
siguiente modificamos el último commit

```ssh
	git commit --ammend
```

Deshacer un commit o cambios en una rama
```ssh
	git reset --hard <commit_id o hash> 
```

Ver commit id
```ssh
	git log
```