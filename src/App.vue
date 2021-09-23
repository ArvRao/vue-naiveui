<template>
  <div>
    <n-loading-bar-provider>
      <n-message-provider>
        <n-notification-provider>
          <n-dialog-provider>
            <h1>Card:</h1>
            <Card />
            <h1>Types of buttons</h1>
            <Button />
            <h1>Basic Grid</h1>
            <Grid />

            <h1>Basic Form</h1>
            <Form />
          </n-dialog-provider>
        </n-notification-provider>
      </n-message-provider>
    </n-loading-bar-provider>
  </div>
</template>

<script>
import Button from "./components/Button.vue";
import Card from "./components/Card.vue";
import Grid from "./components/grids.vue";
import Form from "./components/basicForm.vue";
import {
  NMessageProvider,
  NLoadingBarProvider,
  NNotificationProvider,
  NDialogProvider,
} from "naive-ui";
import { defineComponent } from "vue";

export default defineComponent({
  name: "App",
  components: {
    Button,
    Card,
    Grid,
    Form,
    NMessageProvider,
    NLoadingBarProvider,
    NNotificationProvider,
    NDialogProvider,
  },
});
</script>

<style></style>
