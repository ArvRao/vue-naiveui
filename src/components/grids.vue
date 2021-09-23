<template>
    <div>
        <n-grid x-gap="12" :cols="3">
    <n-gi>
      <div class="light-green">
          First grid
      </div>
    </n-gi>
    <n-gi>
      <div class="green">
          Second grid
      </div>
    </n-gi>
    <n-gi>
      <div class="light-green">
          Third grid
      </div>
    </n-gi>
    
  </n-grid>
    </div>
</template>

<script>
import { NGrid, NGi } from 'naive-ui'
    export default {
        components: {
            NGrid,
            NGi
        }
    }
</script>

<style scoped>
.light-green {
  height: 108px;
  background-color: rgba(0, 128, 0, 0.12);
}
.green {
  height: 108px;
  background-color: rgba(0, 128, 0, 0.24);
}
</style>