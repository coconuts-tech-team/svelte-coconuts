<script lang="ts">
  import { Card, CardTitle, CardHeader, CardBody } from "sveltestrap";

  export let title;
  export let summary;
</script>

<div class="card">
  <Card class="card__description">
    <CardHeader>
      <CardTitle>{title}</CardTitle>
    </CardHeader>
    <CardBody>
      {@html summary}
    </CardBody>
  </Card>
</div>

<style lang="scss">
  .card {
    margin-top: 50px;
    margin-bottom: 50px;
  }
</style>
