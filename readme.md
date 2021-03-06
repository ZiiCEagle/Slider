# Slider Jquery v1.0

Ce plugin vous permettra de faire simplement des sliders entre deux images au survol de la souris.
Vous pouvez également accéder à une démo en ligne sur http://guillaumebriday.github.io/slider-jquery/.

## Table des matières

* Membre(s)
* Dépendance
* Comment s'en servir
* Informations complémentaires


## Membre(s)

* "Guillaume Briday" <guillaumebriday@gmail.com>

## Dépendance

Le plugin a besoin de Jquery pour fonctionner.

## Comment s'en servir

1. Inclure le css :

    ```html
        <link rel="stylesheet" href="js-slider.min.css">
        // <link rel="stylesheet" href="js-slider.css">
    ```

2. Inclure Jquery et le plugins:

    ```html
        <script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>
        <script  type="text/javascript" src="js-slider.min.js"></script>
        // <script  type="text/javascript" src="js-slider.js"></script>
    ```

3. Coller la structure HTML du plugin où vous le souhaitez :

    Vous devrez adapter le lien des images pour y mettre les votres.

    ```html
        <div class="js-slider-container">
            <img src="before.jpg" class="js-slider-first" />
            <div class="js-slider-last-container">
                <img src="after.jpg" class="js-slider-last">
            </div>
        </div>
    ```


4. Appelez le plugin en Jquery:

    ```javascript
        (function($){
            $(".js-slider-container").slider();
        })(jQuery);
    ```

    Vous pouvez également rajouter des options :

    * rollback : permet de faire revenir automatiquement ou non le slider au milieu lorsque la souris ne survole plus les images.
    * duration : C'est le durée de l'animation de "callback" en ms
    * width : C'est la taille par défaut de la seconde image

    ```javascript
        (function($){
            $(".js-slider-container").slider({
                rollback : true, // true|false
                duration : 400, // Durée de l'animation en ms
                width : '50%'
            });
        })(jQuery);
    ```

## Informations complémentaires

N'hésitez pas à me contacter pour avec des informations complémentaires ou me remonter un bug.
