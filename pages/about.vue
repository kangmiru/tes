<!-- <template>
    <div>
        <h2 class="text-blue-700">History Of Erigo</h2>
        <p class="text-justify">ERIGO is a local brand, the pride of Indonesia. ERIGO is a fashion brand founded by Muhammad Sadad in 2011. This local brand focuses on streetwear fashion that can be worn by men and women in Indonesia and globally. ERIGO has succeeded in becoming a local brand that is selling well in the market and has even begun to go global.</p>
        <p class="text-justify">ERIGO started doing business on November 28, 2010. The fashion business started by creating a brand called "Selected and Co". Over time, the brand changed its name to "ERIGO". In 2016, Erigo has a vision to support the traveling with Erigo campaign. With the aim of the campaign to show other countries a good view of the creativity of the nation's    children and also participate in lifting Indonesian tourism.</p>
        <p>api response:</p>
        <div>{{ data }}</div>
    </div>
</template> -->

<template>
    <section class="relative isolate overflow-hidden bg-white px-6 py-24 sm:py-32 lg:px-8">
      <div class="absolute inset-0 -z-10 bg-[radial-gradient(45rem_50rem_at_top,theme(colors.indigo.100),white)] opacity-20" />
      <div class="absolute inset-y-0 right-1/2 -z-10 mr-16 w-[200%] origin-bottom-left skew-x-[-30deg] bg-white shadow-xl shadow-indigo-600/10 ring-1 ring-indigo-50 sm:mr-28 lg:mr-0 xl:mr-16 xl:origin-center" />
      <div class="mx-auto max-w-2xl lg:max-w-4xl">
        <figure class="mt-10">
          <blockquote class="text-center text-xl font-semibold leading-8 text-gray-900 sm:text-2xl sm:leading-9">
            <p>ERIGO started doing business on November 28, 2010. The fashion business started by creating a brand called "Selected and Co". Over time, the brand changed its name to "ERIGO". In 2016, Erigo has a vision to support the traveling with Erigo campaign.</p>
          </blockquote>
          <figcaption class="mt-10">
            <img class="mx-auto h-20 w-20 rounded-full" src="https://assets.pikiran-rakyat.com/crop/16x84:1024x748/x/photo/2021/09/08/2245537483.jpeg" alt="" />
            <div class="mt-4 flex items-center justify-center space-x-3 text-base">
              <div class="font-semibold text-gray-900">Muhammad Saddad</div>
              <svg viewBox="0 0 2 2" width="3" height="3" aria-hidden="true" class="fill-gray-900">
                <circle cx="1" cy="1" r="1" />
              </svg>
              <div class="text-gray-600">CEO of Erigo</div>
            </div>
          </figcaption>
        </figure>
      </div>
    </section>
  </template>
  

<script setup>

  // const { data } = await useFetch('/api/ninja?name=mario')
  // const { data } = await useFetch('/api/ninja?name=mario', {
  //   method: 'post',
  //   body: {age: 30}
  // })

  const { data } = await useFetch('/api/currency/GBP')
</script>

<style scoped>
    h2 {
        margin-bottom: 20px;
        font-size: 36px;
    }
    p {
        margin: 20px 0;
    }
</style>