<template>
  <div class="min-h-screen bg-white text-black">
    <header class="fixed inset-x-0 top-0 z-50 h-20 md:h-16.5 bg-[#f8f9fa]">
      <div class="relative mx-auto h-full w-full px-3 lg:hidden">
        <div class="flex w-full h-full items-center justify-between">
          <a
              href="#"
              class="flex min-w-0 items-center no-underline"
          >
            <img src="/asset/live-support.png" alt="Live Support" class="h-12 w-12"/>

            <span
                class="ml-2 min-w-0 truncate text-[clamp(14px,4.5vw,20px)] font-normal text-[#a5a8a9]"
            >
        Live Support
      </span>
          </a>
          <div class="flex items-center justify-between gap-x-4">
          <button
              type="button"
              @click="homeWalletModal"
              class="shrink-0 cursor-pointer rounded-md py-2.5 px-3.75 bg-[#88cbf5] text-[clamp(12px,3.5vw,14px)] text-white no-underline"
          >
            Connect
          </button>
                  <button
                      type="button"
                      class="flex h-7 w-7 items-center justify-center border border-gray-300 rounded-md px-6 py-5"
                      @click="mobileMenuOpen = !mobileMenuOpen"
                      aria-label="Toggle navigation"
                  >
              <span class="flex flex-col gap-1">
                <span class="block h-0.5 w-6 bg-gray-600 rounded-sm"></span>
                <span class="block h-0.5 w-6 bg-gray-600 rounded-sm"></span>
                <span class="block h-0.5 w-6 bg-gray-600 rounded-sm"></span>
              </span>
                  </button>
            <div
                v-if="mobileMenuOpen"
                class="absolute left-0 right-0 top-20 border-t border-[#222] bg-white px-4 py-3"
            >
              <button
                  @click="openTawkChat()"
                  class="block text-sm border border-[#eee] rounded-md px-3.75 py-2.5 text-[#a5a8a9] no-underline"
              >
                Talk to an Agent
              </button>
            </div>
          </div>

        </div>

      </div>
      <div class="hidden h-full w-full items-center justify-between px-4 py-2 lg:flex">
        <a
            href="#"
            class="ml-16 flex h-full shrink-0 items-center no-underline"
        >
          <img src="/asset/live-support.png" alt="Live Support" class="h-10 w-10"/>

          <span class="ml-2 whitespace-nowrap text-xl font-normal text-[#a5a8a9]">
        Live Support
      </span>
        </a>
        <nav class="mr-24 flex items-center">

          <button

              @click="openTawkChat()"
              class="flex items-center bg-white text-[#a5a8a9] cursor-pointer rounded-md border border-[#eee] px-2.5 py-2.5 text-base no-underline"
          >
            Talk to an Agent
          </button>

          <button
              @click="homeWalletModal"
              class="ml-3.5 rounded-md py-2.5 px-3.75 bg-[#88cbf5] flex items-center cursor-pointer text-base text-white no-underline"
          >
            Connect
          </button>

        </nav>

      </div>

    </header>

    <main class="pt-10">
      <section
          class="relative overflow-hidden bg-[#7a7b7b]"
      >
        <div class="mx-auto w-full md:max-w-175 relative flex justify-center items-center flex-col h-125  pb-21.25 pt-32 md:pt-[42px]">

          <h1 class="text-center text-xl md:text-[32px] font-bold px-12 md:px-4 leading-9 pt-16 mb-4 text-white ">
            Hi, How can we help you?
          </h1>
          <div class="flex items-center rounded-md bg-white w-[90%] overflow-hidden">
            <input
                placeholder="Enter the search item here..."
                class="flex-1 min-w-0 px-4 py-3 outline-none bg-transparent text-gray-900"
            />
            <button class="shrink-0 bg-gray-200 rounded-r-[5px] py-3.75 px-4 border-none cursor-pointer">
              <img src="/asset/search.svg" width="30px" alt="search" />
            </button>
          </div>

        </div>

      </section>
      <section
          class="relative z-10 mx-auto -mt-12.5 px-4"
      >
        <div class="flex flex-col md:flex-row md:justify-center md:space-x-10 gap-2 sm:flex-row sm:justify-between relative">
          <button
              type="button"
              class="flex w-full md:justify-between md:gap-4 md:w-[327px] h-[132px] rounded-[15px] bg-[#fff] p-2.5 text-left text-black shadow-lg sm:w-[calc(50%-6px)]"
          >
            <div class="flex items-center justify-center">
              <svg
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 64 64"
                  class="h-[80px] w-[100px]"
              >
                <circle
                    cx="32.05"
                    cy="30.65"
                    r="14.75"
                    fill="none"
                    stroke="#475867"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                />

                <path
                    d="M38.27 44.4v8.8a1.56 1.56 0 0 1-1.55 1.56h-9.33a1.56 1.56 0 0 1-1.55-1.56v-8.8"
                    fill="none"
                    stroke="#475867"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                />

                <line
                    x1="30.54"
                    y1="58.94"
                    x2="33.65"
                    y2="58.94"
                    fill="none"
                    stroke="#475867"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                />

                <path
                    d="M42.35 34.16a10.65 10.65 0 0 1-.87 1.91"
                    fill="none"
                    stroke="#475867"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                />

                <path
                    d="M32.05 19.78a10.88 10.88 0 0 1 10.88 10.87"
                    fill="none"
                    stroke="#475867"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                />

                <line
                    x1="32"
                    y1="5.06"
                    x2="32"
                    y2="9.64"
                    fill="none"
                    stroke="#88cbf5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                />

                <line
                    x1="13.9"
                    y1="12.55"
                    x2="17.14"
                    y2="15.79"
                    fill="none"
                    stroke="#88cbf5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                />

                <line
                    x1="50.1"
                    y1="48.75"
                    x2="46.86"
                    y2="45.52"
                    fill="none"
                    stroke="#88cbf5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                />

                <line
                    x1="6.4"
                    y1="30.65"
                    x2="10.98"
                    y2="30.65"
                    fill="none"
                    stroke="#88cbf5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                />

                <line
                    x1="57.6"
                    y1="30.65"
                    x2="53.02"
                    y2="30.65"
                    fill="none"
                    stroke="#88cbf5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                />

                <line
                    x1="13.9"
                    y1="48.75"
                    x2="17.14"
                    y2="45.52"
                    fill="none"
                    stroke="#88cbf5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                />

                <line
                    x1="50.1"
                    y1="12.55"
                    x2="46.86"
                    y2="15.79"
                    fill="none"
                    stroke="#88cbf5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                />
              </svg>
            </div>

            <div>
              <strong class="text-base font-bold text-black">
                Browse articles
              </strong>

              <p class="mt-1 text-base text-black leading-6">
                Explore How-To's and learn best practices from our knowledge...
              </p>
            </div>
          </button>
          <button
              type="button"
              class="flex md:justify-between md:gap-4 md:w-81.75 h-33 rounded-[15px] w-full bg-white p-2.5 text-left text-black shadow-lg sm:w-[calc(50%-6px)]"
          >
            <div class="flex items-center justify-center">
              <svg
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 64 64"
                  class="h-[80px] w-[100px]"
              >
                <circle
                    cx="20.96"
                    cy="22.89"
                    r="7.95"
                    fill="none"
                    stroke="#475867"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                />

                <path
                    d="M5.05 51A15.91 15.91 0 0 1 22 35.12c8.45.55 14.84 8 14.84 16.42v4.26A3.18 3.18 0 0 1 33.68 59H8.23a3.18 3.18 0 0 1-3.18-3.2Z"
                    fill="none"
                    stroke="#475867"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                />

                <path
                    d="M37.86 23.4A11.63 11.63 0 1 1 40.38 26l-4 1.49Z"
                    fill="none"
                    stroke="#88cbf5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                />

                <line
                    x1="47.43"
                    y1="11.11"
                    x2="47.43"
                    y2="17.11"
                    fill="none"
                    stroke="#88cbf5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                />

                <line
                    x1="47.43"
                    y1="20.75"
                    x2="47.43"
                    y2="21.75"
                    fill="none"
                    stroke="#88cbf5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                />
              </svg>
            </div>

            <div class="mt-2">
              <strong class="text-base text-black font-bold">
                Talk to an Agent
              </strong>

              <p class="mt-1 text-base text-black leading-6">
                Connect with Live Help Desk Support Agent Now...
              </p>
            </div>
          </button>

        </div>
      </section>
      <section
          class="w-full px-4 pb-12 pt-[50px]"
      >
        <div class="flex flex-col items-center justify-between gap-2">
          <h2 class="text-[28px] font-bold leading-8 text-black mb-3">
            Knowledge base
          </h2>

          <a
              href="#"
              class="text-base leading-6 text-[#88cbf5] mb-6"
          >
            View all article
          </a>
        </div>

        <div
            class="mx-auto mt-2 grid w-full max-w-240 grid-cols-1 gap-x-6 gap-y-8 px-4 sm:grid-cols-2 lg:grid-cols-3"
        >
          <button
              v-for="item in articles"
              :key="item.title"
              @click="openTawkChat()"
              class="h-full cursor-pointer"
          >
            <div
                class="h-full flex py-16 min-h-51.5 w-full flex-col items-center justify-end rounded-[10px] border border-[#ccc] px-10 pb-4 text-center"
            >

              <img src="/asset/live-support.png" alt="" class="w-17.5 h-17.5"/>

              <h3 class="mt-3 mb-3 text-base font-bold leading-6">
                {{ item.title }}
              </h3>

              <p class="mb-3 max-w-70 text-center text-base leading-6">
                {{ item.text }}
              </p>

            </div>
          </button>
        </div>
      </section>
      <section
          class="border-t border-[#dee2e6] px-4 pb-10 pt-8"
      >

        <div
            class="mx-auto max-w-[960px]"
        >

          <div class="mb-8 flex items-center justify-between">
            <h2 class="text-2xl font-bold leading-7">
              Most popular articles
            </h2>

            <button
                @click="openTawkChat()"
                class="text-base text-[#88cbf5] leading-6 cursor-pointer"
            >
              View all article
            </button>
          </div>


          <div class="grid grid-cols-1 sm:grid-cols-2">

            <div
                v-for="(faq, index) in faqs"
                :key="faq.title"
                class="min-h-[83px] border-b border-[#dee2e6] px-5 py-[18px] sm:border-r"
                :class="{
      'sm:border-r-0': index % 2 === 1,
      'sm:border-b-0': index >= faqs.length - 2
    }"
            >
              <button
                  @click="openTawkChat()"
                  class="cursor-pointer flex items-start text-base font-bold leading-6 text-[#a5a8a9] no-underline"
              >
                <!-- Plus icon -->
                <span class="relative mt-[2px] mr-2 h-5 w-5 shrink-0">
      <img src="/asset/file.svg" alt=""/>
    </span>

                <div class="mr-5 flex flex-col items-start">
                  <strong>
                    {{ faq.title }}
                  </strong>

                  <small class="mt-[5px] block text-sm font-normal leading-5">
                    {{faq.date}}
                  </small>
                </div>
              </button>
            </div>

          </div>

        </div>

      </section>

    </main>
    <footer class="h-14 bg-[#a5a8a9] text-white flex items-center justify-center text-center text-base leading-6">
      Helpdesk Software by Freshdesk | Cookie policy
    </footer>
    <HomeWalletModal :open="showHomeWalletModal" @close="showHomeWalletModal = false" />
  </div>
</template>
<script setup lang="ts">

const mobileMenuOpen = ref(false)
const showConnectWallet = ref(false)
const showHomeWalletModal = ref(false)
const homeWalletModal = () => { showHomeWalletModal.value = true }
const connectAutomatically = () => {
  showConnectWallet.value = false
}
const popularLinks = [
  'Wallet Issues',
  'Synchronization',
  'Security',
  'Notification',
  'Claim Issues',
  'Transactions',
  'Development'
]

const articles = [
  ['Blockchain', 'Live Support is capable of handling higher transaction volume than its counterpart - Ethereum...'],
  ['Wallet Encryption', 'Wallet encryption allows you to secure your wallet, so that you can view transactions and your account balance...'],
  ['Open-Source Software', 'Live Support is an open source software project released under the MIT/X11 license which gives you the power to...'],
].map(([title, text]) => ({
  title,
  text
}))

const faqs = [
    { "title":  'Change wallet after transaction',
      "date": "Modified on 24 October by MGK71"

},
  { "title": 'Why is litecoin so strong?',
    "date": "Modified on 17 August by Nolan Matthew"
  },
  { "title": 'Want to boost your business online visibilty in 2023?',
    "date": "Modified on 25 October by Design Centrals"
  },
  { "title": 'Buy and sell crypto currency in Dubai',
    "date": "Modified on 09 October by Xchangeruae"
  },
]
const openTawkChat = () => {
  if (typeof window !== 'undefined' && window.Tawk_API) {
    window.Tawk_API.maximize()
  }
}
</script>