<template>
  <div style="display:grid;place-items:center;" @click="dialog = true">
    <v-icon class="text-h1 d-block mx-auto">
      mdi-shield-check
    </v-icon>
    <span class="text-subtitle-1">Internet Sano</span>
    <v-dialog
      v-model="dialog"
      width="90%"
    >
      <v-card>
        <v-card-title class="text-h5 grey lighten-2">
          Conoce como llevar un uso sano del internet
        </v-card-title>

        <v-card-text>
          En el mundo actual, donde todo gira alrededor de la tecnología, debemos tener conciencia y darle un buen uso a esa herramienta que ahora es indispensable para la realización de todas nuestras actividades diarias. <br>
          Es así como nuestros niños, niñas y adolescentes están cada vez más involucrados en esta evolución lo que genera un riesgo constante si, como adultos, no estamos al tanto del contenido de la red.<br><br>

          Por lo anterior y en búsqueda de su protección, el Gobierno Nacional expidió la Ley 679 del 2001 y el decreto 1524 del 2004, normas que buscan prevenir y contrarrestar el Material de Abuso de Niñas, Niños y Adolescentes.<br><br>

          Ley 679 de 2001<br><br>

          Decreto 1524 de 2002<br>
          Esta estrategia del Ministerio de Tecnologías de la Información y las Comunicaciones hace un llamado a toda la comunidad en general para que denuncie y participe en la prevención de la explotación sexual de nuestros menores de edad, y así mismo busca promover una comunicación permanente con los adultos responsables y maestros para incentivar el uso de un Internet Sano.<br>
          Como cumplimiento de lo anterior fue creado el sitio web www.internetsano.gov.co donde los ciudadanos pueden realizar denuncias de sitios en Internet, que vayan en contravía de las normas, las cuales son remitidas a la Oficina de Delitos Informáticos de la DIJIN – Policía Nacional y posteriormente bloqueados a través de solicitudes realizadas por el Ministerio de Tecnologías de la Información y las Comunicaciones a los proveedores de Acceso a Internet.<br><br>

          DIRECCIÓN CENTRAL DE POLICÍA JUDICIAL - DIJIN<br>
          GRUPO INVESTIGATIVO DELITOS INFORMÁTICOS<br>
          Teléfono: PBX: 426 6900 Ext. 6301-6302<br>
          <a href="https://www.policia.gov.co/dijin">https://www.policia.gov.co/dijin</a><br><br>

          MINISTERIO DE TECNOLOGÍAS DE LA INFORMACIÓN Y LAS COMUNICACIONES<br>
          Línea de atención gratuita: 01 800 0912667<br>
          <a href="http://www.enticconfio.gov.co">http://www.enticconfio.gov.co</a><br>
          Internet Sano también cuenta con un grupo de profesionales, quienes te orientarán con las denuncias y así promover el buen uso de la red. Esta estrategia contempla también la conformación de Brigadas de Voluntarios en Alfabetización conformadas por niñas, niños y adolescentes para que ayuden a sus padres y adultos cercanos a convertirse en Ciudadanos Digitales.<br>
          Para mayores informes comunícate con el ministerio:<br><br>

          MINISTERIO DE TECNOLOGÍAS DE LA INFORMACIÓN Y LAS COMUNICACIONES<br>
          EDIFICIO MURILLO TORO<br>
          Carrera 8 entre calles 12 y 13, Bogotá D.C.<br>
          Teléfono: (571) 3443460<br>
          <a href="http://www.mintic.gov.co">http://www.mintic.gov.co</a><br>
        </v-card-text>

        <v-divider />

        <v-card-actions>
          <v-btn
            color="primary"
            @click="dialog = false"
          >
            Finalizar
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
  </div>
</template>
<script>
export default {
  data () {
    return {
      dialog: false
    }
  }
}
</script>
