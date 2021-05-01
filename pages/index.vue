<template>
  <div class='header-wrapper' :style="{ backgroundImage: `url(${image})`}">
    <div class='row'>
      <div class='column'>
        <div class='first-column text-3xl'>
          <h3 class="text-rest-blacker mt-7 text-xl font-bold">DIResto</h3>
        </div>
      </div>
      <div class='column ml-24'>
        <div class='second-column'>
          <img src="../static/img/logo/logo.png" width="126px" height="61px" alt="logo" />
        </div>
      </div>
    </div>
    <form class="mb-4 w-347 h-47 md:mb-0 md:w-1/4 pt-4">
      <label class="hidden" for="">Search</label>
      <input class="bg-grey-lightest border-2 focus:border-orange p-2 rounded-full shadow-inner w-full" placeholder="Поиск еды" type="text">
      <button class="hidden">Submit</button>
    </form>
    <h3 class="font-bold">Обеды</h3>
    <div class="holder h-348 w-437 grid sm:grid-cols-1 md:grid-cols-3 lg:grid-cols-4 rounded-md shadow-sm">
      <div class="each mb-10 m-2 border-gray-800 bg-gray-100 relative rounded-2xl">
        <h1 class="font-bold text-xl p-3">Паста Медлей</h1>
        <nuxt-link to="/detail" class="badge absolute top-5 right-0 m-1 text-rest-yellow  px-2 text-xs rounded">Состав</nuxt-link>
        <iframe src="https://player.vimeo.com/video/25312553" class="w-full" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen>
        </iframe>
        <div class="info-box text-xs flex p-1 font-semibold text-rest-yellow">
          <span class="p-1"><star-icon/></span>
          <span class="mr-1 p-1 font-bold text-gray-500">(124 ratings) Завтрак</span>
        </div>
        <hr>
        <div class='row'>
          <div class='column'>
            <div class='first-column text-xs p-2'>
              <rest-button
                title="20 min"
                type="primary"
                :svgIcon="'timerIcon'"
              />
            </div>
          </div>
          <div class='column'>
            <div class='second-column text-xs p-2 ml-11' >
              <rest-button
                class="ml-11"
                title="Share"
                type="primary"
                :svgIcon="'shareIcon'"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class='row'>
      <div class='column'>
        <div class='first-column'>
          <p class="font-bold text-rest-blacker">Популярная еда</p>
        </div>
      </div>
      <div class='column'>
        <div class='second-column'>
          <p class="text-rest-yellow">Посмотреть все</p>
        </div>
      </div>
    </div>
    <div class="max-w-2xl pt-2 p-5 rounded-md tracking-wide">
      <div  class="flex">
        <img alt="pizza" class="w-45 rounded-md border-2 border-gray-300" src="https://img.pizza/75/75" />
        <div  class="flex flex-col ml-5">
          <p class="text-base text-rest-blacker font-semibold mb-2">Пицца Маргарита</p>
          <p  class="text-rest-gray mb-2">Завтрак ~ Пицца</p>
          <div class="flex">
            <star-icon class="mr-2"/>
            <span class="text-rest-yellow text-xs">4.9</span>
            <span class="mr-1 px-2 text-rest-gray text-xs">(124 ratings)</span>
          </div>
        </div>
      </div>
    </div>
    <div class="max-w-2xl pt-2 p-5 rounded-md tracking-wide">
      <div id="header" class="flex">
        <img alt="mountain" class="w-45 rounded-md border-2 border-gray-300" src="https://img.pizza/75/75" />
        <div id="body" class="flex flex-col ml-5">
          <p class="text-base text-rest-blacker font-semibold mb-2">Пицца Маргарита</p>
          <p  class="text-rest-gray mb-2">Завтрак ~ Пицца</p>
          <div class="flex">
            <star-icon class="mr-2"/>
            <span class="text-rest-yellow text-xs">4.9</span>
            <span class="mr-1 px-2 text-rest-gray text-xs">(124 ratings)</span>
          </div>
        </div>
      </div>
    </div>
    <div class="max-w-2xl pt-2 p-5 rounded-md tracking-wide">
      <div class="flex">
        <img alt="mountain" class="w-45 rounded-md border-2 border-gray-300" src="https://img.pizza/75/75" />
        <div  class="flex flex-col ml-5">
          <p  class="text-base text-rest-blacker font-semibold mb-2">Пицца Маргарита</p>
          <p  class="text-rest-gray  mb-2">Завтрак ~ Пицца</p>
          <div class="flex">
            <star-icon class="mr-2"/>
            <span class="text-rest-yellow text-xs">4.9</span>
            <span class="mr-1 px-2 text-rest-gray text-xs">(124 ratings)</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import bgImage from "../static/img/img.png"
import StarIcon from "../components/icons/starIcon";
export default {
  components: {StarIcon},
  data() {
    return {
      image: bgImage,
    };
  }
}
</script>

<style>
.header-wrapper {
  margin: 15px;
}

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
}

.second-column {
  text-align: right;
}
</style>
