# aprendiendogit

Tutorial de comandos básicos y workflow en equipo

<span style="display:block;text-align:center">![image](https://user-images.githubusercontent.com/49002900/140984964-8beffbf0-d941-431a-8c71-46083a042aeb.png)</span>

# Primeros pasos

Configurar Nombre que salen en los commits
```ssh
	git config --global user.name "michaelsordo"
```
Configurar Email
```ssh	
	git config --global user.email michaelsordoseijo@gmail.com
```
Marco de colores para los comando
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

Asegurarse siempre de estar trabajando con la última version
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

Si solo queremos añadir un archivos
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

Te permite ver las diferencias en local respecto al repositorio
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

Asegurarnos de que tenemos la ultima version
```ssh
	git pull origin master
```

Crear una branch
```ssh
	git branch <nameBranch>
```
Pasarnos a esa branch
```ssh
	git checkout <nameBranch>
```
Modificamos código
Añadimos todos los archivos para el commit o el archivo en cuestión
```ssh
	git add .
```
Agregamos archivo/commit
Subirlo a mi branch 
```ssh
	git push -u origin <miBranch>
```
Unir nuestra branch a master
Pasarnos a master
```ssh
	git checkout master
```

Mostrar las branch que hemos "mergeado" hasta ahora
Si solo hemos utilizado master solo aparecerá esta
```ssh
	git branch --merged
```
Ahora "mergeamos" nuestra branch
```ssh
	git merge <miBranchconlaquetrabaje>
```
Metió los cambios ya , pero todavía está en nuestra máquina
Lo subimos
```ssh
	git push origin <master>
```
Es una buena práctica limpiar las branch
```ssh
	git push origin --delete <miBranch>
```

