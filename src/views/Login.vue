
<template>
  <div>
    <a-row type="flex" justify="space-around" align="middle">
      <a-col :span="8">
        <Form />
      </a-col>
    </a-row>
  </div>
</template>

<script>
// @ is an alias to /src
import Form from "@/components/Form.vue";

export default {
  name: "Login",
  components: { Form },
};
</script>
<style scoped>
</style>