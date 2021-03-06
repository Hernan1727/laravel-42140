![logo de laravel](https://github.com/exegeses/laravel-42140/blob/main/imagenes/laravel-logo.png?raw=true)

# laravel-42140
> Curso de Laravel |  
> Martes y Jueves 19hs (Arg) |   
> Código: 42140 |  
> sensei: Marcos Pinardi |  

1. Definición
2. Requisitos
3. Recursos
4. Instalación
5. Iniciar el server

## Definición
> Laravel es uno de los frameworks de código abierto más fáciles de asimilar para PHP.  El objetivo de Laravel es el de ser un framework que permita el uso de una sintaxis refinada y expresiva para crear código de forma sencilla, evitando el “código espagueti” y permitiendo multitud de funcionalidades.  Aprovecha todo lo bueno de otros frameworks y utiliza las características de las últimas versiones de PHP.  Fue creado en 2011 por Taylor Otwell y tiene una gran influencia de frameworks como Ruby on Rails, Sinatra y ASP.NET MVC.  
> Gran parte de Laravel está formado por dependencias, especialmente de Symfony, esto implica que el desarrollo de Laravel dependa también del desarrollo de sus dependencias. 

## Requisitos

> De Software  

1. un terminal 
- [ ] la del sistema operativo  
- [ ] cmDer https://cmder.net/
- [ ] Cygwin https://www.cygwin.com/
- [ ] Git Bash

2. Composer 
 Composer es un administrador de dependencias en PHP.  
 https://getcomposer.org/  
 https://getcomposer.org/Composer-Setup.exe

## Recursos
- [ ] Manual oficial de Laravel:  https://laravel.com/
- [ ] Laracasts_  https://laracasts.com/
- [ ] Styde https://styde.net/ 
- [ ] Laravel News https://laravel-news.com/

## Instalación
> Usando composer vamos a movernos al directorio de trabajo    
> En ese directorio vamos a crear un proyecto (carpeta con toda la magia de laravel) .  
> Con el comando "cd" nos movemos a nuestro directorio de trabajo    
> y luego, con el comando "composer create-project" crearemos un proyecto     

`composer create-project laravel/laravel nombre "version"`


> Ejemplo para instalar laravel 6x    
`composer create-project laravel/laravel proyecto "6.*"`

## Iniciando el server
> Nos tenemos que mover a la carpeta del proyecto    
> y en la terminal hacer    

`cd proyecto`


> EL MARAVILLOSO MUNDO DE ARTISAN    
> para iniciar al server es el comando    

`php artisan serve `  

## Actualización desde un proyecto en repositorio

> Cuando en un equipo de trabajo varios descargar un proyecto iniciado, la instalación es diferente.

  -- Primero debemos descargar el proyecto
  
> Para descargar el proyecto podemos clonarlo usando git, pulearlo usando git o 
> simplemente descargando el .zip    

> Una vez que lo descargaste, aún no funciona, le faltan dependencias.
> ¿cómo las dedscargamos?

> Primero nos metemos en el directorio del proyecto y luego usamos el comando: 

    composer update    
 
> Este comando va a hacer que descargue todas las dependencias.   
> ¿ya está todo listo?  NO, aun falta crear el archivo de configuración general

> No tenemos el archivo .env, hay que crearlo. 
> Es tan simple como hacer una copia del archivo .env.example y renombrarlo .env    

> ¿ya está todo listo?  NO, aun falta generar la APP_KEY. Esto se logra con el comando:    


    php artisan key:generate 

