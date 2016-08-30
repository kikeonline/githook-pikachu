# pikachu-githook
[githooks](https://git-scm.com/docs/githooks) - post-receive: Archivo que se ejecuta automáticamente al recibir un push de git al servidor. Este es un bash script base que se puede usar para automatizar pasos que se hacen despues de un push. Pero lo más importante de todo es que pikachu saluda a la persona que hizo el push.
![alt tag](https://github.com/kikeonline/pikachu-githook/blob/master/terminal-screen.png)

# Instalación/Uso
Copiar el archivo post-receive a la carpeta .git/hooks

Dar permisos ejecutables
  ```bash
  sudo chmod +x post-receive
  ```

En este archivo se encuentra una condicional: IF el push proviene del master se copian los archivos a la carpeta donde se sirve la pagina web, ELSE (otro branch que no es master) simplemente se recibe el push sin hacer nada mas.

De ahi la imaginación es el limite ✌️
