# Esta es una breve explicacion de cómo usar Github

    1) Tenemos que iniciar el repositorio local en la ubicación que queramos, pararnos ahí, y en la
    terminal de Git, hacer un: 
        git -init
    2) Configurar el nombre de usuario y el mail con el comando:
        git config user.name "USER-NAME"
        git config user.email "USER-EMAIL"
    En caso de querer hacerlo de una vez para siempre, se puede hacer:
        git config --global user.name "USER-NAME"
        git config --global user.email "USER-EMAIL"
    3) Para linkear el repositorio local, con el remoto en un futuro, hay que apuntar
    al mismo a través de la URL, o de la clave SSH, ambos se copian del repositorio en 
    github, y se escribe el sig. comando:
        git remote add origin URL-O-SSH-KEY

# De este paso en adelante, va a ser lo mas repetitivo que vamos a hacer, lo anterior se hace una sola vez 
# al principio cuando se crea
    
    4) Hay que agregar los archivos al "staging area", para esto se pueden usar dos comandos, el primero
    agregará todos los archivos, y el segundo sólo los que yo indique con su nombre:
        git add . 
        git add FILE-NAME
    5) Dentro del "staging area" se van a commitear, o comentar los archivos, es una buena práctica hacerlo
    para que se entienda que cambios implemento en esa nueva versión.
        git commit -m "NEW-VERSION-DESCRIPTION"
    6) Una vez hecho el commit, solo queda subirlo al repo remoto, y esto es con:
        git push origin master
    Que va a pushear, los cambios al repo remoto -> origin, en la rama master, también llamada main.

