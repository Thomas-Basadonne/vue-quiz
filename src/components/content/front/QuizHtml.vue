<script>
import Quiz from "../../../views/Quiz.vue";
import AppHeader from "../../_partials/AppHeader.vue";

export default {
  components: {
    Quiz,
    AppHeader,
  },
  data() {
    return {
      title: "HTML",
      htmlQuestions: [
        {
          question: "Cos'è HTML?",
          answer: 3,
          options: [
            "Highly Textual Markup Language",
            "Hyperlink and Text Markup Language",
            "Hyperlink Transfer Markup Language",
            "Hyper Text Markup Language",
          ],
          selected: null,
        },
        {
          question: "Qual è il tag HTML principale?",
          answer: 0,
          options: ["<html>", "<head>", "<body>", "<title>"],
          selected: null,
        },
        {
          question: "Cosa rappresenta il tag <p>?",
          answer: 1,
          options: [
            "Un titolo",
            "Un paragrafo",
            "Un elenco non ordinato",
            "Un'elenco ordinato",
          ],
          selected: null,
        },
        {
          question:
            "Quale tag viene utilizzato per creare un collegamento ipertestuale?",
          answer: 0,
          options: ["<a>", "<link>", "<href>", "<url>"],
          selected: null,
        },
        {
          question: "Qual è il tag per creare una lista non ordinata?",
          answer: 2,
          options: ["<ol>", "<li>", "<ul>", "<dl>"],
          selected: null,
        },
        {
          question:
            "Quale attributo HTML è utilizzato per specificare un collegamento ipertestuale?",
          answer: 2,
          options: ["link", "src", "href", "url"],
          selected: null,
        },
        {
          question:
            "Qual è il tag per creare un'intestazione di primo livello?",
          answer: 0,
          options: ["<h1>", "<h2>", "<h3>", "<h4>"],
          selected: null,
        },
        {
          question: "Qual è il tag HTML per l'immagine?",
          answer: 2,
          options: ["<image>", "<picture>", "<img>", "<photo>"],
          selected: null,
        },
        {
          question: "Cosa rappresenta il tag <br>?",
          answer: 0,
          options: [
            "Un'interruzione di riga",
            "Un paragrafo",
            "Un titolo",
            "Un collegamento",
          ],
          selected: null,
        },
        {
          question:
            "Quale elemento HTML rappresenta un elemento di input del modulo?",
          answer: 1,
          options: ["<text>", "<input>", "<form>", "<button>"],
          selected: null,
        },
      ],
    };
  },
};
</script>

<template>
  <AppHeader />
  <Quiz :questions="htmlQuestions" :title="title" />
</template>

<style lang="scss" scoped></style>
