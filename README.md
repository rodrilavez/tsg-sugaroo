# The Sakai Group - Website

## Problemas identificados y solucionados

### ✅ Rutas corregidas
- Cambiadas todas las rutas relativas (`./`) por rutas absolutas (`/`)
- Corregidas las rutas en favicon y manifest
- Actualizadas las imágenes de fondo en CSS

### ⚠️ Problema pendiente: Archivo TIFF
El archivo `crowd.tiff` no es compatible con todos los navegadores web. 

**Solución recomendada:**
1. Ejecutar el script de conversión:
   ```bash
   ./convert-image.sh
   ```

2. Luego actualizar el HTML para usar el archivo WebP:
   ```html
   <img src="/images/crowd.webp" alt="Crowd at concert" ...>
   ```

### 📁 Archivos agregados
- `vercel.json`: Configuración para el despliegue en Vercel
- `.gitignore`: Para evitar archivos innecesarios en el repositorio

### 🚀 Despliegue en Vercel
Los cambios están listos para el despliegue. Las rutas ahora funcionarán correctamente en Vercel.

## Comandos útiles

```bash
# Convertir imagen TIFF a WebP
./convert-image.sh

# Verificar el sitio localmente
python3 -m http.server 8000
# Luego visitar: http://localhost:8000
```
