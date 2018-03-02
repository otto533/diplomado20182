# Modificaciones proyecto whatHappenedToMe

1. Los objetos gráficos como lo es el botón y la etiqueta de texto se encontraban duplicados, cuyos duplicados les agregaban al nombre la palabra outlet

2. El botón no contenía el mensaje “Touch me” en el storyboard

3. Para los fines de este proyecto no necesitamos un outlet para el botón. El correspondiente mensaje “Touch me” se pudo asignar desde el interface builder

4. La instancia del outlet para la etiqueta de texto carece de la palabra reservada IBOutlet	

5. La función a llamar al momento de apretar el botón no fue declarada como IBAction, de modo que fue necesario agregar dicha palabra reservada

6. El tipo de datos del sendero dentro de la función decía any, lo correcto es que sea UIButton


7. Las referencias hechas entre el intarfacebuilder y el viewcontroller estaban incorrectas, de modo que se hizo su respectivo flujo para un funcionamiento correcto

   - Botón: 		InterfaceBuilder -> ViewController
   - TextField: 		VierController -> InterfaceBuilder
