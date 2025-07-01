# 🆘 Solución de problemas

## Problemas comunes y soluciones

### El dispositivo no arranca

**Síntomas**: Pantalla negra, no responde al encender
**Soluciones**:

- ✅ Verificar que la fuente de alimentación proporcione suficiente corriente (se recomiendan 2 A)
- ✅ Comprobar que todas las conexiones de hardware estén seguras
- ✅ Probar con otra tarjeta SD con una imagen de SeedSigner nueva
- ✅ Probar con otro cable de alimentación

### Problemas con el escaneo de códigos QR

**Síntomas**: Códigos QR no reconocidos, tiempos de espera de escaneo
**Soluciones**:

- ✅ Asegurarse de que el código QR esté bien iluminado
- ✅ Mantener el dispositivo firme a una distancia adecuada (15-30 cm)
- ✅ Limpiar la lente de la cámara con un paño suave
- ✅ Intentar ajustar la densidad del código QR en la configuración
- ✅ Comprobar la configuración de rotación de la cámara
- ✅ Probar la funcionalidad de la cámara en E/S de hardware Prueba

### Generación incorrecta de la semilla

**Síntomas**: La semilla generada no coincide con los resultados esperados
**Soluciones**:

- ✅ Verificar que se estén utilizando las fuentes de entropía adecuadas (buena aleatoriedad)
- ✅ Asegurarse de que la iluminación sea adecuada durante la captura de entropía de la cámara
- ✅ Para las tiradas de dados, usar dados físicos adecuados (no digitales)
- ✅ Verificar la transcripción de la palabra semilla durante la copia de seguridad
- ✅ Ejecutar el proceso de verificación de la copia de seguridad

### Problemas de respuesta de los botones

**Síntomas**: Los botones no responden, entrada inconsistente
**Soluciones**:

- ✅ Ejecutar una prueba de E/S de hardware para identificar el problema
- ✅ Limpiar los botones para eliminar residuos
- ✅ Comprobar si el sombrero WaveShare presenta daños físicos
- ✅ Probar diferentes combinaciones de botones (A, B, C funcionan de forma idéntica)

### Problemas de pantalla

**Síntomas**: Parpadeo de la pantalla, parcial Pantalla, colores incorrectos
**Soluciones**:

- ✅ Revisar las conexiones del dispositivo WaveShare
- ✅ Ejecutar la prueba de E/S de hardware
- ✅ Probar con una fuente de alimentación diferente
- ✅ Verificar la integridad de la tarjeta SD

## Mensajes de error

### "Tipo de QR desconocido"

**Significado**: SeedSigner no reconoce el formato del código QR escaneado
**Soluciones**:

- ✅ Verificar que se está escaneando un tipo de QR compatible (PSBT, SeedQR, etc.)
- ✅ Verificar la calidad y claridad del código QR
- ✅ Asegurarse de que la iluminación y la posición de la cámara sean adecuadas

### "Semilla no válida"

**Significado**: La frase semilla introducida no pasa la validación BIP-39
**Soluciones**:

- ✅ Revisar cada palabra de la frase semilla
- ✅ Verificar que el orden de las palabras sea correcto
- ✅ Asegurarse de que todas las palabras sean del Lista de palabras BIP-39
- ✅ Revisar errores tipográficos al introducir manualmente

### "Error de suma de comprobación"

**Significado**: La última palabra no coincide con la suma de comprobación requerida
**Soluciones**:

- ✅ Usar la herramienta "Calcular 12.ª/24.ª palabra" para encontrar la última palabra correcta
- ✅ Verificar que todas las palabras anteriores sean correctas
- ✅ Revisar errores de transcripción
