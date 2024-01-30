<h1 align="center">Hola 👋, soy Agustin Schwank</h1>
<h3 align="center">Un desarrollador frontend apasionado de: Santa Fe, Argentina</h3>

- 📝 Regularmente escribo artículos de <a target="_blank" href="https://agustinschwank.com.ar/">(musica, informatica, tutoriales)</a> que son algunas de mis pasiones.
- ⚡ Dato curioso: si te gusta, simplemente hazlo 
- 📫 Para contactarme: **hola@agustinschwank.com.ar**

<h3 align="left">Mis Redes Sociales:</h3>
<a href="https://www.facebook.com/agustinschwank" target="_blank"><img src='https://cdn-icons-png.flaticon.com/512/733/733547.png' alt='facebook' height='40'></a>  <a href="https://www.instagram.com/agustinschwank/" target="_blank"><img src='https://cdn-icons-png.flaticon.com/512/2111/2111463.png' alt='instagram' height='40'></a>  <a href="https://twitter.com/agustinschwank" target="_blank"><img src='https://cdn-icons-png.flaticon.com/512/124/124021.png' alt='twitter' height='40'></a>

<h3 align="left">Herramientas:</h3>
<p align=left">
<img src="https://img.icons8.com/fluency/344/visual-studio-code-2019.png" alt="vscode" width="40" height="40"/>  <img src="https://cdn-icons-png.flaticon.com/512/174/174854.png" alt="html5" width="40" height="40"/>  <img src="https://cdn-icons-png.flaticon.com/512/732/732190.png" alt="css3" width="40" height="40"/>  <img src="https://cdn-icons-png.flaticon.com/512/5968/5968292.png" alt="javascript" width="40" height="40"/>  <img src="https://cdn-icons-png.flaticon.com/512/919/919831.png" alt="sass" width="40" height="40"/>  <img src="https://cdn-icons-png.flaticon.com/512/919/919830.png" alt="php" width="40" height="40"/>  <img src="https://img.icons8.com/color/344/mysql-logo.png" alt="mysql" width="40" height="40"/>  <img src="https://img.icons8.com/color/344/mongodb.png" alt="mongodb" width="40" height="40"/>  <img src="https://cdn-icons-png.flaticon.com/512/5968/5968520.png" alt="photoshop" width="40" height="40"/>  <img src="https://cdn-icons-png.flaticon.com/512/5968/5968472.png" alt="ilustrator" width="40" height="40"/>
</p>



<hr/>

## 🌐 Últimos Artículos
<!-- Lista dinámica de últimos artículos -->
<!-- Se utiliza JavaScript para obtener y mostrar los últimos artículos desde tu propia API -->
<div id="articles-container"></div>
<script>
  // URL de tu API que entrega un JSON con información de los últimos artículos
  const apiUrl = 'https://reqres.in/api/users?page=2';
  const getArticleInfo = (article) => {
    console.lgo(article);
    const date = new Date(article.date).toLocaleDateString();
    return `- **[${article.title}](${article.url})** - ${date}`;
  };
  // Obtener datos desde tu API
  fetch(apiUrl)
    .then(response => response.json())
    .then(articles => {
        //console.log(articles.data);
      // Obtener el contenedor donde se mostrarán los últimos artículos
      const articlesContainer = document.querySelector('#articles-container');
      // Crear una lista no ordenada para los artículos
      const articlesList = document.createElement('ul');
      // Agregar cada artículo a la lista
      articles.data.forEach(article => {
        const articleItem = document.createElement('li');
        articleItem.innerHTML = `doc: ${article.first_name}`;
        articlesList.appendChild(articleItem);
      });
      // Agregar la lista de artículos al contenedor
      articlesContainer.appendChild(articlesList);
    })
    .catch(error => console.error('Error al obtener los últimos artículos desde la API:', error));
</script>

## 📫 ¡Puedes contactarme a través de mi correo electrónico!
- Correo electrónico: [hola@agustinschwank.com.ar](mailto:hola@agustinschwank.com.ar)

¡Gracias por visitar mi perfil! 🚀
