# Ejercicio integrador (clases 90 y 91)

Para este ejercicio vamos a hacer una pequeña web estática con React. 

El diseño sugerido es [este](https://app.zeplin.io/project/5c3f3f3e182f8e339ca49b34/screen/5e5fddce588192130135038f), pero sentite libre de modificarlo como más te guste o hacer un estilado mínimo: la idea es practicar React y no maquetado. 

**Si no tenés acceso a esa web, por favor enviame tu mail por discord. Si ya lo hiciste, debes aceptar la invitación de Zeplin que llegó a tu correo.**

Dado el siguiente array de objetos, 

```js
const products = [
  {
    title: 'Coombes',
    type: "Lounge",
    price: 2600,
    rating: 4,
    img: 'https://i.imgur.com/ZAxMGG5.png',
    isAvailable: true,
    onSale: false,
  },
  {
    title: 'Keeve Set',
    type: "Table & Chairs",
    price: 590,
    rating: 4,
    img: 'https://i.imgur.com/tT8sFIs.jpeg',
    isAvailable: false,
    onSale: false,
  },
  {
    title: 'Nillè', 
    type: "Armchair",
    price: 950,
    rating: 5,
    img: 'https://i.imgur.com/Vx1cZY0.png', 
    isAvailable: false,
    onSale: true,
  },
  {
    title: 'Blanko', 
    type: "Side table",
    price: 90,
    rating: 4,
    img: 'https://i.imgur.com/N1Bf4ox.jpg',
    isAvailable: true,
    onSale: false,
  },
  {
    title: 'Momo', 
    type: "Shelves",
    price: 890,
    rating: 4,
    img: 'https://i.imgur.com/AlKxDE4.jpeg', 
    isAvailable: true,
    onSale: false,
  },
  {
    title: 'Penemillè', 
    type: "Chair",
    price: 120,
    rating: 4,
    img: 'https://i.imgur.com/pmANPjN.jpeg',
    isAvailable: true,
    onSale: false,
  },
  {
    title: 'Kappu', 
    type: "Shelves",
    price: 420,
    rating: 4,
    img: 'https://i.imgur.com/s2rsPa1.jpg',
    isAvailable: true,
    onSale: false,
  },
];
```

### Primera parte 

1. Crear un nuevo proyecto de React
2. En App.js, copiar el array. 
3. Por cada uno de los elementos del array, mostrar un componente `<Card>` que muestre las propiedades: `title`, `type`, `price` e `img`. 
4. Estilar las tarjetas con `scss`, declarando un archivo llamado `Card.scss`, siguiendo el estilado sugerido o como más te guste.  


### Segunda parte

1. Agregar dos `props` a cada componente `Card`: `isAvailable` y `onSale`. 
2. Si `isAvailable` es `false`, el fondo de la tarjeta debe mostrarse en gris. (O cualquier otro estilado que prefieras, por ejemplo, la imagen puede tener un overlay gris, el titulo puede estar tachado, etc). 
3. Si `onSale` es `true`, al lado del titulo debe aparecer un `span` que diga "ON SALE!" 

### Tercera parte

Cada tarjeta debe mostrar su `rating` correspondiente. 
1. Para comenzar, que cada tarjeta muestre el numero correspondiente a la propiedad `rating`. 
2. Una vez logrado eso, agregá los iconos de Font Awesome a tu proyecto de React. Para usar los iconos de Font Awesome vas a tener que instalar 3 dependencias en tu proyecto:
    - `@fortawesome/free-regular-svg-icons`
    - `@fortawesome/free-solid-svg-icons`
    - `@fortawesome/react-fontawesome`
Proba con una sola estrella para ver si se ve bien, y recorda que siempre tenes a disposicion la documentacion oficial: https://fontawesome.com/how-to-use/on-the-web/using-with/react
3. Usando los componentes `faStar` de /solid y `faStar` de /regular (recorda que le tenes que cambiar el nombre a alguno de los dos), lográ que el rating se vea correctamente de acuerdo al modelo. 
