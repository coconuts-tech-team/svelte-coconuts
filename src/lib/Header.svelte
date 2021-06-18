<script lang="ts">
  import swal from "sweetalert";

  const home = () => {
    swal("Hellow world");
  };
</script>

<div class="header">
  <button on:click={home}> ほーむ </button>
  aaaa
</div>

<style lang="scss">
  .header {
    height: 50px;
    vertical-align: middle;
    background-color: aqua;
  }
</style>
