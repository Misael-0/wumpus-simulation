Algoritmo Min-Max

Indicaciones y anotaciones sobre la práctica.

- El directorio "sprites" incluye las imágenes utilizadas para representar el tablero, estas imágenes han sido elaboradas en Photoshop CS6.

- El código ha sido ejecutado sobre Jupyter Notebook en su versión 6.4.8 y las imágenes se muestran correctamente, en versiones más recientes las imágenes no se muestran, pero en el ALT de cada imagen se ha indicado el nombre del Sprite, por tanto, aún así se podrá entender la representación del tablero.

- En la salida del código se incluye en modo texto cada una de las evaluaciones según los estados sucesores y se representa solo aquella escogida. Adicionalmente, se muestra el estado tras el movimiento real del agente y, luego, el estado tras el movimiento aleatorio del hoyo.

- Según el equilibrio de las puntuaciones tomadas para la evaluación de los sucesores, el agente busca el oro de una forma extremadamente segura, las ejecuciones pueden ser largas, pero las probabilidades de derrota son realmente bajas.

- Tal y como se comenta en el código, aunque se muestre la evaluación de la celda actual en la que se encuentra el agente, esta celda no se considera en minimax, porque se supone que el agente siempre debe moverse en su turno, no puede quedarse quieto. En el código se comenta una implementación alternativa para considerar la posición actual.

- Se prioriza respetar las reglas de distancia, si no es posible respetar alguna regla, se opta por no colocar la entidad. Esto significa que podría no colocarse uno de los hoyos. Se recomienda reiniciar el tablero si se da esta situación.