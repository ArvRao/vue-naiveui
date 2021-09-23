<template>
    <div>
        
        <n-carousel show-arrow autoplay>
    <img
      class="carousel-img"
      src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRiXULuZwOmvyThRxDX-IabvFEZMeRfNryZvQ&usqp=CAU"
    />
    <img
      class="carousel-img"
      src="https://s.anw.red/news/1623177220.jpg!/both/800x450/quality/78/progressive/true/ignore-error/true"
    />
    <img
      class="carousel-img"
      src="https://s.anw.red/news/1623152423.jpg!/both/800x450/quality/78/progressive/true/ignore-error/true"
    />
  </n-carousel>


        <n-card title="Arvind" size='huge' bordered=true>I study in DSCE, telecom final year</n-card>

        <n-card title="Card with Cover">
    <template #cover>
      <img src="@/assets/passport_pic.jpg" width="50px"/>
    </template>
    Card Content
  </n-card>

  <n-card content-style="padding: 0;">
    <n-tabs
      type="line"
      size="large"
      :tabs-padding="20"
      pane-style="padding: 20px;"
    >
      <n-tab-pane name="FRONTEND">
          I use Vue.js library for UI styling of my apps
      </n-tab-pane>
      <n-tab-pane name="BACKEND">
          Django and Django REST library for building APIs which is later sent to
          Vue app in the frontend for data communication with the help of axios HTTP library
      </n-tab-pane>
    </n-tabs>
  </n-card>

    <div style="position:relative; left:80px; top:2px;">
<n-collapse arrow-placement="right">
    <n-collapse-item title="Schoolings" name="1">
      <div>
          <ul>
              <li>Adarsha Public School</li>
              <li>Daffodils</li>
              <li>Ryan</li>
              <li>Chaitanya</li>
              <li>Shiksha Sagar</li>
          </ul>
      </div>
    </n-collapse-item>
    <n-collapse-item title="College" name="2">
      <div>
          <ul>
              <li>Seshadripuram Composite</li>
          </ul>
      </div>
    </n-collapse-item>
    <n-collapse-item title="Hobbies" name="3">
      <div>
          <ul>
              <li>Chess</li>
              <li>Reading</li>
              <li>Hiking</li>
          </ul>
      </div>
    </n-collapse-item>
  </n-collapse>
    </div>
    </div>
  
</template>

<script>
import { NCard, NTabs, NTabPane, NCarousel, NCollapse, NCollapseItem } from 'naive-ui'
    export default {
        name: "Card",
    components: {
        NCard,
        NTabs,
        NTabPane,
        NCarousel,
        NCollapse,
        NCollapseItem
    }
    
}
</script>

<style scoped>
.n-card {
  max-width: 300px;
}


.carousel-img {
  width: 100%;
  height: 240px;
  object-fit: cover;
}
</style>