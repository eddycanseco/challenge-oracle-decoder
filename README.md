 <h1 align="center">Proyecto Encriptador / Desencriptador de Texto</h1>
    <h2>Objetivo del Proyecto</h2>
         <p>La finalidad es desarrollar, utilizando los conocimiento adquiridos en los cursos de JavaScript,
             HTML y CSS, una aplicacion que pueda realizar las operaciones de encriptar y tambien desencriptar 
             un texto formado exclusivamente por letras minusculas, cualquier otro caracter como caracteres 
             especiales, letra mayusculas o minusculas acentuadas seran consideradas como caracteres prohibidos
            y la operacion no podra efectuarse.
         </p>
    <h3>Funcionalidades</h3>
         <p>La aplicacion tiene tres botones y dos areas de desplegado de texto, cuyo proposito es:
            <u1>
                 <li>Area de captura de texto.</li>
                 <li>Area de desplegado de resultado de las operaciones de encriptar o desencriptar o error.</li>
                 <li>Boton para encriptar texto.</li>
                 <li>Boton para desencriptar texto.</li>
                 <li>Boton para copiar texto, del area de resultado al de captura de texto, esto para facilitar la validacion
                   de las operaciones.</li>
            </u1>
         </p>
    <h4>Uso de la Aplicacion </h4>
         <p>La pantalla despliega dos areas de texto, la ubicada del lado izquierdo es donde 
            se captura el texto al cual se le aplicara el algoritmo para encriptarlo o desencriptar. 
            Del lado derecho, debajo de la imagen, aparece un espacio en donde se desplegara el resultado de las acciones
            de encriptamiento o desencriptamiento del texto capturado.
            Del lado izquierdo de la pantalla aparecen tres botones, dos de ellos alineados y que corresponden a las
            operaciones de encriptar y desencriptar respectivamente. Abajo de estos botones se encuentra el correspondiente
            a la accion de copiar, y la accion que realiza es la  de copiar el resultado hacia el area correspondiente de captura 
            de texto para poder aplicarle, por ejemplo, la accion inversa y validar la operacion seleccionada previamente.
            Cabe aclarar que el boton "COPIAR" inicialmente esta deshabilitado y pretende simular un CTRL-C y CTRL-V.
         </p>
    <h5>Mejora a la Aplicacion</h5>
         <p>
          La funcionalidad de copiar en realidad solo simula la operacion de ctrl-c y ctrl-v, una mejora consiste
          en implementar el siguiente codigo que fue proporcionado por Chatgpt a solicitud expresa mia. Se probo y
          funciona, pero aun no lo entiendo a cabalidad. Lo dejare para mas adelante y una vez comprendido se 
          actualizara tal funcionalidad. 
         </p>
     <h6>Codigo a Incorporar en un futuro proximo:</h6>
     <p> 
          document.getElementById('copyButton').addEventListener('click', function() {
               const textArea = document.getElementById('textArea');
               textArea.select();
               document.execCommand('copy');
               alert('Texto copiado al portapapeles');
            }
        );
     </p>
     <p>
          document.getElementById('pasteButton').addEventListener('click', function() {
               navigator.clipboard.readText().then(text => {
                   document.getElementById('textArea').value = text;
               }).catch(err => {
               console.error('Error al pegar el texto: ', err);
               });
          }
       );
     </p> 
