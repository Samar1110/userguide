# Cálculo de la generación de la frase semilla de 12.ª/24.ª palabra

Este método de creación de frases semilla permite generar una frase semilla criptográficamente segura introduciendo manualmente 11 palabras (para una frase semilla de 12 palabras) o 23 palabras (para una frase semilla de 24 palabras) y calculando la palabra final con la validación de suma de comprobación adecuada. La palabra final (12.ª o 24.ª) incorpora entropía adicional y garantiza que la frase semilla cumpla con los estándares BIP39.

## Proceso completo con todas las capturas de pantalla

1. **Navegar**: Menú principal → **Herramientas** → **Calc. 12ª/24ª Palabra**

<div align="center">
     <img src="images/ToolsOptionSelectView.png" alt="Selección del menú Herramientas" width="250"/>
</div>
<div align="center">
<img src="images/SeedGenerateCalcMethodView.png" alt="Selección del método de dados" width="250"/>
</div>

2. **Elegir longitud**: Seleccionar **12 palabras** o **24 palabras**

<div align="center">
     <img src="images/SeedMnemonicLengthCalcView.png" alt="Longitud inicial para el cálculo de la palabra final" width="250"/>
</div>

3. **Ingresar palabras existentes**: Usar el teclado en pantalla Con sugerencias de palabras inteligentes:
- **Tecla A**: Subir en la lista de sugerencias
- **Tecla C**: Bajar en la lista de sugerencias
- **Tecla B**: Seleccionar la palabra sugerida resaltada

<div align="center">
     <img src="images/WordEntry.png" alt="Teclado en pantalla con sugerencias de palabras" width="250"/>
</div>

<div align="center">
     <img src="images/ToolsCalcFinalWordEnterSeedView.png" alt="Introducción de palabras semilla existentes" width="250"/>
</div>

## Métodos de entropía para calcular la palabra final

El sistema proporciona tres fuentes de entropía diferentes para calcular la palabra final, lo que garantiza la seguridad criptográfica:
<div align="center">
     <img src="images/ToolsCalcFinalWordFinalizePromptView.png" alt="Palabra semilla final" width="250"/>
</div>

**🪙 Método de Entropía al Lanzamiento de Moneda**

- Lanza una moneda física exactamente 7 veces.
- En cada lanzamiento, selecciona **1 para Cara** o **0 para Cruz** presionando el **Joystick**.
- Este método proporciona 7 bits de entropía para calcular la palabra final.

<div align="center">
     <img src="images/ToolsCalcFinalWordCoinFlipsView.png" alt="Interfaz de Entropía al Lanzamiento de Moneda" width="250"/>
</div>

- El sistema muestra la cadena binaria y calcula la suma de comprobación.

<div align="center">
     <img src="images/ToolsCalcFinalWordCoinFlipResultView.png" alt="Vista del resultado del lanzamiento de moneda" width="250"/>
</div>

**📝 Método de entropía por selección de palabras**

- Elija cualquier palabra de la lista de palabras BIP39 como su entropía. Fuente
- La palabra seleccionada proporciona los bits de entropía necesarios para el cálculo de la palabra final.

<div align="center">
     <img src="images/ToolsCalcFinalWordEntropyView.png" alt="Método de entropía por selección de palabras" width="250"/>
</div>

<div align="center">
     <img src="images/ToolsCalcFinalWordEntropyResultView.png" alt="Método de entropía por selección de palabras" width="250"/>
</div>

**🔢 Método de terminación en cero**

- Utiliza una cadena simple de ceros de 7 bits más la suma de comprobación de 4 bits calculada. - Este es el método más simple, pero aun así produce una palabra final válida.

<div align="center">
     <img src="images/ToolsCalcFinalWordZerosMethodView.png" alt="Selección del método de ceros" width="250"/>
</div>

## Visualización y finalización de la palabra final

**Visualización de la palabra final**

- Muestra la palabra final calculada con todos los detalles de su derivación.
- Muestra la fuente de entropía utilizada y el cálculo de la suma de comprobación.

<div align="center">
     <img src="images/ToolsCalcFinalWordShowFinalWordView.png" alt="Pantalla de cálculo de la palabra final" width="250"/>
</div>

**Pantalla de finalización**

- Revisa la frase inicial completada con la palabra final calculada.
- Tu frase inicial ya está lista para ser respaldada y utilizada.

<div align="center">
     <img src="images/ToolsCalcFinalWordDoneView.png" alt="Cálculo de finalización de la palabra final" width="250"/>
</div>

> **📚 Nota técnica**: La palabra final de cualquier semilla BIP39 contiene bits de entropía y bits de suma de comprobación. La suma de comprobación garantiza la validez matemática de la frase inicial y ayuda a detectar errores de transcripción.