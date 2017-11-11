<template>
  <div id="app">
    <router-view></router-view>
  </div>
</template>

<style>
@import url(https://fonts.googleapis.com/css?family=Lato);

body {
  background-color: #f1f2f0;
  color: #35342f;
  font-family: 'Lato', sans-serif;
}

.page {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  margin: 80px auto;
}

.fadeIn-animation {
  animation: fadeIn 1.5s;
}

.fadeIn-page-animation {
  animation: fadeIn 1s;
}

@keyframes fadeIn {
    from {
        opacity:0;
    }
    to {
        opacity:1;
    }
}
@-moz-keyframes fadeIn {
    from {
        opacity:0;
    }
    to {
        opacity:1;
    }
}
@-webkit-keyframes fadeIn {
    from {
        opacity:0;
    }
    to {
        opacity:1;
    }
}
@-o-keyframes fadeIn {
    from {
        opacity:0;
    }
    to {
        opacity: 1;
    }
}
</style>
