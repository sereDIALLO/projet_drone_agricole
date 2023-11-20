# Description technique du projet Wingman

Wingman est une aile volante autonaume avec station de chargement qui est capable de patrouiller une zone voulue et de détecter des animaux et personnes avec une suite de caméras thermiques et optiques. Son rôle principal sera donc la surveuillance de zones prédéfinies, et la défense de ces zones contre des animaux qui pourraient endommager les sols et plantations (oiseaux, sangliers, ...) au moyen de systèmes sonores et lumineux.   

L'aile volante sera un design full-body en polymères légers mais durables, avec une propulsion arrière par hélice et un moteur électrique style BLDC.   
Le système de vol sera contrôlé par un ordinateur de vol dédidé (avec gps et système d'IMU 9 axe pour positionnement XYZ et rotation 3 axes), ainsi qu'un driver de moteur BLDC et divers servomoteurs pour le contrôle des ailerons.

Un modem 4G sera présent dans l'ordinateur de bord et le système embarquera un ordinateur basé sur le SOC RK3588s, qui permet une grande puissance de calcul, ainsi qu'une accélération IA à 6 Tops. 8gb de ram seront présents sur l'ordinateur de bord et le système fonctionnera sous une variente de linux Debian, armbian, qui ne posera pas de problèmes de licence.

Le système sonore sera géré par un puissant amplificateur connecté en I2S, et le système lumineux sera contrôlé par PWM pour le mouvement de viders moteurs autour du laser.

Enfin un système de TOF (time of flight) sera présent au milieu de l'aile volante vers le bas pour une meilleure estimation de l'altidude.

Le système de caméra sera double, on aura une caméra thermique pour la détection de personnes longue distance (Flir Boson®+ CZ 14-75), et la caméra optique sera une caméra global shutter haute résolution à déterminer.
