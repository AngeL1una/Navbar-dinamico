# Navbar-dinamico
Este fragmento de código define un arreglo llamado navItems que contiene objetos
con las propiedades path y text. Cada objeto representa un enlace de navegación con su ruta y el texto a mostrar.

--------------------------------
const navItems  = [
  {path: '/about', text: 'About'},
  {path: '/contact', text: 'Contact'},
  {path: '/pricing', text: 'Pricing'}
]
--------------------------------
El código utiliza la función map() para recorrer el arreglo navItems y generar enlaces dinámicamente.
Este código es adecuado para un proyecto en Next.js donde el componente <Link> de Next.js es utilizado para la navegación.
--------------------------------
{
   navItems.map(navItem =>(
    <Link key={navItem.path} className='p-2' href={navItem.path}>{navItem.text}</Link>
  )) 
}

Angel Luna Lugo 
