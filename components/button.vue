<template>
  <section @click="open" id="button">
    <p>Read the guide</p>
  </section>
</template>

<script>
export default {
  methods: {
    open() {
      window.open(
        "https://docs.google.com/document/d/e/2PACX-1vTS4E8H8TO9GjqDdtsenza4rXpCnxk9HuPI9wgqIBr169gXCvW0OSmBZtAPuDUkWhhgqHY28T0SURDg/pub"
      );
    },
  },
};
</script>

<style scoped>
#button {
  display: flex;
  width: auto;
  transform: translateY(0px);
  transition: ease-in 200ms;
  height: auto;
  margin: auto;
  margin-top: 30px;
  cursor: pointer;
  background-color: rgb(107, 107, 107);
  border-radius: 20px;
}
#button:hover {
  background-color: rgb(29, 29, 29);
  transform: translateY(-5px);
}
p {
  font-family: "Inter";
  font-size: 24px;
  color: white;
  padding: 20px;
  margin: auto;
}
@media (max-width: 1000px) {
  p {
    font-family: "Inter";
    font-size: 20px;
    color: white;
    padding: 20px;
    margin: auto;
  }
}
</style>