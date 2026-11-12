# VíaGest — ampliación documental (demostración)

Proyecto React + TypeScript + Vite basado en el ZIP proporcionado.

## Ejecutar en Windows
1. Descomprime el ZIP y abre la carpeta en Visual Studio Code.
2. En la terminal PowerShell, si Node no se reconoce: `$env:Path += ";C:\Program Files\nodejs"`.
3. Ejecuta `npm.cmd install` y después `npm.cmd run dev`.
4. Abre la dirección local que indique Vite (habitualmente http://localhost:5173/).

## Funciones nuevas
- Ruta `/documentacion`: guía sobre documentos, obtención, preparación y fotografía.
- Asistente de 8 preguntas sobre operación, partes, residencia fiscal, documentos y circunstancias especiales.
- Lista orientativa de documentos y advertencia de revisión profesional.
- Subida temporal de PDF/JPG/PNG (máx. 10 MB), arrastrar y soltar, vista previa y eliminación.
- Resumen de archivos y comprobación de documentos marcados como requeridos en el prototipo.

## Limitaciones importantes
No es una plataforma de producción: no existe backend, almacenamiento, firma electrónica, cobro, envío a gestoría ni integración con DGT. No utilices documentos personales reales para probar. Las reglas documentales son orientativas y requieren revisión jurídica y operativa por la gestoría antes de ofrecer un servicio real. Las tarjetas de ejemplo son ilustraciones genéricas, no imágenes oficiales. La política de privacidad es provisional.

## Verificación
La comprobación TypeScript `tsc -b` finalizó sin errores en el entorno de desarrollo. No se pudo completar `vite build` en Linux porque el ZIP contenía dependencias nativas de Rollup para Windows y no estaba disponible el paquete nativo de Linux; ejecuta `npm.cmd install` y `npm.cmd run build` en Windows para validar la compilación final.
