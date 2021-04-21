<template>
  <div class='header-wrapper'>
    <div class='row'>
      <div class='column'>
        <div class='first-column'>
          <h3>LOGO</h3>
        </div>
      </div>
      <div class='column'>
        <div class='second-column'>
          <h3>Чайла</h3>
        </div>
      </div>
    </div>
    <form class="mb-4 w-full md:mb-0 md:w-1/4 pt-4">
      <label class="hidden" for="">Search</label>
      <input class="bg-grey-lightest border-2 focus:border-orange p-2 rounded-full shadow-inner w-full" placeholder="Search" type="text">
      <button class="hidden">Submit</button>
    </form>
    <h3 class="font-bold">Завтраки</h3>
    <div class="holder mx-auto w-10/12 grid sm:grid-cols-1 md:grid-cols-3 lg:grid-cols-4 rounded-md">
      <div class="each mb-10 m-2 shadow-lg border-gray-800 bg-gray-100 relative">
        <h1 class="font-bold">Омлет с овощами</h1>
<!--        <img class="w-full" src="https://i.ytimg.com/vi/qew27BNl7io/maxresdefault.jpg" alt="" />-->
        <iframe class="w-full"
                src="https://www.youtube.com/embed/tgbNymZ7vqY?playlist=tgbNymZ7vqY&loop=1">
        </iframe>
        <nuxt-link to="/detail" class="badge absolute top-0 right-0 m-1 text-rest-yellow  px-2 text-xs rounded">Состав</nuxt-link>
        <div class="info-box text-xs flex p-1 font-semibold text-rest-yellow">
          <span class="p-1"><star-icon/></span>
          <span class="mr-1 p-1 font-bold text-gray-500">(124 ratings) Завтрак</span>
        </div>
        <div class='row'>
          <div class='column'>
            <div class='first-column text-xs'>
              <rest-button
                title="20 min"
                type="primary"
                :svgIcon="'timerIcon'"
              />
            </div>
          </div>
          <div class='column'>
            <div class='second-column text-xs' >
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
          <h3 class="font-bold">Популярная еда</h3>
        </div>
      </div>
      <div class='column'>
        <div class='second-column'>
          <h6 class="text-rest-yellow">Посмотреть все</h6>
        </div>
      </div>
    </div>
    <div class="max-w-2xl bg-white pt-2 p-5 rounded-md tracking-wide">
      <div  class="flex">
        <img alt="mountain" class="w-45 rounded-md border-2 border-gray-300" src="https://img.pizza/100/100" />
        <div  class="flex flex-col ml-5">
          <h4  class="text-xl font-semibold mb-2">Пицца Маргарита</h4>
          <p  class="text-gray-800 mb-2">Завтрак ~ Пицца</p>
          <div class="flex">
            <star-icon class="mr-2"/>
            <span class="text-rest-yellow text-xs">4.9</span>
            <span class="mr-1 px-2 font-bold text-gray-500 text-xs">(124 ratings)</span>
          </div>
        </div>
      </div>
    </div>
    <div class="max-w-2xl bg-white pt-2 p-5 rounded-md tracking-wide">
      <div id="header" class="flex">
        <img alt="mountain" class="w-45 rounded-md border-2 border-gray-300" src="https://img.pizza/100/100" />
        <div id="body" class="flex flex-col ml-5">
          <h4 class="text-xl font-semibold mb-2">Пицца Маргарита</h4>
          <p  class="text-gray-800 mb-2">Завтрак ~ Пицца</p>
          <div class="flex">
            <star-icon class="mr-2"/>
            <span class="text-rest-yellow text-xs">4.9</span>
            <span class="mr-1 px-2 font-bold text-gray-500 text-xs">(124 ratings)</span>
          </div>
        </div>
      </div>
    </div>
    <div class="max-w-2xl bg-white pt-2 p-5 rounded-md tracking-wide">
      <div class="flex">
        <img alt="mountain" class="w-45 rounded-md border-2 border-gray-300" src="https://img.pizza/100/100" />
        <div  class="flex flex-col ml-5">
          <h4  class="text-xl font-semibold mb-2">Пицца Маргарита</h4>
          <p  class="text-gray-800 mb-2">Завтрак ~ Пицца</p>
          <div class="flex">
            <star-icon class="mr-2"/>
            <span class="text-rest-yellow text-xs">4.9</span>
            <span class="mr-1 px-2 font-bold text-gray-500 text-xs">(124 ratings)</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import StarIcon from "../components/icons/starIcon";
export default {
  components: {StarIcon}
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
  height: 100%;
}
</style>
