<template>
  <div
    class="flex flex-col h-screen w-screen bg-cover"
    style="background-image: url(/bg-work-harder.jpg)"
  >
    <!-- Top Bar -->
    <div
      class="
        h-8
        flex
        items-center
        justify-between
        py-2
        px-4
        bg-gray-900 bg-opacity-90
        text-gray-400 text-sm
        shadow-lg
      "
    >
      <div>Marius Andresen</div>
      <div>
        <span>Tue May 25 10:45 AM</span>
      </div>
    </div>

    <!-- Main Content -->
    <div class="flex flex-grow items-center justify-center">
      <!-- Console Window -->
      <div
        class="
          h-5/6
          w-1/2
          flex flex-col
          bg-gray-900 bg-opacity-90
          rounded-lg
          shadow-lg
        "
      >
        <div
          class="
            flex
            justify-between
            bg-gray-900
            rounded-t-lg
            px-4
            py-1
            text-gray-400 text-sm
          "
        >
          <div class="flex items-center space-x-1.5">
            <div flex items-center>
              <svg
                class="h-2"
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 64 64"
                aria-labelledby="title"
                aria-describedby="desc"
              >
                <circle cx="32" cy="32" r="32" stroke-width="0" fill="red" />
              </svg>
            </div>
            <div flex items-center>
              <svg
                class="h-2"
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 64 64"
                aria-labelledby="title"
                aria-describedby="desc"
              >
                <circle cx="32" cy="32" r="32" stroke-width="0" fill="yellow" />
              </svg>
            </div>
            <div flex items-center>
              <svg
                class="h-2"
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 64 64"
                aria-labelledby="title"
                aria-describedby="desc"
              >
                <circle cx="32" cy="32" r="32" stroke-width="0" fill="green" />
              </svg>
            </div>
          </div>
          <div class="select-none">Portfolio</div>
          <div class="select-none"></div>
        </div>
        <div
          class="
            flex flex-col flex-grow
            justify-end
            pl-2
            text-gray-400
            font-mono
          "
        >
          <div>history goes here</div>
          <div>
            <span>kalosar@macbook></span>
            <span class="animate-ping font-bold">_</span>
          </div>
        </div>
      </div>
    </div>

    <!-- Action Bar -->
    <div class="flex justify-center">
      <div
        class="
          flex
          items-center
          py-2
          px-6
          mb-2
          bg-gray-900 bg-opacity-90
          rounded-xl
          space-x-4
        "
      >
        <a
          href="#"
          class="
            h-14
            w-14
            bg-black
            rounded-lg
            p-2
            transform
            transition
            duration-500
            hover:scale-110
          "
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 64 64"
            aria-labelledby="title"
            aria-describedby="desc"
          >
            <path
              data-name="layer2"
              d="M32 0a32.021 32.021 0 00-10.1 62.4c1.6.3 2.2-.7 2.2-1.5v-6c-8.9 1.9-10.8-3.8-10.8-3.8-1.5-3.7-3.6-4.7-3.6-4.7-2.9-2 .2-1.9.2-1.9 3.2.2 4.9 3.3 4.9 3.3 2.9 4.9 7.5 3.5 9.3 2.7a6.93 6.93 0 012-4.3c-7.1-.8-14.6-3.6-14.6-15.8a12.27 12.27 0 013.3-8.6 11.965 11.965 0 01.3-8.5s2.7-.9 8.8 3.3a30.873 30.873 0 018-1.1 30.292 30.292 0 018 1.1c6.1-4.1 8.8-3.3 8.8-3.3a11.965 11.965 0 01.3 8.5 12.1 12.1 0 013.3 8.6c0 12.3-7.5 15-14.6 15.8a7.746 7.746 0 012.2 5.9v8.8c0 .9.6 1.8 2.2 1.5A32.021 32.021 0 0032 0z"
              fill="#FFFFFF"
            />
            <path
              data-name="layer1"
              d="M12.1 45.9c-.1.2-.3.2-.5.1s-.4-.3-.3-.5.3-.2.6-.1c.2.2.3.4.2.5zm1.3 1.5a.589.589 0 01-.8-.8.631.631 0 01.7.1.494.494 0 01.1.7zm1.3 1.8a.585.585 0 01-.7-.3.6.6 0 010-.8.585.585 0 01.7.3c.2.3.2.7 0 .8zm1.7 1.8c-.2.2-.5.1-.8-.1-.3-.3-.4-.6-.2-.8a.619.619 0 01.8.1.554.554 0 01.2.8zm2.4 1c-.1.3-.4.4-.8.3s-.6-.4-.5-.7.4-.4.8-.3c.3.2.6.5.5.7zm2.6.2c0 .3-.3.5-.7.5s-.7-.2-.7-.5.3-.5.7-.5c.4.1.7.3.7.5zm2.4-.4q0 .45-.6.6a.691.691 0 01-.8-.3q0-.45.6-.6c.5-.1.8.1.8.3z"
              fill="#202020"
            />
          </svg>
        </a>

        <a
          href="#"
          class="
            h-14
            w-14
            bg-blue-500
            p-2
            rounded-lg
            transform
            transition
            duration-500
            hover:scale-110
          "
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 64 64"
            aria-labelledby="title"
            aria-describedby="desc"
          >
            <path
              data-name="layer1"
              fill="#FFFFFF"
              d="M1.15 21.7h13V61h-13zm46.55-1.3c-5.7 0-9.1 2.1-12.7 6.7v-5.4H22V61h13.1V39.7c0-4.5 2.3-8.9 7.5-8.9s8.3 4.4 8.3 8.8V61H64V38.7c0-15.5-10.5-18.3-16.3-18.3zM7.7 2.6C3.4 2.6 0 5.7 0 9.5s3.4 6.9 7.7 6.9 7.7-3.1 7.7-6.9S12 2.6 7.7 2.6z"
            />
          </svg>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style></style>
