<template>
<div>
  <div>
        <div class="float-right z-30 fixed top-0 right-0 m-1 pt-4">
            <div class="z-30 lg:hidden">
    <button 
    v-if="!sidebar"
    @click="sidebar=true"
    type="button" id="sidebar-open" class="flex px-6 items-center  text-gray-700 focus:outline-none focus:text-gray-800">
           menu
    </button>
    <button
    v-else
      type="button"
      id="sidebar-close"
       @click="sidebar=false"
      class="flex px-6 items-center text-gray-700 focus:outline-none focus:text-gray-800"
    >
      close
    </button>
  </div>
        </div>
        <div class="clearfix"></div>
      
    </div>
  <div class="min-h-screen lg:flex">
    <no-ssr>
    <div class="static h-full inset-0 h-full bg-gray-100 z-20 flex-none w-full lg:w-1/5 bg-gray-200 text-gray-700"
    :class="{'hidden lg:block': !sidebar}">
    <div class="fixed bg-gray-200 h-screen w-full lg:w-1/5">
    
        <div class='px-2'>
          <p>
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Enim, tempore?
          </p>
        </div>
        </div>
    </div>
      </no-ssr>
    <div class="flex-1 bg-white lg:w-4/5 lg:static text-gray-700">
        <div class="container mx-auto mt-5 lg:mt-20 px-2 text-left">
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Sit minus quia nostrum id. Odit consectetur aliquid, doloremque eaque ducimus nostrum eligendi minima ratione blanditiis tempore ipsam exercitationem ex et repellendus quasi minus reprehenderit officia ea sed beatae! Harum, sit neque.
            </p>
        </div>
        <!-- footer -->
    </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      sidebar : false
    }
  }
}
</script>
<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
</style>
