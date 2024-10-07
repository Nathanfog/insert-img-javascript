# insert-img-javascript
Inserir-imagem-javascript


<script>
//Só executa se o DOM estar carregado
if (document.readyState=="loading") document.addEventListener('DOMContentLoaded', IniciarCode);
else IniciarCode();

function IniciarCode() {

  const imageContainer = document.querySelector('.itemVideo .videoIconeGaleria');

  const playButton = document.createElement('div');
  playButton.classList.add('playButton');

  // Create an image element and set the source to your desired image link
  const playImage = document.createElement('img');
  playImage.src = 'https://static.lojadopapel.com.br/media/wysiwyg/magemenu/playdemo.png'; // Replace with your actual image path

  // Append the image to the play button element
  playButton.appendChild(playImage);

  imageContainer.appendChild(playButton);
}



</script>

<style>

.playButton {
    position: absolute;
    width: 40px;
    height: 40px;

    border-radius: 50%;
    color: white;
    display: flex;
    font-size: 24px;
    z-index: 50;
}

.playButton img {
  width: 100%;
  height: 100%;
  object-fit: cover; 
}

.videoIconeGaleria {
    display: flex;
    justify-content: center;
    align-items: center;
}

</style>
