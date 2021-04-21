<template>
  <div class="min-h-screen min-w-screen bg-gray-100 flex pt-10 justify-center">
    <div>
      <div class="flex flex-col max-w-md bg-white px-8 py-6 rounded-xl space-y-5">
        <h3 class="font-serif font-bold text-gray-900 text-xl">Омлет с овощами</h3>
        <img class="w-full rounded-md" src="../static/img/photo.png" alt="pizza" />
        <div class='row'>
          <div class='column'>
            <div class='first-column'>
              <star-icon class="pr-1"/>
              <star-icon class="pr-1"/>
              <star-icon class="pr-1"/>
              <star-icon class="pr-1"/>
              <star-icon class="pr-1"/>
            </div>
            <p class="text-xs">5 Star Rating</p>
          </div>
          <div class='column'>
            <div class='second-column'>
              <img class="h-10 ml-12" src="../static/img/logo/logo.png" alt="logo" />
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
                class="ml-12"
                title="20 min"
                type="primary"
                :svgIcon="'timerIcon'"
              />
            </div>
          </div>
        </div>
        <p class="font-bold text-left font-rest-black text-base">Description</p>
        <p class="leading-relaxed text-sm font-rest-black">Lorem Contrary to popular belief, Lorem Ipsum is not simply random text.</p>
        <p class="font-rest-black text-xs"><span class="font-bold">Calorie of food(kcal):</span> 299</p>
        <nuxt-link to="/"
                   class="px-24 py-4 bg-rest-yellow rounded-md text-white focus:border-transparent"
        ><rest-button
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
</style>
