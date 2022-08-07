<script>
import Navbar from './components/Navbar.vue'

export default {
  components: {
    Navbar
  },
  data() {
    return {
      navItems: [
        { name: 'Blog', href: 'https://blog.francie.cc', fa_icons: 'fa-solid fa-cubes' },
        { name: 'Blogroll', href: 'https://blogroll.francie.cc', fa_icons: 'fa-solid fa-people-robbery' },
        { name: 'Projects', href: 'https://github.com/franci-e', fa_icons: 'fa-solid fa-trowel-bricks' },
        { name: 'Twitter', href: 'https://twitter.com/franciejiang', fa_icons: 'fa-brands fa-twitter'}
      ]
    }
  }
}
</script>

<template>

  <div class="flex w-full flex-col">
    <div class="flex lg:justify-end p-2 justify-center [letter-spacing:1em] lg:[letter-spacing:0.05em] text-2xl lg:text-lg lg:[font-family:var(--display)] lg:[text-transform:uppercase]">
    <Navbar
    v-for="itm in navItems"
    :href="itm.href"
    :name="itm.name"
    :fa_icons="itm.fa_icons"
  ></Navbar>
  </div>
  <div class="justify-center items-center flex">
    <div class="flex text-black flex-col m-4 lg:m-2 text-xl items-center justify-center">
    <div class="text-4xl md:text-6xl p-1 flex-col flex lg:text-8xl [font-weight:800] [opacity:0.6]">
      Francie Jiang
      <div class="flex"><small class="[font-family:CharisSILW] text-xl align-top [margin-left:0.1em] [opacity:0.6]">(/'frænsi: tɕi:aŋ/)</small></div>
    </div>
    <div class="w-5/6">
      <div class="[font-family:var(--serif)] [opacity:0.7] text-2xl">
        Introduction
      </div>
      <div>
        Francie Jiang lives in a country where no bad things are allowed to happen and no <em><a href="https://en.wiktionary.org/wiki/negative_Nancy">Negative Nancies</a></em> are allowed to survive. Unfortunately, she, coincidentally, is a textbook example of a <em>Negative Francie</em>. She often loses hopes to survive for the involution in her country<sup class="text-sky-500" id="startRef"><a href="#ref1">[1]</a><a href="#ref2">[2]</a><a href="#ref3">[3]</a></sup>. She endeavors to find ways to slack off with great joy, including studying subjects which do not pertain to her exams, such as <em><a href="https://en.wikipedia.org/wiki/Gaokao">Gaokao</a></em>. <br> <br>
        She is currently a senior high student with some above-average rank in her school, which only gives its students a 6-hour break per week and a 2-day off per month. Despite the inhumane vacation schedule, she is also suffering from the pressure given by her parents. It is of no surprise that she would lose hope in her life. At her leisure, she is fascinated by writing codes, whether <em>sh*tty</em> or not, for her ideal job is electrical engineer. <br> <br>
        She likes retro things. It is for this she bought several old tech gadgets, including a 15-inch early-2008 MacBook Pro, an iPhone 4S, an iPod touch 4, and a Nokia N95.<br> <br>
        She is now studying <a href="https://vuejs.org">Vue.js</a> and other frontend frameworks. <br> <br>
        She is not satisfied with her hitherto life, therefore, she has a strong desire to study in a university, which provides a libre environment for her.
      </div>
      <div class="text-2xl [opacity:0.7] [font-family:var(--serif)] mt-2">
        References & Citations
      </div>
      <div class="text-lg overflow-hidden">
        <div id="ref1">
          <span class="text-sky-500">
            <a href="#startRef">[1]</a>
          </span>
          . Liu, Y., 2021. China's "Involuted" Generation. [online] The New Yorker. Available at: &lt;<a class="text-sky-500" href="https://www.newyorker.com/culture/cultural-comment/chinas-involuted-generation">https://www.newyorker.com/culture/cultural-comment/chinas-involuted-generation</a>&gt; [Accessed 1 August 2022].
        </div>
        <div id="ref2">
          <span class="text-sky-500">
            <a href="#startRef">[2]</a>
          </span>
          . Wang, F. and Wang, Y., 2021. The buzzwords reflecting the frustration of China's young generation. [online] BBC News. Available at: &lt;<a class="text-sky-500" href="https://www.bbc.com/news/world-asia-china-57328508">https://www.bbc.com/news/world-asia-china-57328508</a>&gt; [Accessed 1 August 2022].
        </div>
        <div id="ref3">
          <span class="text-sky-500">
            <a href="#startRef">[3]</a>
          </span>
          . Wang, Q. and Ge, S., 2020. How One Obscure Word Captures Urban China’s Unhappiness. [online] #SixthTone. Available at: &lt;<a class="text-sky-500" href="https://www.sixthtone.com/news/1006391/how-one-obscure-word-captures-urban-chinas-unhappiness">https://www.sixthtone.com/news/1006391/how-one-obscure-word-captures-urban-chinas-unhappiness</a>&gt; [Accessed 1 August 2022].
        </div>
      </div>
      <div class="flex justify-center text-center flex-col [opacity:0.6] text-base mt-2">
        &copy; 2022 Francie Jiang Properties Foundation (FJPF). All rights reserved. 
        <div>Built with <a href="https://tailwindcss.com">Tailwind CSS</a> and <a href="https://vuejs.org">Vue.js</a>. Deployed at <a href="https://vercel.app">Vercel</a>. Used <a href="https://sil.org">Charis SIL font by SIL International for IPA display</a></div>
      </div>
    </div>

  </div>

  </div>
  
  </div>
  

</template>
