Esta colección de archivos muestra el juego del wumpus usando lógica proposicional, implementado mediante el algoritmo de DPLL consistente en la reducción de 
ramificación gracias al uso de símbolos puros y cláusulas unitarias.

- Agent.py controla el núcleo del juego, es el agente, quien recibe información del entorno, y mediante la función de 'entails' realiza una reducción al absurdo
mediante el algoritmo del DPLL.
- GeneraciónTablero y RenderizadoTabla son dos scripts para la generación del entorno del juego, de manera que su representación se vea de manera clara. Para ello
se establece un tamaño de tablero NxN, y los elementos son colocados de manera al azar; cada vez que se reinicia el juego, el tablero cogerá una forma nueva. Se crea
una función que establece un camino entre el agente y el oro, evitando así un juego imposible (el camino es totalmente random, la única condición es que deben ser
casillas adyacentes, no sigue ni un algoritmo de camino más corto)
- Experimento.py es un script implementado, usando Chatgpt, con el objetivo de ver cómo varía el tiempo en función del aumento del tamaño de tablero y con ello el
número de símbolos presentes.

Se podrá hacer una prueba de ejecución, ejecutando únicamente el fichero main.py desde terminal.
