<template>
  <div >
    <a-row>
      <a-col :span="12">
        <a-space>
          Space
          <a-button type="primary">Button</a-button>
          <a-upload>
            <a-button> <a-icon type="upload" /> Click to Upload </a-button>
          </a-upload>
          <a-popconfirm
            title="Are you sure delete this task?"
            ok-text="Yes"
            cancel-text="No"
          >
            <a-button>Confirm</a-button>
          </a-popconfirm>
        </a-space></a-col
      >
      <a-col :span="12"> ffew </a-col>
    </a-row>
    <a-row>
      <a-col :span="24"> dddd </a-col>
    </a-row>
  </div>
</template>


<script>
// @ is an alias to /src

export default {
  name: "Home",
  components: {  },
};
</script>
<style scoped>
</style>