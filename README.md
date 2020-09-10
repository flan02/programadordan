<!DOCTYPE html>
<html lang="es-AR">
<meta charset="utf-8">
<head>
<style type="text/css">
html{
	background-color: #222;
	font: 20px Garamond;
	color: #139;
	
	 
}	

#cv{
	        color: #FFF;
	        font: 28px Garamond;
	        position: absolute;
	        left: 370px;
	        top: 50px;
	       
	       

}

#foto_perfil{
    position:absolute; 
	margin-top: 0;
	border: 2px solid #FFF;
}


#center{
     
    width: 900px; height: 730px; 
	margin-left: 200px;
	margin-right: 200px;
	background: #000;
}

.cont{

	position: relative;
	display: inline-block;
	text-align: center;

}

.subtitulo{
	text-align: center;
}

.main .impar{

       margin-top:-30px; 
       background-color: #009;
       color: #FFF;
     /*   padding-bottom: 3px; 
        padding-top: 3px;*/
 padding-bottom: 3px; 
}

.main .impar:hover{

       background-color: #FFF;
       color: #009; 
     /*   padding-bottom: 3px; 
        padding-top: 3px;*/

}



</style>

<title></title>

</head>

<body>

<div id="center">	

<header>

<img src="../../../Mis Datos/Desktop/curriculum/perfil.jpg"/ alt="Foto de perfil" width="150" height="150" id="foto_perfil">	

<div id="cont">

	<img src="../../../Mis Datos/Desktop/curriculum/banner.png"/ alt="Banner del perfil" width="900" height="153" id="banner_perfil">

<h1 id="cv"></h1>

</div>

</header>

<main class="main">
	
<article class="impar">	


<h2 class="subtitulo">Datos Personales</h2>
<ul>
	<li>Apellido y Nombre: Chanivet, Dan</li>
	<li>Edad: 32</li>
	<li>Lugar de residencia: San Justo, Zona oeste. Buenos Aires</li>
	<li>Email: chanivetdan@hotmail.com</li>
	<li>Telefono: 15-5259-1618</li>
	<li>Profesion: Entrenador de Basquet / Desarrollador Web / Programador </li>

</ul>

</article>

<article class="impar">	


<h2 class="subtitulo">Formacion Academica</h2>
<ul>
	<li>Escuela Primaria: Instituto Maria Mazzarello, Moron Buenos Aires.</li>
	<li>Escuela Secundaria: Instituto Maria Mazzarello, Moron Buenos Aires.</li>
	<li>CENARD, Entrenador Nacional de Basquet</li>
	<li>Curso JAVA SE, JAVA Beans, Aplicaciones de escritorio</li>
	<li>Actualmente: Ingenieria Mecanica, Universidad Nacional de la Matanza. 2do año</li>

</ul>
</article>

<article class="impar">	


<h2 class="subtitulo">Tecnologias de programacion. Front end / Back end</h2>
<ul>
	<li>HTML5 --> HTML, CSS3, JAVASCRIPT.</li>
	<li>JAVA SE</li>
	<li>PHP7+</li>
	<li>SQL - MySql</li>

</ul>
</article>

</main>

</div>

</body>

<script type="text/javascript">
	
var x = document.getElementById('cv');

let wrt = str => {

	let arrFromStr = str.split('');

	let i = 0;

	let printStr = setInterval(function(){

		if(arrFromStr[i] === ' '){

		

			x.innerHTML += arrFromStr[i];

			x.innerHTML += arrFromStr[i + 1];

			i += 2;

		} else {

			x.innerHTML += arrFromStr[i];

			i++;

		}

		if(i === arrFromStr.length - 1){

			clearInterval(printStr);

			x.style.color = '#FFF';

		}

	}, 150);

};



wrt('...{ Curriculum Vitae: Dan Chanivet, full StackWeb Developer }....');


</script>

</html>
