<template>
  <div class="presentation-gif">
    <img
      src="../assets/PresentationGif.gif"
      alt="Hi, I'm Gabriel a FullStack developer"
    />
  </div>
  <div class="typewriter">
    <h1>
      The technologies that I'm used to are <br />
      VueJS, NodeJS, Serverless and AWS
    </h1>
  </div>
</template>

<script setup>
import { computed } from "vue";

const teste = "abcd";

const testMethod = (prop1, prop2) => {
  switch (prop1) {
    case "teste1":
      console.log("aaaa");
      break;
    case "teste2":
      console.log("bbbb");
      break;
    default:
      console.log("testMethod");
      break;
  }
};

//create a computed
const testComputed = computed(() => {
  return "computed value";
});
</script>

<style>
.presentation-gif {
  display: block;
  margin-left: auto;
  margin-right: auto;
  margin-bottom: 15%;
  width: 40%;
}

.technologies {
  font-size: 25px;
  line-height: 1.1;
  font-weight: 600;
  letter-spacing: 0em;
  font-family: SF Pro Display, SF Pro Icons, Helvetica Neue, Helvetica, Arial,
    sans-serif;
}

.typewriter {
  display: flex;
  justify-content: center;
  align-items: center;
}

.typewriter h1 {
  overflow: hidden; /* Ensures the content is not revealed until the animation */
  border-right: 0.15em solid black; /* The typwriter cursor */
  white-space: nowrap; /* Keeps the content on a single line */
  margin: 0 auto; /* Gives that scrolling effect as the typing happens */
  letter-spacing: 0.15em; /* Adjust as needed */
  animation: typing 3.5s steps(40, end), blink-caret 0.75s step-end infinite;
  font-family: SF Pro Display, SF Pro Icons, Helvetica Neue, Helvetica, Arial,
    sans-serif;
}

/* The typing effect */
@keyframes typing {
  from {
    width: 0;
  }
  to {
    width: 40%;
  }
}

/* The typewriter cursor effect */
@keyframes blink-caret {
  from,
  to {
    border-color: transparent;
  }
  50% {
    border-color: black;
  }
}
</style>
