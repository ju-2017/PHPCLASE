# PHPCLASE

SELECCIONAR REGISTROS esto va en controlador formulario

public funtion Ctringreso(){
 if(iseet($_POST["IngresoImail"])){
 
 $tabla = "registros";
 $item = "email";//nombre de la columna que quiero ver la considencia
 $valor = $_POST["IngresoImail"]; //enviar el valor  que ingresan en la caja de texto 
 
 
 $respuesta = ModeloFormulario :: mdlseleccionarregistro($tabla, $item, $valor);
 
 if($respuesta["Email"]==$_POST["IngresoImail"]&&$respuesta["password"])==$_POST["Ingresopassword"]{
 
 $_SESION["validarIngreso"]="ok";
 
 echo'<script>
  
  if(window.history.replaceState){
  
  window.history.replaceState(null, null, window.location.href);
  
  
  }
  
  window.location = "index.php?pagina=inicio"




</script>';
 
 }else
 
 }

}
