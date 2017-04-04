% A mockup document of plantkeeper application  
% Erik J. Kinnunen; 1502999
% April 4, 2017

Description
===========
Herb and plant managing software


Technologies
------------
  * React (React-Native)
  * NodeJS
  * MongoDB (or Firebase)
  * OpenWeatherMap

Backend logic steps
-------------------
* Water need calculation
    1. Get weather data
    1. Determine weather type (cloudy, sunny)
    1. Compare room temperature to outside temperature
    1. Change water intake level based on the temperature
    1. Calculate new water need  
* Fertilize need calculation
    1. Get current season
    1. Determine fertilize application interval
    1. Calculate new fertilize value
\pagebreak

Database schema sketch
----------------------

Example of basic database composition

  **Plant**  

  | Name | Type | Planting | Location | Water | Fertilizer | Temperature | UserID |
  |:----:+:----:+:-----:+:--------:+:------:+:------:+:-:|
  | Basil | Basil | 1.1.2017 | Helsinki | 100 | 100 | 21 | 1 |

  **Type**

  * Values are measured in interval of days
  * Values in TYPE table are the default plant values

  | Type | Watering | Fertilize |
  |:----:+:--------:+:-----------:|
  | Basil| 1        | 16          |

  **User**

  | Id | Name | Password |
  |:---:+:----:+:--------:|
  | 1  | ejuh | &%212345 |

User interaction
----------------

  1. __View__
      * Water and fertilizer level bars
      * Plant statistics
      * Current weather on plant location
      * Amount of plants
      * List view  
  2. __Action__
      * Add plants
      * Action buttons in plant view
          * Watering button
          * Fertilizer button
\pagebreak

View mockup
------
![Mockup image](http://erikjuhani.com/img/plantkeeper.png "Mockup")
