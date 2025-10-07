# 🍹 Cocktail Order System

Bienvenido a **Cocktail Order System**, una aplicación web desarrollada con React que permite a los usuarios explorar, seleccionar y realizar pedidos de cócteles, mientras que el personal del bar o restaurante puede gestionar los pedidos de manera eficiente. 🥂

---

## 🎯 Propósito

Esta aplicación tiene dos objetivos principales:

1. **Clientes**: Explorar y ordenar cócteles según categoría, búsqueda alfabética o selecciones destacadas.
2. **Personal del bar**: Gestionar los pedidos entrantes, siguiendo su ciclo de vida desde pendiente → atendido → pagado.

La aplicación integra la **API de TheCocktailDB** para obtener datos de bebidas y **Firebase** para persistencia de pedidos, asegurando un flujo completo de gestión de pedidos.

---

## 🛠 Pila técnica

La aplicación está construida con tecnologías modernas de desarrollo web:

- **React**: Biblioteca de UI basada en componentes.
- **react-router-dom**: Navegación multipágina del lado del cliente.
- **axios**: Cliente HTTP para llamadas a TheCocktailDB.
- **Firebase**: Backend como servicio para la gestión de pedidos.
- **react-bootstrap**: Componentes de interfaz adaptables.
- **styled-components**: Estilos CSS-in-JS para componentes.
- **@fortawesome**: Iconos para mejorar la UI.

---

## 🗂 Estructura de la aplicación

src/

├── pages/ # Páginas principales asignadas a rutas (Category, Search, Selection, Tpv)

├── components/ # Componentes reutilizables (Header, Navbar, Footer, Card, Button)

├── useContext/ # Gestión de estados globales con React Context

├── app/firebase/ # Integración con Firebase (CRUD)

├── img/ # Imágenes y activos estáticos

public/ # Archivos públicos (index.html, favicon)

---


Cada componente sigue el patrón **ComponentName.jsx + ComponentName.styles.js** para separar la lógica y los estilos.

---

## 🔄 Flujo de aplicación

1. El cliente añade bebidas a su pedido.
2. El estado del pedido se actualiza en **DataContext**.
3. Se sincroniza con **localStorage** para persistencia.
4. El personal gestiona el pedido desde la página TPV.
5. Una vez completado, el pedido se marca como pagado en Firebase.

---

## 🌐 Integración de servicios externos

| Servicio           | Función                                      |
|-------------------|---------------------------------------------|
| **TheCocktailDB** | Obtención de datos de cócteles (categorías, recetas, imágenes) |
| **Firebase**       | Persistencia de pedidos y estados de pago  |

---

## 📦 Instalación

1. Clonar el repositorio:
```bash
git clone https://github.com/MiriamFernandezPerez/cocktail-order-system.git
```

2. nstalar dependencias:
```bash
npm install
```

3. Iniciar la aplicación:
```bash
npm start
```

Abre http://localhost:3000 en tu navegador.

## 🧩 Funciones principales

- Explorar cócteles por **categoría, búsqueda o selección**.
- Añadir bebidas al **carrito de pedidos**.
- Gestión de pedidos mediante **página TPV**.
- Persistencia de pedidos y sincronización con **Firebase**.
- Interfaz adaptativa con **Bootstrap** y **Styled-Components**.
- Iconos interactivos con **FontAwesome**.

## 📖 Próximos pasos

Para más información sobre la arquitectura, patrones de estado o integración de API:

- Consulta los archivos en `src/useContext/` para **gestión de estado global**.
- Revisa `src/app/firebase/api.js` para **operaciones CRUD en Firebase**.
- Explora los componentes de `src/components/` para **UI y estilos**.

## 🍸 Autor

**Miriam Fernández Pérez**

Un sistema completo de pedidos de cócteles que une clientes y personal de bar en una experiencia fluida y moderna. ✨
