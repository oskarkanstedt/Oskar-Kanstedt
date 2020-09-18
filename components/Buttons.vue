<template>
  <div>
    <b-button :to="to" variant="secondary" class="button">{{
      buttonText
    }}</b-button>
  </div>
</template>

<script>
export default {
  props: {
    buttonText: String,
    to: String,
  },
}
</script>

<!--Här har jag skapat en komponent för knapparna i min meny. Detta för att förenkla när jag kallar på dessa i mina .vue pages-->
