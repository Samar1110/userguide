# Exportar clave pública (Xpub)

Crea monederos de solo lectura en tu software de Bitcoin favorito exportando tu clave pública. Esto te permite monitorear saldos y preparar transacciones sin exponer tus claves privadas.

## Proceso completo paso a paso con todas las capturas de pantalla

1. **Acceder a Exportar**: Desde la pantalla principal de la semilla, seleccione **"Exportar Xpub"**

<div align="center">
     <img src="images/SeedMenuView.png" alt="Menú principal de Seed con la opción Exportar Xpub" width="250"/>
</div>

2. **Seleccionar el tipo de firma**:
- **"Monofirma"** - Para monederos personales estándar
- **"Multifirma"** - Para monederos multifirma que requieren varios dispositivos

<div align="center">
     <img src="images/SeedExportXpubSigTypeView.png" alt="Selección del tipo de firma Xpub" width="250"/>
</div>

3. **Seleccionar el tipo de script**:
- **Native Segwit** (bech32) - Recomendado para las comisiones más bajas
- **Nested Segwit** (P2SH) - Para compatibilidad con sistemas antiguos
- **Taproot** - Para funciones avanzadas de privacidad y contratos inteligentes

<div align="center">
     <img src="images/SeedExportXpubScriptTypeView.png" alt="Selección del tipo de script para Xpub" width="250"/>
</div>

4. **Elegir el software de billetera**: Seleccione su billetera preferida entre las opciones compatibles

<div align="center">
     <img src="images/SeedExportXpubCoordinatorView.png" alt="Selección del software de billetera" width="250"/>
</div>

5. **Aceptar la advertencia de privacidad**: Pulse **"Entiendo"** después de leer las implicaciones de privacidad de Xpub

<div align="center">
     <img src="images/SeedExportXpubWarningView.png" alt="Pantalla de advertencia de privacidad de Xpub" width="250"/>
</div>

6. **Generar código QR**: Selecciona **"Exportar XPub"** para mostrar el código QR para compartir.

<div align="center">
     <img src="images/SeedExportXpubDetailsView.png" alt="Código QR generado por XPub" width="250"/>
</div>

7. **Importar a la billetera**: Escanea el código QR con el software de billetera que elijas.

<div align="center">
     <img src="images/SeedExportXpubQRView.png" alt="Código QR generado por XPub" width="250"/>
</div>

> **🔒 Advertencia de privacidad**: Tu XPub (clave pública extendida) revela todas tus direcciones de Bitcoin e historial de transacciones. Compártela únicamente con un software de billetera de confianza y nunca la publiques en línea.
