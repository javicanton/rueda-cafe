# 🍃 Rueda de Sabores del Café Interactiva

Una visualización interactiva tipo sunburst de 3 niveles para representar la rueda de sabores del café, desarrollada con D3.js.

![Coffee Flavor Wheel](https://img.shields.io/badge/Visualización-Sunburst-blue) ![D3.js](https://img.shields.io/badge/D3.js-v7-green) ![CSV](https://img.shields.io/badge/Datos-CSV-orange)

## ✨ Características

- 🎯 **Sunburst de 3 niveles**: Visualización jerárquica clara y elegante
- 📊 **Carga desde CSV**: Importa tus propios datos fácilmente
- 🎨 **Colores personalizables**: Define colores específicos en el CSV
- 🖱️ **Interactiva**: Haz clic en los segmentos para ver detalles
- 📱 **Responsive**: Se adapta a diferentes tamaños de pantalla

## 🚀 Cómo Usar

### En GitHub Pages (recomendado)
1. Sube el proyecto a GitHub
2. Activa GitHub Pages en la configuración del repositorio
3. Abre la URL: `https://javicanton.github.io/rueda-cafe`
4. ¡Funciona directamente sin servidor local!

### Local
1. Simplemente abre `index.html` en tu navegador
2. La visualización se cargará automáticamente
3. ¡Explora haciendo clic en los segmentos!

## 📁 Estructura del Proyecto

```
rueda-cafe/
├── index.html                    # Aplicación principal
├── coffee_flavor_wheel.csv      # Datos del Coffee Lexicon
└── README.md                    # Este archivo
```

## 📊 Formato del CSV

El archivo CSV usa el formato del SCAA Coffee Taster's Flavor Wheel Lexicon:

```csv
Nivel1,Nivel2,Nivel3,Color,Definición (Lexicon),Tipo ref.,Referencia ejemplo,Intensidad ref.,Preparación ref.
Dulce,Caramelo,Miel,#f48fb1,"Aromático dulce, floral y viscoso.",Sabor,Miel comercial,—,—
Afrutado,Frutas cítricas,Limón,#ef5350,"Cítrico, ácido, astringente.",Ambos,Zumo limón 1:4,Aroma 5.5; Sabor 7,—
```

### Columnas principales:

- **Nivel1**: Categoría principal (nivel más interno del sunburst)
- **Nivel2**: Subcategoría (nivel medio)
- **Nivel3**: Descriptor específico (nivel externo)
- **Color**: Color en formato hexadecimal (#RRGGBB)
- **Definición**: Descripción sensorial del descriptor (se muestra al hacer clic)

## 🛠️ Tecnologías

- **HTML5** - Estructura
- **CSS3** - Estilos modernos
- **JavaScript ES6+** - Lógica de la aplicación
- **D3.js v7** - Visualización tipo sunburst

## 🔧 Configurar en GitHub

1. Crea un nuevo repositorio en GitHub

2. Sube los archivos:

```bash
git init
git add .
git commit -m "Initial commit: Coffee Flavor Wheel"
git branch -M main
git remote add origin https://github.com/javicanton/rueda-cafe.git
git push -u origin main
```

3. Activa GitHub Pages:
   - Ve a Settings > Pages
   - En "Source", selecciona "main" branch
   - Guarda y espera unos segundos
   
4. Abre la URL que te proporciona GitHub Pages

5. **IMPORTANTE**: Actualiza la línea 310 del `index.html` con tu usuario de GitHub:
   ```javascript
   'https://raw.githubusercontent.com/TU-USUARIO/rueda-cafe/main/coffee_flavor_wheel.csv'
   ```

## 💡 Personalización

### Crear tu propio CSV

1. Crea un archivo CSV con la estructura indicada arriba
2. Define tus categorías en 3 niveles
3. (Opcional) Especifica colores personalizados en formato hexadecimal
4. Carga el archivo usando el botón en la interfaz

### Modificar colores automáticos

Si no especificas colores en el CSV, se asignan automáticamente. Puedes modificar la paleta de colores editando esta línea en `index.html`:

```javascript
const color = d3.scaleOrdinal(d3.schemeSet3);
```

Otras paletas disponibles: `d3.schemeCategory10`, `d3.schemePastel1`, `d3.schemeTableau10`, etc.

## 📝 Datos Incluidos

El archivo `coffee_flavor_wheel.csv` incluye el lexicon completo de SCAA:

- **Dulce**: Aromáticos dulces (Vainilla, Vainillina), Caramelo (Azúcar moreno, Melaza, Jarabe de arce), Miel
- **Floral**: Rosa, Jazmín, Manzanilla, Té negro
- **Afrutado**: Frutas de baya (Fresa, Frambuesa, Arándano, Mora), Frutas secas (Uva pasa, Ciruela pasa), Otras frutas (Manzana, Pera, Melocotón, Uva, Cereza, Granada, Coco, Piña), Frutas cítricas (Limón, Pomelo, Naranja, Lima)
- **Ácido/Agrio**: Aromáticos agrios, Ácido acético, Ácido butírico, Ácido isovalérico, Ácido cítrico, Ácido málico
- **Alcohol/Fermentado**: Vinoso, Whiskey, Fermentado, Excesivamente maduro
- **Verde/Vegetal**: Aceite de oliva, Crudo, Inmaduro, Vaina de guisante, Verde (fresco, oscuro), Vegetal, Heno, Herbal, Leguminoso
- **Rancio/Papel**: Rancio, Papel, Cartón
- **Terroso**: Amaderado, Moho, Polvoriento, Húmedo, Fenólico, Animal, Cárnico/Caldo
- **Químico**: Amargo, Salado, Medicinal, Caucho, Petrolífero, Skunky
- **Tostado**: Tabaco, Tabaco de pipa, Acre, Ceniza, Quemado, Ahumado, Tostado (nivel), Tostado marrón
- **Cereal**: Grano, Malta
- **Especias**: Picante, Pimienta, Anís, Nuez moscada, Especias marrones, Canela, Clavo
- **Frutos secos**: Almendra, Avellana, Cacahuete
- **Cacao**: Chocolate, Cacao, Chocolate negro

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/nueva-caracteristica`)
3. Commit tus cambios (`git commit -m 'Agregar nueva característica'`)
4. Push a la rama (`git push origin feature/nueva-caracteristica`)
5. Abre un Pull Request

## 📄 Licencia

Este proyecto está bajo la Licencia MIT.

## 🙏 Agradecimientos

- Inspirado en la Coffee Taster's Flavor Wheel de SCAA/WCR
- Visualización construida con D3.js
- Diseño minimalista y funcional

---

**Desarrollado con ❤️ para la comunidad del café**
