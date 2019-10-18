# Generador del sitio web PythonDay México 2019


## Instalación de Hugo

Todos los detalles de instalación de Hugo están acá:
<https://gohugo.io/getting-started/quick-start/>


## Setup del repositorio

1. Primero clonamos este repositorio:
   ```
   git clone https://github.com/PythonDayMX/website-generator.git
   ```
2. Clonamos el folder `public` desde otro repo (es la carpeta con los contenidos, lo que se publica):
   ```
   cd website-generator
   git clone https://github.com/PythonDayMX/pythondaymx.github.io.git
   mv pythondaymx.github.io public
   ```
3. Podemos iniciar el servidor con recarga en vivo de Hugo:
   ```
   hugo server
   ```
4. ¡Listo! Podemos proceder a editar el código con un refresh en vivo por parte del servidor. Los cambios pueden verse en `http://localhost:1313/`.

## Generador de cambios al folder `/public`

Una vez los cambios ya estén hechos, podemos generar el sitio a la carpeta `/public` haciendo:

```
hugo
```

Para hacer push de los cambios al repo del sitio web (`pythondaymx.github.io`), basta hacer:

```
cd public
git add .
git commit -m "Hice cambios XYZ."
git push
```
