# CsBases - Fundamentos de .NET

Este proyecto es una guía práctica sobre los conceptos esenciales de C# y .NET, estructurado para demostrar desde tipos de datos básicos hasta patrones de diseño y asincronía.

## 📂 Estructura del Proyecto

El código está organizado por módulos para facilitar la navegación:

* **02-Tipos-Basicos**: Manejo de `DataTypes` y lógica fundamental.
* **04-Herencia**: Implementación de contratos con `IProduct` y la clase base `Product`.
* **05-Patron-Adaptador**: Transformación de modelos mediante `ProductDto` y `ProductAdapter`.
* **06-Inyeccion-dependencias**: Desacoplamiento de lógica con `LabelService` y `ProductManager`.
* **07-Metodos-Asincronos**: Simulación de acceso a datos con `ProductRepository`.
* **08-Atributos**: Decoración de código con metadatos personalizados (`UpperCaseAttribute`).

---

## 🛠️ Conceptos Destacados

### El Patrón Adaptador (DTO)
El `ProductAdapter` actúa como un puente para transformar entidades de dominio en objetos de transferencia de datos (DTOs). Esto permite:
1.  **Seguridad**: No exponer datos sensibles del modelo original.
2.  **Formateo**: Preparar los datos para la interfaz de usuario (ej. el campo `Code`).



### Transformación de Identificadores
El proyecto utiliza una lógica específica para la generación de códigos de producto:
- **Regla**: `P-{Id}-{8 caracteres del GUID}`
- **Implementación**: Se utiliza interpolación de cadenas y manipulación de `ReadOnlySpan<char>` o `Substring`.

---

## 🚀 Instalación y Uso

1. **Requisitos**: Tener instalado [.NET 10 SDK](https://dotnet.microsoft.com/).
2. **Clonar**:
   ```bash
   git clone [https://github.com/tu-usuario/CsBases.git](https://github.com/tu-usuario/CsBases.git)
3. **Ejecutar en terminal**:
    ```bash
    dotnet run 
     ```