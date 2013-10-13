<html>
<head>
<title>SISTEMA DE INGRESO PARA CURSO DE DISEÑO GRAFICO</title>
</head>
<body text="016E63" background="fondo.jpg" style="background-repeat:no-repeat">
<div align="center"><H2>BIENVENIDO AL SISTEMA DE INGRESO <br>DEL CURSO DE DISEÑO GRAFICO FACCI ONLINE</H2><br>
<p>Dirigido a Estudiantes Universitarios, Egresados y Profesionales de la Carrera de Ingeniería en Sistemas, personas con conocimientos de
Publicidad, Artes Gráficas, Creativos Gráfico, e Interesados a nivel general.</p>
<div style="border-style:solid; border-color:white; border-widht:2px;"><H4>INGRESE SUS DATOS</H4>
<div> NOMBRES <input type="text" id="name" name="form"></div><br>
<div> APELLIDOS <input type="text" id="apellido" name="form"></div><br>
<div> C.I. <input type="text" id="ci" name="form"></div><br>
<div> CORREO ELECTRONICO <input type="text" id="email" name="form"></div><br>
<div> TELEFONO <input type="text" id="movil" name="form"></div><br>
<div> FECHA NACIMIENTO <input type="date" id="edad" name="form"></div><br>
<div> Seleccionar horario <br>
<input type="radio" id="matu" name="horario" value="matu"> Matutino
<input type="radio" id="vesper" name="horario" value="vesper"> Vespertino</div>
<br><b> INGRESE EN QUE ESPECIAL LE GUSTARIA INCURSIONAR</b><br>
CURSO DE ILUSTRADOR<br>
CURSO DE ADOBE PHOTOSHOP<br>
CURSO DE INDESIGN<br>
COREL DRAW<br>
XARA 3D <br>
IMAGE READY<br>
<input type="text" id="seleccion" name="form">
<input type="button" id="editorseleccion" value="Validar si esta disponible" onclick="seleccioncurso()"><br>
<input type="button" id="aceptar" value="Aceptar" onclick="aceptar1();">
</div>
</body>
</html>

<script type="text/javascript">
function seleccioncurso() {
	if((document.getElementById("seleccion")).value=="CURSO ILUSTRADOR" || (document.getElementById("seleccion")).value=="CURSO DE ADOBE PHOTOSHOP" || (document.getElementById("seleccion")).value=="CURSO DE INDESIGN" ||
	(document.getElementById("seleccion")).value=="COREL DRAW" || (document.getElementById("seleccion")).value=="XARA 3D" || (document.getElementById("seleccion")).value=="IMAGE READY"){
	alert("DISPONIBLE");
	}
	else {alert ("NO ESTA DISPONIBLE!");}
}
function aceptar1 (){
	for(i=0;i<document.getElementsByName("form").length;i++){
		if(document.getElementsByName("form")[i].value=="") {
		alert("DATOS NO INGRESADOS!");
		}else{} 
	}
	if(!document.getElementsByName("form")[0].value=="" && !document.getElementsByName("form")[1].value=="" && !document.getElementsByName("form")[2].value=="" && 
	!document.getElementsByName("form")[3].value=="" && !document.getElementsByName("form")[4].value=="" && !document.getElementsByName("form")[5].value==""){
	
	alert("DATOS COMPLETADOS FELICITACIONES!")}
}
</script>

