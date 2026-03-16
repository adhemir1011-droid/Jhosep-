<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Para Ti ❤️</title>
<style>
body{
  margin:0;
  font-family: 'Segoe UI', sans-serif;
  color:white;
  display:flex;
  align-items:center;
  justify-content:center;
  min-height:100vh;
  text-align:center;
  background:#ff4b6e;
  overflow:hidden;
}

.hearts{
  position:fixed;
  width:100%;
  height:100%;
  top:0;
  left:0;
  z-index:0;
}

.heart{
  position:absolute;
  color:#ff9bb0;
  font-size:24px;
  animation:float 8s linear infinite;
}

@keyframes float{
  0%{transform:translateY(100vh) scale(1);opacity:0}
  10%{opacity:1}
  100%{transform:translateY(-10vh) scale(1.5);opacity:0}
}

.card{
  position:relative;
  z-index:1;
  max-width:800px;
  padding:40px;
  background:rgba(0,0,0,0.35);
  border-radius:20px;
  backdrop-filter: blur(10px);
}

h1{
  margin-bottom:20px;
}

p{
  line-height:1.7;
  margin-bottom:16px;
  font-size:18px;
}
</style>
</head>
<body>

<div class="hearts" id="hearts"></div>

<div class="card">
<h1>Para ti ❤️</h1>

<p>Hay algo que llevo guardando en el corazón desde hace tiempo, y ya no quiero seguir callándolo. Tal vez estas palabras me den un poco de miedo, porque no sé cómo las vas a recibir, pero lo que siento por ti es demasiado real como para seguir escondiéndolo.</p>

<p>Desde que llegaste a mi vida, todo cambió de una forma que no esperaba. Al principio solo eras alguien con quien hablar, alguien con quien compartir momentos y risas a través de una pantalla. Pero poco a poco te fuiste convirtiendo en alguien mucho más importante para mí… alguien que ocupa un lugar especial en mis pensamientos todos los días.</p>

<p>Hay algo en ti que me atrapó sin que me diera cuenta. Tu forma de ser, tu manera de hablar, tu forma de ver las cosas… todo en ti me parece único. A veces me descubro esperando tus mensajes, pensando en lo que estarás haciendo, o imaginando cómo sería poder estar contigo en persona, hablando de todo y de nada al mismo tiempo.</p>

<p>Y la verdad es que ya no quiero seguir fingiendo que solo eres una amiga para mí, porque en mi corazón sé que eres mucho más que eso. Me gustas… me gustas de una manera profunda, sincera y fuerte. No es algo pasajero ni algo que apareció de un día para otro. Es algo que fue creciendo poco a poco hasta convertirse en algo que ya no puedo ignorar.</p>

<p>Puede que todo haya empezado de forma virtual, pero lo que siento por ti no tiene nada de virtual. Es real, es intenso, y cada día que pasa se vuelve más fuerte. Me importas más de lo que imaginas, y por eso hoy decidí ser completamente sincero contigo.</p>

<p>No te digo esto para presionarte ni para cambiar lo que tenemos si tú no sientes lo mismo. Lo digo porque tú mereces saber lo que hay en mi corazón. Y lo que hay en mi corazón… eres tú.</p>
</div>

<script>
const container = document.getElementById('hearts');

function createHeart(){
  const heart = document.createElement('div');
  heart.classList.add('heart');
  heart.innerHTML = '❤';
  heart.style.left = Math.random()*100 + 'vw';
  heart.style.fontSize = (Math.random()*20 + 20) + 'px';
  heart.style.animationDuration = (Math.random()*5 + 5) + 's';
  container.appendChild(heart);

  setTimeout(()=>{
    heart.remove();
  },8000);
}

setInterval(createHeart,300);
</script>

</body>
</html>
