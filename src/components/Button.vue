<template>
  <n-space align="center">
    <n-button color="#8a2be2">
      <template #icon>
        <n-icon>
          <cash-icon />
        </n-icon>
      </template>
      #8a2be2
    </n-button>
    <n-button color="#ff69b4">
      <template #icon>
        <n-icon>
          <cash-icon />
        </n-icon>
      </template>
      #ff69b4
    </n-button>
    <n-button ghost color="#8a2be2">
      <template #icon>
        <n-icon>
          <cash-icon />
        </n-icon>
      </template>
      #8a2be2
    </n-button >
    <n-button ghost color="#ff69b4">
      <template #icon>
        <n-icon>
          <cash-icon />
        </n-icon>
      </template>
      #ff69b4
    </n-button>

    <n-button text color="#8a2be2">
      <template #icon>
        <n-icon>
          <cash-icon />
        </n-icon>
      </template>
      Custom color
    </n-button>
  
    <n-button round>Round</n-button>
    <n-button :bordered=False>Rect</n-button>

    <br>
    Tooltip:
  <br>
  <n-tooltip trigger="hover">
    <template #trigger>
      <n-button> Name </n-button>
    </template>
    Either First or last or your nick name
  </n-tooltip>
 <br />


    <br>
    <h1>Modal</h1>
    <h1><n-button @click="showModal = true" round text color="#2b8ae2">Sample model</n-button>
  <n-modal v-model:show="showModal"> <!--n-modal takes show prop as argument -->
    <n-card style="width: 600px;" title="Sample Model" :bordered="false" size="huge">
      <template #header-extra> Sidebars</template>
      Content
      <template #footer> Footer </template>
    </n-card>
  </n-modal></h1>
  </n-space>
</template>

<script>
import { NButton, NModal, NCard, NTooltip } from 'naive-ui'
import { CashOutline as CashIcon } from '@vicons/ionicons5'
import { defineComponent, ref } from 'vue'
  export default defineComponent ({
    name: 'Button',
   
    components: {
      NButton,
      CashIcon,
      NModal,
      NCard,
      NTooltip
    },
    setup () {
    return {
      showModal: ref(false)
    }
  }
  })
</script>

<style scoped>

</style>