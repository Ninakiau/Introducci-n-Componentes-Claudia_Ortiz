<script >
  export default {
  name: "App",
  data() {
    return {
      RUN: "22.222.222-2",
      apellidos: "MUSK",
      nombres: "ELON REEVE",
      fechaNacimiento: "01/01/1971",
      nacionalidad: "CHILENO",
      sexo: "M",
      fechaNacimiento: "28/06/1971",
      numeroDocumento: "222.222.222",
      fechaEmision: "01/01/2025",
      fechaVencimiento: "01/01/2030",
    };
  },
}

</script>

<template>
<div class="carnet">
      <aside>
        <div>
          <span>CEDULA DE INDENTIDAD</span>
          <img width="40" src="/chile_bandera.png" alt="" />
        </div>

        <img src="/foto_elon.jpg" alt="" />
        <p>RUN {{ RUN }}</p>
      </aside>

      <main>
        <header>
          <p>REPUBLICA DE CHILE</p>
          <span>SERVICIO DE REGISTRO CIVIL E IDENTIFICACIÓN</span>
        </header>
        <section>
          <article>
            <header>APELLIDOS</header>
            <span>{{ apellidos}}</span>
          </article>
          <article>
            <header>NOMBRES</header>
            <span>{{ nombres }}</span>
          </article>

          <div class="grid-2-colums">
            <article>
              <header>NACIONALIDAD</header>
              <span>{{ nacionalidad }}</span>
            </article>
            <article>
              <header>SEXO</header>
              <span>{{ sexo }}</span>
            </article>
          </div>
          <div class="grid-2-colums">
            <article>
              <header>FECHA DE NACIMIENTO</header>
              <span>{{ fechaNacimiento }} </span>
            </article>
            <article>
              <header>NÙMERO DOCUMENTO</header>
              <span>{{ numeroDocumento }}</span>
            </article>
          </div>
          <div class="grid-2-colums">
            <article>
              <header>FECHA DE EMISIÒN</header>
              <span>{{ fechaEmision }}</span>
            </article>
            <article>
              <header>FECHA DE VENCIMIENTO</header>
              <span>{{ fechaVencimiento }}</span>
            </article>
          </div>
          <article>
            <header>FIRMA DEL TITULAR</header>
            <span>X Æ A-12</span>
          </article>
        </section>
      </main>
    </div>

</template>

<style>
body {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 60vh;
        font-size: 10px;
        font-family: sans-serif;
      }

      .carnet {
        width: 400px;
        height: 230px;
        background: #c8deed;
        border-radius: 20px;
        display: grid;
        grid-template-columns: 30% 1fr;
        padding: 20px;
        box-shadow: 0px 0px 10px 2px black;
      }

      aside div {
        display: flex;
      }

      aside > img {
        margin-top: 10px;
        width: 100%;
      }

      aside p {
        text-align: center;
        font-size: 14px;
        font-weight: bold;
      }

      main {
        padding: 0px 0px;
      }

      main article {
        margin: 0px 1px 0px 0px;

      }

      main article header {
        font-weight: bold;
        color: #0235a4;
        font-size: 9px;
      }

      main header p {
        font-size: 20px;
        margin-top: 0px;
        font-weight: bold;
        color: #0235a4;
        margin-left: 15px;
      }

      main header span {
        font-size: 8px;
        color: #399be1;
        margin-left: 15px;
      }

      main section {
        margin-top: 5px;
        margin-left: 15px;
      }

      main section article span {
        font-size: 13px;
        font-weight: 600;
      }

      main section .grid-2-colums {
        display: grid;
        grid-template-columns: 50% 50%;
      }
</style>
