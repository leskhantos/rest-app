<template>
  <div class="">
    <div>
      <img class="bg-photo" src="../static/img/photo.png" height="229px" alt="pizza"/>
      <div class=" flex flex-col max-w-md px-8 py-4 space-y-5" style="border-radius:20px;background-color:white;margin-top: 200px">
        <h3 class="font-bold text-rest-blacker text-xl">Паста Медлей</h3>
        <div class='row'>
          <div class='column'>
            <div class='first-column'>
              <star-icon class="pr-1"/>
              <star-icon class="pr-1"/>
              <star-icon class="pr-1"/>
              <star-icon class="pr-1"/>
              <star-icon class="pr-1"/>
            </div>
            <p class="text-xs text-rest-blacker">5 Star Rating</p>
          </div>
          <div class='column'>
            <div class='second-column'>
              <img class="h-9 ml-20" src="../static/img/logo/logo.png" alt="logo" />
            </div>
          </div>
        </div>
        <div class='row'>
          <div class='column'>
            <div class='first-column text-xs'>
              <rest-button
                title="Share"
                type="primary"
                :svgIcon="'shareIcon'"
              />
            </div>
          </div>
          <div class='column'>
            <div class='second-column text-xs' >
              <rest-button
                class="ml-20"
                title="20 min"
                type="primary"
                :svgIcon="'timerIcon'"
              />
            </div>
          </div>
        </div>
        <p class="font-bold text-left text-rest-blacker text-base">Description</p>
        <p class="leading-relaxed text-sm text-rest-blacker">Lorem Contrary to popular belief, Lorem Ipsum is not simply random text.</p>
        <p class="text-rest-blacker text-xs"><span class="font-bold">Calorie of food(kcal):</span> 299</p>
        <nuxt-link to="/"
                   class="px-20 py-1 bg-rest-yellow text-xs rounded-md text-white focus:border-transparent"
        ><rest-button
          class="ml-4"
          title="Watch video"
          type="primary"
          :svgIcon="'videoIcon'"
        /></nuxt-link>
      </div>
    </div>
  </div>
</template>

<script>
import StarIcon from "../components/icons/starIcon";
export default {
  name: "detail",
  components: {StarIcon},
}
</script>

<style scoped>

.row {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  width: 100%;
}

.column {
  display: flex;
  flex-direction: column;
  flex: 1;
}

.first-column {
  height: 100%;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
}

.second-column {
  text-align: right;
  height: 100%;
}
.bg-photo {
  position: absolute;
  left: 0;
  top: 0;
  z-index: -1;
}
</style>
