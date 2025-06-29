# Guía de Usuario de SeedSigner

<div align="center">
  <img src="/en/images/SeedSigner_Logo.png" alt="Logo de SeedSigner" width="400"/>
</div>

SeedSigner es un dispositivo de firma de Bitcoin de código abierto y con separación de aire que te ayuda a gestionar frases semilla y firmar transacciones de forma segura. Esta guía proporciona instrucciones paso a paso organizadas por flujos de trabajo comunes.

## 📋 Tabla de Contenidos

### 🚀 Primeros Pasos

- [Configuración Inicial y Encendido](/es/getting_started/initial_setup_and_power_on.md)
- [Fundamentos de Navegación](/es/getting_started/navigation_basics.md)
- [Apagado Seguro](/es/getting_started/powering_off_safely.md)
- [Reiniciar tu Dispositivo](/es/getting_started/restarting_your_device.md)

### 🌱 Gestión de Semillas

- **Crear Nuevas Semillas**
  - [Generación de Semilla Basada en Cámara](/es/seed_management/creating_new_seeds/camera_based_seed_generation.md)
  - [Generación de Semilla Basada en Dados](/es/seed_management/creating_new_seeds/dice_based_seed_generation.md)
  - [Generación de Semilla Calculando la 12ª/24ª Palabra](/es/seed_management/creating_new_seeds/calc_12th24th_word_seed_generation.md)
- **Cargar Semillas Existentes**
  - [Entrada Manual de Semilla](/es/seed_management/load_existing_seeds/manual_seed_entry.md)
  - [Escaneo de SeedQR](/es/seed_management/load_existing_seeds/seedqr_scanning.md)
  - [Agregar Frase de Paso BIP-39](/es/seed_management/load_existing_seeds/adding_bip_39_passphrase.md)

### 🔧 Trabajar con Semillas Cargadas

- [Exportar Clave Pública (Xpub)](/es/working_with_loaded_seeds/export_public_key_xpub.md)
- [Generar Dirección de Recepción](/es/working_with_loaded_seeds/generate_receiving_addresses.md)
- [Generar Cambio de Dirección](/es/working_with_loaded_seeds/generate_change_addresses.md)
- [Ver Palabras Clave](/es/working_with_loaded_seeds/view_seed_words.md)
- [Crear copia de seguridad de SeedQR](/es/working_with_loaded_seeds/create_seedqr_backup.md)

### ✍️ Transacciones y Verificación

- [Firmar Transacción de Bitcoin (PSBT)](/es/transacciones_y_verificacion/firmar_transaccion_bitcoin_psbt.md)
- [Verificar Propiedad de Dirección](/es/transacciones_y_verificacion/verificar_propiedad_de_direccion.md)
- [Descartar Semilla Cargada](/es/transacciones_y_verificacion/descartar_semilla_cargada.md)

### ⚙️ Configuración del Dispositivo

- **Configuraciones Básicas**
  - [Configuración de Idioma](/es/configuracion_del_dispositivo/configuraciones_basicas/configuracion_de_idioma.md)
  - [Configuraciones Persistentes](/es/configuracion_del_dispositivo/configuraciones_basicas/configuraciones_persistentes.md)
  - [Soporte de Software Coordinador](/es/configuracion_del_dispositivo/configuraciones_basicas/soporte_software_coordinador.md)
  - [Visualización de Denominación](/es/configuracion_del_dispositivo/configuraciones_basicas/visualizacion_de_denominacion.md)
  - [Prueba de E/S de Hardware](/es/configuracion_del_dispositivo/configuraciones_basicas/prueba_es_hardware.md)
  - [Información de Donaciones](/es/configuracion_del_dispositivo/configuraciones_basicas/informacion_de_donaciones.md)

- **Configuraciones Avanzadas**
  - [Selección de Red Bitcoin](/es/configuracion_del_dispositivo/configuraciones_avanzadas/seleccion_de_red_bitcoin.md)
  - [Densidad de Código QR](/es/configuracion_del_dispositivo/configuraciones_avanzadas/densidad_de_codigo_qr.md)
  - [Configuración de Exportación Xpub](/es/configuracion_del_dispositivo/configuraciones_avanzadas/configuracion_exportacion_xpub.md)
  - [Configuración de Tipos de Firma](/es/configuracion_del_dispositivo/configuraciones_avanzadas/configuracion_tipos_de_firma.md)
  - [Configuración de Tipos de Script](/es/configuracion_del_dispositivo/configuraciones_avanzadas/configuracion_tipos_de_script.md)
  - [Mostrar Detalles de Xpub](/es/configuracion_del_dispositivo/configuraciones_avanzadas/mostrar_detalles_xpub.md)
  - [Configuración de Frase de Paso BIP-39](/es/configuracion_del_dispositivo/configuraciones_avanzadas/configuracion_frase_de_paso_bip-39.md)
  - [Rotación de Cámara](/es/configuracion_del_dispositivo/configuraciones_avanzadas/rotacion_de_camara.md)
  - [SeedQR Compacto](/es/configuracion_del_dispositivo/configuraciones_avanzadas/seedqr_compacto.md)
  - [Semillas Hijas BIP-85](/es/configuracion_del_dispositivo/configuraciones_avanzadas/semillas_hijas_bip-85.md)
  - [Semillas Electrum](/es/configuracion_del_dispositivo/configuraciones_avanzadas/semillas_electrum.md)
  - [Firma de Mensajes](/es/configuracion_del_dispositivo/configuraciones_avanzadas/firma_de_mensajes.md)
  - [Advertencias de Privacidad](/es/configuracion_del_dispositivo/configuraciones_avanzadas/advertencias_de_privacidad.md)
  - [Advertencias Graves](/es/configuracion_del_dispositivo/configuraciones_avanzadas/advertencias_graves.md)
  - [Consejos de Brillo QR](/es/configuracion_del_dispositivo/configuraciones_avanzadas/consejos_brillo_qr.md)
  - [Logos de Socios](/es/configuracion_del_dispositivo/configuraciones_avanzadas/logos_de_socios.md)

- **Configuraciones de Hardware**
  - [Configuración de Tipo de Pantalla](/es/configuracion_del_dispositivo/configuraciones_hardware/configuracion_tipo_de_pantalla.md)
  - [Inversión de Color](/es/configuracion_del_dispositivo/configuraciones_hardware/inversion_de_color.md)

### 🔧 Soporte y Recursos

- [Solución de Problemas](/es/soporte_y_recursos/solucion_de_problemas.md)
- [Recursos Adicionales](/es/soporte_y_recursos/recursos_adicionales.md)
- [Consideraciones de Seguridad](/es/soporte_y_recursos/consideraciones_de_seguridad.md)

> 💡 **Consejo de Navegación Rápida**: Usa Ctrl+F (o Cmd+F en Mac) para buscar temas específicos dentro de esta guía.

---

## Componentes de Hardware

Un dispositivo SeedSigner consta de:

1. **Raspberry Pi Zero** - La unidad de procesamiento principal
2. **Cámara Raspberry Pi** - Para escanear códigos QR y capturar entropía
3. **WaveShare 1.3inch LCD Hat** - Pantalla e interfaz de control

### Controles del LCD Hat WaveShare

<div align="center">
  <img src="/en/images/WaveShare_LCD_Hat.png" alt="WaveShare LCD Hat" width="350"/>
</div>

El LCD Hat WaveShare proporciona los siguientes controles:

- **Joystick**: Navegación de cuatro direcciones (Arriba, Abajo, Izquierda, Derecha) más presión central
- **Key1 (A)**: Botón de acción principal
- **Key2 (B)**: Botón de acción secundario  
- **Key3 (C)**: Botón de acción terciario

### Referencia de Funciones de Botones

| Control        | Función                                    |
| -------------- | ------------------------------------------- |
| Joystick Arriba    | Mover selección hacia arriba                           |
| Joystick Abajo  | Mover selección hacia abajo                         |
| Joystick Izquierda  | Mover selección hacia la izquierda                         |
| Joystick Derecha | Mover selección hacia la derecha                        |
| Presión Joystick | Selección/confirmación alternativa (dependiente del contexto) |
| Key1 (A)       | Seleccionar opción resaltada o confirmar acción |
| Key2 (B)       | Seleccionar opción resaltada o confirmar acción |
| Key3 (C)       | Seleccionar opción resaltada o confirmar acción |

**Notas Importantes de Navegación**:

- Las tres teclas (A, B, C) funcionan de manera idéntica para selección y confirmación
- Para volver a una pantalla anterior, navega primero a la flecha/botón de retroceso usando el joystick, luego presiona cualquier tecla para activarlo
- La presión central del joystick puede tener diferentes funciones dependiendo del contexto de la pantalla actual

---

## 🏁 Conclusión

SeedSigner proporciona una solución segura y de código abierto para la gestión de claves de Bitcoin y la firma de transacciones. Siguiendo los flujos de trabajo de esta guía, puedes:

- ✅ Generar frases semilla verdaderamente aleatorias usando múltiples fuentes de entropía
- ✅ Cargar y gestionar de forma segura frases semilla existentes
- ✅ Firmar transacciones de Bitcoin sin exponer claves privadas a dispositivos conectados en red
- ✅ Exportar claves públicas para configuración de carteras de solo lectura
- ✅ Verificar la propiedad de direcciones y detalles de transacciones
- ✅ Mantener seguridad completa de separación de aire durante todas las operaciones

### Recuerda las Reglas de Oro

1. **Nunca omitas la verificación del respaldo de la semilla** - Una palabra incorrecta significa Bitcoin perdido
2. **Siempre verifica los detalles de la transacción** - Las transacciones de Bitcoin son irreversibles
3. **Mantén la seguridad de separación de aire** - Nunca conectes SeedSigner a redes
4. **Usa entornos privados** - Protégete contra vigilancia y grabación
5. **Almacena los respaldos de forma segura** - Trata las frases semilla como los activos valiosos que protegen

### Obtener Ayuda

Si encuentras problemas no cubiertos en esta guía:

- Revisa el repositorio oficial de SeedSigner en GitHub para actualizaciones
- Visita foros de la comunidad y grupos de chat para apoyo entre pares
- Revisa la sección de solución de problemas para soluciones comunes
- Considera contactar a la comunidad de desarrollo para problemas técnicos complejos

**Recuerda**: Tu seguridad de Bitcoin es en última instancia tu responsabilidad. Tómate el tiempo para entender cada paso, practica con cantidades pequeñas, y nunca te apresures durante operaciones críticas de seguridad.

---

*Esta guía es mantenida por la comunidad de SeedSigner y se actualiza regularmente. Para la versión más reciente y recursos adicionales, visita el repositorio oficial de SeedSigner en GitHub.*