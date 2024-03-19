

<main class="flex justify-center align-center">
  <div class="card w-1/3 p-2 mt-4">
    <h2 class="my-2">Video Editing</h2>

    <div class="scrolling-gradient-gray w-auto m-2 h-[500px]">
      <div class="rotated-text">
        <h1>To be determined</h1>
        <hr class="translate-line"/>
      </div>

    </div>


  </div>
</main>

<style>
  .rotated-text {
    @apply w-full h-full;
    -ms-transform: rotate(-45deg) translate(20%, 40%);
    -webkit-transform: rotate(-45deg) translate(20%, 40%);
    transform: rotate(-40deg) translate(20%, 40%);
  }
  .translate-line {
    @apply w-5/6;
    -ms-transform: translate(20%, 40%);
    -webkit-transform: translate(20%, 40%);
    transform: translate(-10%);
  }

  .scrolling-gradient-gray {
    background: linear-gradient(45deg, rgba(0,0,0,0) 0%, rgba(0, 0, 0, 0.40) 50%, rgba(0,0,0,0) 100%);
    background-size: 200% 200%;
    animation: gradient 15s linear infinite;
  }

  @keyframes gradient {
    0% {
      background-position: 0% 82%
    }
    50% {
      background-position: 100% 19%
    }
    100% {
      background-position: 0% 82%
    }
  }
</style>
