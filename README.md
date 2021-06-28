<html>
<head>
<meta charset="UTF-8">
<title>CANVAS</title>
<style>
#miCanvas{	border:dotted 2px yellow;
				background:green;	}
</style>
<script>
window.onload = function(){
	var canvas = document.getElementById("miCanvas");
	if(canvas && canvas.getContext){
		var ctx = canvas.getContext("2d");
		if(ctx){

			//Degrade Fondo
			var gradiente = ctx.createLinearGradient(0,0,0,canvas.height);
			gradiente.addColorStop(0.3, "red");
			gradiente.addColorStop(0.5, "White");
			gradiente.addColorStop(0.7, "blue");
			
			ctx.fillStyle = gradiente;
			ctx.fillRect(0,0,canvas.width,canvas.height);
			//Insertar Imagen
			var imagen = new Image();
			function procesaImagen(){
				ctx.drawImage(imagen,200,200,800,400);
			}
			imagen.src = "moto.jpg";
			imagen.onload = function(e){
				procesaImagen();
			}


			//Descripcion de lineas
			ctx.lineWidth = 24;
			ctx.strokeStyle = "black";
			///Linea Vertical E
			ctx.beginPath();
			ctx.lineTo(50,50);
			ctx.lineTo(50,150);
			ctx.stroke();
			//Primea linea E
			ctx.lineCap = "round";
			ctx.moveTo(50,50);
			ctx.lineTo(120,50);
			ctx.stroke();
			//Segunda linea E
			ctx.lineCap = "round";
			ctx.moveTo(50,100);
			ctx.lineTo(120,100);
			ctx.stroke();
			//Tercera linea E	
			ctx.lineCap = "round";
			ctx.moveTo(50,150);
			ctx.lineTo(120,150);
			ctx.stroke();
			//Linea Vertical I
			ctx.beginPath();
			ctx.lineTo(170,50);
			ctx.lineTo(170,150);
			ctx.stroke();
			//Linea Vertical D
			ctx.beginPath();
			ctx.lineTo(220,50);
			ctx.lineTo(220,150);
			ctx.stroke();
			//Primea linea D
			ctx.lineCap = "round";
			ctx.moveTo(220,50);
			ctx.lineTo(270,60);
			ctx.stroke();
			//Segunda linea D
			ctx.lineCap = "round";
			ctx.moveTo(220,150);
			ctx.lineTo(270,140);
			ctx.stroke();
			//Tercera linea D
			ctx.lineCap = "round";
			ctx.moveTo(270,60);
			ctx.lineTo(290,80);
			ctx.stroke();
			//Cuarta linea D
			ctx.lineCap = "round";
			ctx.moveTo(270,140);
			ctx.lineTo(290,130);
			ctx.stroke();
			//2DA Linea Vertical D
			ctx.lineTo(290,80);
			ctx.lineTo(290,130);
			ctx.stroke();
			//Linea Vertical E
			ctx.beginPath();
			ctx.lineTo(340,50);
			ctx.lineTo(340,150);
			ctx.stroke();
			//Primea linea E
			ctx.lineCap = "round";
			ctx.moveTo(340,50);
			ctx.lineTo(410,50);
			ctx.stroke();
			//Segunda linea E
			ctx.lineCap = "round";
			ctx.moveTo(340,100);
			ctx.lineTo(410,100);
			ctx.stroke();
			//Tercera linea E	
			ctx.lineCap = "round";
			ctx.moveTo(340,150);
			ctx.lineTo(410,150);
			ctx.stroke();
			//1era Linea Vertical R
			ctx.beginPath();
			ctx.lineTo(460,50);
			ctx.lineTo(460,150);
			ctx.stroke();
			//Primea linea R
			ctx.lineCap = "round";
			ctx.moveTo(460,50);
			ctx.lineTo(510,50);
			ctx.stroke();
			//Segunda linea R
			ctx.lineCap = "round";
			ctx.moveTo(460,100);
			ctx.lineTo(510,100);
			ctx.stroke();
			//2da Linea Vertical R
			ctx.lineTo(510,50);
			ctx.lineTo(510,100);
			ctx.stroke();	
			//Tercera linea R
			ctx.lineCap = "round";
			ctx.moveTo(510,100);
			ctx.lineTo(520,110);
			ctx.stroke();
			//Cuarta linea R
			ctx.lineCap = "round";
			ctx.moveTo(520,110);
			ctx.lineTo(530,150);
			ctx.stroke();
			//Linea Vertical M
			ctx.beginPath();
			ctx.lineTo(620,50);
			ctx.lineTo(620,150);
			ctx.stroke();
			//Primea linea M
			ctx.lineCap = "round";
			ctx.moveTo(620,50);
			ctx.lineTo(655,90);
			ctx.stroke();
			//Segunda linea M
			ctx.lineCap = "round";
			ctx.moveTo(655,90);
			ctx.lineTo(690,50);
			ctx.stroke();
			//Linea Vertical M
			ctx.lineCap = "round";
			ctx.moveTo(695,50);
			ctx.lineTo(695,150);
			ctx.stroke();
			//1era Linea Vertical O
			ctx.beginPath();
			ctx.lineTo(745,50);
			ctx.lineTo(745,150);
			ctx.stroke();
			//Primea linea O
			ctx.lineCap = "round";
			ctx.moveTo(745,50);
			ctx.lineTo(800,50);
			ctx.stroke();
			//Segunda linea O	
			ctx.lineCap = "round";
			ctx.moveTo(745,150);
			ctx.lineTo(800,150);
			ctx.stroke();
			//2da Linea Vertical O
			ctx.beginPath();
			ctx.lineTo(800,50);
			ctx.lineTo(800,150);
			ctx.stroke();
			//1era Linea Vertical R
			ctx.beginPath();
			ctx.lineTo(850,50);
			ctx.lineTo(850,150);
			ctx.stroke();
			//Primea linea R
			ctx.lineCap = "round";
			ctx.moveTo(850,50);
			ctx.lineTo(900,50);
			ctx.stroke();
			//Segunda linea R
			ctx.lineCap = "round";
			ctx.moveTo(850,100);
			ctx.lineTo(900,100);
			ctx.stroke();
			//2da Linea Vertical R
			ctx.lineTo(900,50);
			ctx.lineTo(900,100);
			ctx.stroke();	
			//Tercera linea R
			ctx.lineCap = "round";
			ctx.moveTo(900,100);
			ctx.lineTo(910,110);
			ctx.stroke();
			//Cuarta linea R
			ctx.lineCap = "round";
			ctx.moveTo(910,110);
			ctx.lineTo(920,150);
			ctx.stroke();
			//1era Linea Vertical A
			ctx.beginPath();
			ctx.lineTo(970,50);
			ctx.lineTo(970,150);
			ctx.stroke();
			//Primea linea A
			ctx.lineCap = "round";
			ctx.moveTo(970,50);
			ctx.lineTo(1030,50);
			ctx.stroke();
			//Segunda linea A
			ctx.lineCap = "round";
			ctx.moveTo(970,100);
			ctx.lineTo(1030,100);
			ctx.stroke();
			//2da Linea Vertical A
			ctx.beginPath();
			ctx.lineTo(1030,50);
			ctx.lineTo(1030,150);
			ctx.stroke();
		} else {
			alert("Error al crear tu contexto");	
		}
	}
}
</script>
</head>
<body background="fondo.jpg"
<h1>  INGRESA AL JUEGO </h1>
<canvas id="miCanvas" width="1200px" height="650px">
Tu navegador no soporta CANVAS
</canvas>
</body>
</html>
