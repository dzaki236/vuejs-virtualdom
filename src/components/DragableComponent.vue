<template>
  <div>
    <div v-html="html"></div>
    <draggable-button class="w-75" style="left: 0px; top: 0px;">
      <div class="card p-2 h-2 shadow">
        <form>
          <div class="form-group">
            <label for></label>
            <textarea v-model="html" class="form-control" name id rows="10"></textarea>
          </div>
        </form>
      </div>
      <div>Ketikkan Sesuatu ↑</div>
    </draggable-button>
  </div>
</template>

<style scoped>
.h-2 {
  height: 20em;
}
</style>
<script>
export default {
  name: "DragableComponent",
  data: () => {
    return {
      html: ""
    };
  },
};
</script>