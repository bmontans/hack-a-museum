<template>
  <div>
    <!-- FORMULARIO -->
    <form>
      <label for="name">Nombre</label>
      <br />
      <input name="name" type="text" placeholder="Tu Nombre" />
      <br />

      <!-- ASUNTO -->
      <label for="subject">Asunto del mensaje</label>
      <br />
      <input name="subject" type="text" placeholder="El asunto" />
      <br />

      <!-- MENSAJE -->
      <label for="textarea">Escribe tu mensaje</label>
      <br />
      <textarea name="textarea" id="textarea" cols="50" rows="4"></textarea>

      <!-- BOTONES -->
      <br />
      <button @click="send()">Enviar</button>
      <button @click="cancel()">Cancelar</button>
    </form>
  </div>
</template>

<script>
import Swal from "sweetalert2";

export default {
  name: "ContactCustom",
  methods: {
    send() {
      Swal.fire(
        "El formulario se ha enviado correctamente.",
        "¡Gracias!",
        "success"
      );
    },
    cancel() {
      Swal.fire({
        icon: "error",
        title: "Oops...",
        text: "Has cancelado el formulario.",
      });
    },
  },
};
</script>

<style scoped></style>
