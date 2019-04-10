<template>
  <section class="container">
    <div class="main-frame">
      <div class="top-content">
        <span v-text="mainContent">
          {{ mainContent.name }}
        </span>
      </div>
      <div class="contents">
        <div v-for="content in contents" :key="content.id" class="sub-contents">
          {{ content.name }}
        </div>
      </div>
    </div>
  </section>
</template>

<script>
  export default {
    layout: 'navbarFooterLess',
    data() {
      return {
        mainContent: 'main content',
        contents: [
          {id: 1, name: 'PHP'     },
          {id: 2, name: 'Perl'    },
          {id: 3, name: 'HTML5'   },
          {id: 4, name: 'CSS3'    },                    
          {id: 5, name: 'Github'  },
          {id: 6, name: 'Laravel' },
          {id: 7, name: 'Docker'  },
          {id: 8, name: 'Vue.js'  },
          {id: 9, name: 'Nuxt.js' },
        ]
      }
    }
  }
</script>

<style>
  html {
    background-color: #fafafa;
  }

  .container {
    margin: 0 auto;
    margin-top: 10px;
    justify-content: center;
    align-items: center;
    text-align: center;
  }

  .main-frame {
    margin: 0 auto;
    width: 900px;
    height: auto;
  }

  .top-content {
    font-size: 100px;
    background-color: white;
    width: 100%;
    height: 300px;
    margin-bottom: 15px;
  }

  .contents {
    display: grid;
    gap: 15px;
    grid-template-columns: repeat(auto-fit, minmax(49%, 1fr));
  }

  .sub-contents {
    font-size: 100px;
    background-color: white;
    height: 300px;
  }
  
  @media(max-width: 320px) {
    .contents {
      display: grid;
      gap: 15px;
      grid-template-columns: repeat(auto-fit, minmax(100%, 1fr));
    }
  }

</style>
