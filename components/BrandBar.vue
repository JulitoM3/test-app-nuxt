<template>
  <b-container>
    <b-row>
      <b-col md="6">
        <brand-name/>
      </b-col>
      <b-col md="6">
        <Nav/>
      </b-col>
    </b-row>
  </b-container>
</template>
<script>
import BrandName from "./BrandName";
import Nav from "./Nav";

export default {
  components: {Nav, BrandName}
}
</script>
