<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width,initial-scale=1.0" />

    <title>Freebie 62 - Resume Alternate (Tailwind CSS) by pixelcave</title>

    <meta
      name="description"
      content="Freebie 62 - Resume Alternate (Tailwind CSS). Check out more at https://pixelcave.com"
    />
    <meta name="author" content="pixelcave" />

    <!-- Icons -->
    <link
      rel="icon"
      href="https://cdn.pixelcave.com/favicon.svg"
      sizes="any"
      type="image/svg+xml"
    />
    <link
      rel="icon"
      href="https://cdn.pixelcave.com/favicon.png"
      type="image/png"
    />

    <!-- Inter web font from bunny.net (GDPR compliant) -->
    <link rel="preconnect" href="https://fonts.bunny.net" />
    <link
      href="https://fonts.bunny.net/css2?family=Inter:wght@300;400;500;600;700;800;900&display=swap"
      rel="stylesheet"
    />

    <!-- Tailwind CSS Play CDN (mainly for development/testing purposes) -->
    <script src="https://cdn.tailwindcss.com?plugins=forms,typography,aspect-ratio"></script>

    <!-- Tailwind CSS v3 Configuration -->
    <script>
      const defaultTheme = tailwind.defaultTheme;
      const colors = tailwind.colors;
      const plugin = tailwind.plugin;

      tailwind.config = {
        darkMode: "class",
        theme: {
          extend: {
            fontFamily: {
              sans: ["Inter", ...defaultTheme.fontFamily.sans],
            },
          },
        },
      };
    </script>

    <!-- Alpine.js -->
    <script
      defer
      src="https://unpkg.com/alpinejs@3.x.x/dist/cdn.min.js"
    ></script>

    <!-- Alpine.js (x-cloak - https://alpinejs.dev/directives/cloak) -->
    <style>
      [x-cloak] {
        display: none !important;
      }
    </style>
  </head>
  <body>
    <!-- Page Container -->
    <div
      x-data="{
        darkMode: false,
        toggleDarkMode() {
          this.darkMode = ! this.darkMode;

          // Toggle dark class on html element
          if (this.darkMode) {
            document.body.parentNode.classList.add('dark');
          } else {
            document.body.parentNode.classList.remove('dark');
          }
        }
      }"
      class="min-h-dvh min-w-[320px] bg-white text-gray-800 dark:bg-gray-950 dark:text-gray-100"
    >
      <!-- Toggle Dark Mode -->
      <div
        class="fixed right-0 top-0 z-50 flex size-12 items-center justify-center"
      >
        <button
          x-on:click="toggleDarkMode()"
          type="button"
          class="inline-block size-9 text-gray-600 hover:opacity-75 dark:text-gray-400"
        >
          <svg
            x-show="!darkMode"
            x-cloak
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 24 24"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
            class="inline-block size-6"
          >
            <circle cx="12" cy="12" r="4" />
            <path d="M12 2v2" />
            <path d="M12 20v2" />
            <path d="m4.93 4.93 1.41 1.41" />
            <path d="m17.66 17.66 1.41 1.41" />
            <path d="M2 12h2" />
            <path d="M20 12h2" />
            <path d="m6.34 17.66-1.41 1.41" />
            <path d="m19.07 4.93-1.41 1.41" />
          </svg>
          <svg
            x-show="darkMode"
            x-cloak
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 24 24"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
            class="inline-block size-6"
          >
            <path d="M12 3a6 6 0 0 0 9 9 9 9 0 1 1-9-9Z" />
          </svg>
        </button>
      </div>
      <!-- END Toggle Dark Mode -->

      <div class="container mx-auto max-w-7xl">
        <div class="grid grid-cols-1 md:grid-cols-12">
          <!-- Info -->
          <div
            class="bg-gray-100 p-5 text-left dark:bg-gray-900 md:col-span-4 lg:p-14"
          >
            <h1
              class="leading-tighter mt-5 text-4xl font-extrabold lg:text-6xl"
            >
              Vansh<br />
              Mishra
            </h1>
            <h2 class="mt-3 text-xl text-purple-600 dark:text-purple-500">
              Web Developer,Freelancer
            </h2>
            <div class="-mx-5 mt-10 lg:-mx-10">
              <img
                src="c:\Users\varun\Downloads\WhatsApp Image 2024-12-07 at 8.31.13 PM.jpeg"
                class="inline-block lg:rounded-sm"
                alt="haun Castillo photo"
              />
            </div>
            <p
              class="mt-10 text-balance leading-relaxed text-gray-700 dark:text-gray-300"
            >
            I’m a dynamic professional with expertise in customer relations and research. I thrive on building strong relationships, delivering accurate results, and turning insights into impactful actions. With a passion for excellence and a proven ability to adapt and innovate, I’m ready to drive success in any team I join..
            </p>
            <div class="mt-10 space-y-5">
              <div class="flex items-center gap-5">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  class="inline-block size-6 flex-none text-purple-600 dark:text-purple-500"
                >
                  <path d="M18 8c0 4.5-6 9-6 9s-6-4.5-6-9a6 6 0 0 1 12 0" />
                  <circle cx="12" cy="8" r="2" />
                  <path
                    d="M8.835 14H5a1 1 0 0 0-.9.7l-2 6c-.1.1-.1.2-.1.3 0 .6.4 1 1 1h18c.6 0 1-.4 1-1 0-.1 0-.2-.1-.3l-2-6a1 1 0 0 0-.9-.7h-3.835"
                  />
                </svg>
                <span class="truncate font-medium">Gurugram,Haryana </span>
              </div>
              <div class="flex items-center gap-5">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  class="inline-block size-6 flex-none text-purple-600 dark:text-purple-500"
                >
                  <path
                    d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"
                  />
                </svg>
                <span class="truncate font-medium">+917880444676</span>
              </div>
              <div class="flex items-center gap-5">
                <svg
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  class="inline-block size-6 flex-none text-purple-600 dark:text-purple-500"
                >
                  <path
                    d="M22 13V6a2 2 0 0 0-2-2H4a2 2 0 0 0-2 2v12c0 1.1.9 2 2 2h8"
                  />
                  <path d="m22 7-8.97 5.7a1.94 1.94 0 0 1-2.06 0L2 7" />
                  <path d="M19 16v6" />
                  <path d="M16 19h6" />
                </svg>
                <a
                  href="javascript:void(0)"
                  class="truncate font-medium text-black underline hover:text-black/75 dark:text-white dark:hover:text-white/75"
                >
                  varunmishra1951@gmail.comm
                </a>
              </div>
              <div class="flex items-center gap-5">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  class="inline-block size-6 flex-none text-purple-600 dark:text-purple-500"
                >
                  <path
                  />
                  <path
                  />
                </svg>
                <a
                  
                >
                </a>
              </div>
            </div>
          </div>
          <!-- END Info -->

          <!-- Bio -->
          <div class="mx-auto max-w-2xl space-y-16 p-5 md:col-span-8 md:p-10">
            <!-- Education -->
            <div>
              <div
                class="mb-8 border-b-4 border-gray-100 py-2.5 dark:border-gray-900"
              >
                <h3 class="text-xl font-medium">Education</h3>
              </div>
              <ul
                class="relative space-y-6 pl-6 before:absolute before:bottom-0 before:left-0 before:top-0 before:block before:w-1 before:rounded-full before:bg-purple-50 before:content-[''] dark:before:bg-purple-950"
              >
                <li
                  class="before:border-1 relative before:absolute before:-left-[1.875rem] before:top-6 before:block before:size-4 before:rounded-full before:border-2 before:border-purple-200/75 before:bg-white before:content-[''] dark:before:border-purple-800/75 dark:before:bg-gray-950"
                >
                  <h4
                    class="text-sm font-semibold text-purple-600 dark:text-purple-500"
                  >
                    2020-2023
                  </h4>
                  <h5 class="mb-2 font-bold">
                    Bachelor of Computer Application (CSJM University) 
                  </h5>
                  <p class="text-sm/relaxed text-gray-700 dark:text-gray-300">
                    With a degree in Computer Science from the University of
                    Kanpur, INDIA, I cultivated the skills and knowledge that form
                    the bedrock of my expertise in web development and
                    programming.
                  </p>
                </li>
                <li
                  class="before:border-1 relative before:absolute before:-left-[1.875rem] before:top-6 before:block before:size-4 before:rounded-full before:border-2 before:border-purple-200/75 before:bg-white before:content-[''] dark:before:border-purple-800/75 dark:before:bg-gray-950"
                >
                  <h4
                    class="text-sm font-semibold text-purple-600 dark:text-purple-500"
                  >
                    2023-2025
                  </h4>
                  <h5 class="mb-2 font-bold">
                    Master of Computer Application , (Galgotias University)
                  </h5>
                  <p class="text-sm/relaxed text-gray-700 dark:text-gray-300">
                    I further honed my skills by pursuing a Master's degree in
                    Computer Science, delving deeper into advanced concepts and
                    emerging technologies to elevate my proficiency in web
                    development at Galgotias University , INDIA.
                  </p>
                </li>
                <li
                  class="before:border-1 relative before:absolute before:-left-[1.875rem] before:top-6 before:block before:size-4 before:rounded-full before:border-2 before:border-purple-200/75 before:bg-white before:content-[''] dark:before:border-purple-800/75 dark:before:bg-gray-950"
                >
                  <h4
                    class="text-sm font-semibold text-purple-600 dark:text-purple-500"
                  >
                    <!-- 2007-2009 -->
                  </h4>
                  <h5 class="mb-2 font-bold">
                    <!-- Professional Studies in Web Developement, NY, USA
                  </h5>
                  <p class="text-sm/relaxed text-gray-700 dark:text-gray-300">
                    My journey continued with Professional Studies in Web
                    Development, where I delved into specialized courses,
                    refining my expertise and staying abreast of the latest
                    industry trends to excel in the dynamic world of web
                    development. -->
                  </p>
                </li>
              </ul>
            </div>
            <!-- END Education -->

            <!-- Work Experience -->
            <div>
              <div
                class="mb-8 border-b-4 border-gray-100 py-2.5 dark:border-gray-900"
              >
                <h3 class="text-xl font-medium">Work Experience</h3>
              </div>
              <ul
                class="relative space-y-6 pl-6 before:absolute before:bottom-0 before:left-0 before:top-0 before:block before:w-1 before:rounded-full before:bg-purple-50 before:content-[''] dark:before:bg-purple-950"
              >
                <li
                  class="before:border-1 relative before:absolute before:-left-[1.875rem] before:top-6 before:block before:size-4 before:rounded-full before:border-2 before:border-purple-200/75 before:bg-white before:content-[''] dark:before:border-purple-800/75 dark:before:bg-gray-950"
                >
                  <h4
                    class="text-sm font-semibold text-purple-600 dark:text-purple-500"
                  >
                    01/2024 - Present
                  </h4>
                  <h5 class="mb-2 font-bold">
                    Freelance Web Developer
                  </h5>
                  <p class="text-sm/relaxed text-gray-700 dark:text-gray-300">
                    Embracing the freedom of a Freelance Web Developer, I thrive
                    on the diversity of projects, employing my technical prowess
                    to bring clients' visions to life through customized and
                    efficient web solutions.                  </p>
                </li>
                <li
                  class="before:border-1 relative before:absolute before:-left-[1.875rem] before:top-6 before:block before:size-4 before:rounded-full before:border-2 before:border-purple-200/75 before:bg-white before:content-[''] dark:before:border-purple-800/75 dark:before:bg-gray-950"
                >
                  <h4
                    class="text-sm font-semibold text-purple-600 dark:text-purple-500"
                  >
                    <!-- 02/2023 - 11/2024 -->
                  <!-- </h4>
                  <h5 class="mb-2 font-bold">Customer Care Executive (Paisa Bazaar Pvt.Ltd)</h5>
                  <p class="text-sm/relaxed text-gray-700 dark:text-gray-300">
                    Team Collaboration: Collaborated with cross-functional teams, including sales, marketing, and product development, to drive business growth.
                  </p>
                </li>
                <li -->
                  <!-- class="before:border-1 relative before:absolute before:-left-[1.875rem] before:top-6 before:block before:size-4 before:rounded-full before:border-2 before:border-purple-200/75 before:bg-white before:content-[''] dark:before:border-purple-800/75 dark:before:bg-gray-950" -->
                >
                  <h4
                    class="text-sm font-semibold text-purple-600 dark:text-purple-500"
                  >
                    <!-- 2010-2020
                  </h4>
                  <h5 class="mb-2 font-bold">
                    Part Time Web Developer at Web Stories LLC
                  </h5> -->
                  <!-- <p class="text-sm/relaxed text-gray-700 dark:text-gray-300">
                    Balancing my commitment as a Part-Time Web Developer at Web
                    Stories LLC, I contribute to the team's success by applying
                    my web development skills, ensuring seamless digital
                    experiences and collaborating on projects that enhance the
                    online presence of the company. -->
                  </p>
                </li>
              </ul>
            </div>
            <!-- END Work Experience -->

            <!-- Projects -->
            <div>
              <div
                class="mb-8 border-b-4 border-gray-100 py-2.5 dark:border-gray-900"
              >
                <h3 class="text-xl font-medium">Projects</h3>
              </div>
              <ul
                class="relative space-y-6 pl-6 before:absolute before:bottom-0 before:left-0 before:top-0 before:block before:w-1 before:rounded-full before:bg-purple-50 before:content-[''] dark:before:bg-purple-950"
              >
                <li
                  class="before:border-1 relative before:absolute before:-left-[1.875rem] before:top-6 before:block before:size-4 before:rounded-full before:border-2 before:border-purple-200/75 before:bg-white before:content-[''] dark:before:border-purple-800/75 dark:before:bg-gray-950"
                >
                  <h4
                    class="text-sm font-semibold text-purple-600 dark:text-purple-500"
                  >
                  </h4>
                  <h5 class="mb-2 font-bold">
                    Find Care - An Appointment Booking Website -
                    <a
                    >
                  </h5>
                  <p class="text-sm/relaxed text-gray-700 dark:text-gray-300">
                    A full-featured blog application enabling users to register, authenticate, and manage their blog posts seamlessly.
                    coordination and enhancing the user experience within the
                    dynamic realm of software as a service.
                  </p>
                </li>
                <li
                  class="before:border-1 relative before:absolute before:-left-[1.875rem] before:top-6 before:block before:size-4 before:rounded-full before:border-2 before:border-purple-200/75 before:bg-white before:content-[''] dark:before:border-purple-800/75 dark:before:bg-gray-950"
                >
                  <h4
                    class="text-sm font-semibold text-purple-600 dark:text-purple-500"
                  >
                    
                  </h4>
                  <h5 class="mb-2 font-bold">
                    Desgine the Definitive  Guide to T- Shirt -
                    <a
                     
                    >
                  </h5>
                  <p class="text-sm/relaxed text-gray-700 dark:text-gray-300">
                    T-shirts are a timeless wardrobe staple, blending comfort, style, and versatility. This guide covers everything you need to know about T-shirts, from their history and fabric choices to design trends and printing techniques. Learn how to choose the perfect fit, explore different styles, and discover tips for creating custom T-shirts..
                  </p>
                </li>
              </ul>
            </div>
            <!-- END Projects -->

            <!-- Social -->
            <div>
              <div
                class="mb-8 border-b-4 border-gray-100 py-2.5 dark:border-gray-900"
              >
                <h3 class="text-xl font-medium">Social</h3>
              </div>
              <ul
                class="relative space-y-6 pl-6 before:absolute before:bottom-0 before:left-0 before:top-0 before:block before:w-1 before:rounded-full before:bg-purple-50 before:content-[''] dark:before:bg-purple-950"
              >
                <li
                  class="before:border-1 relative before:absolute before:-left-[1.875rem] before:top-6 before:block before:size-4 before:rounded-full before:border-2 before:border-purple-200/75 before:bg-white before:content-[''] dark:before:border-purple-800/75 dark:before:bg-gray-950"
                >
                  <h4
                    class="text-sm font-semibold text-purple-600 dark:text-purple-500"
                  >
                    LinkedIn
                  </h4>
                  <h5 class="mb-2 font-bold">Work Profile</h5>
                  <p>
                    <a
                      href="javascript:void(0)"
                      class="text-sm font-medium text-gray-600 underline hover:text-gray-600/75 dark:text-gray-400 dark:hover:text-gray-400/75"
                    >
                    https://www.linkedin.com/in/vanshmishra16
                    </a>
                  </p>
                </li>
                <li
                  class="before:border-1 relative before:absolute before:-left-[1.875rem] before:top-6 before:block before:size-4 before:rounded-full before:border-2 before:border-purple-200/75 before:bg-white before:content-[''] dark:before:border-purple-800/75 dark:before:bg-gray-950"
                >
                  <h4
                    class="text-sm font-semibold text-purple-600 dark:text-purple-500"
                  >
                    
                    
                    </a>
                  </p>
                </li>
                <li
                >
                  <h4
                  >
                    <!-- Facebook
                  </h4>
                  <h5 class="mb-2 font-bold">Personal Profile</h5>
                  <p>
                    <a
                      class="text-sm font-medium text-gray-600 underline hover:text-gray-600/75 dark:text-gray-400 dark:hover:text-gray-400/75"
                      href="javascript:void(0)"
                    >
                      https://facebook.com/shaun.castillo
                    </a> -->
                  </p>
                </li>
              </ul>

              <!-- Footer -->
              <footer
                class="mt-20 space-y-2 py-8 text-sm text-gray-600 dark:text-gray-400"
              >
                <p class="font-semibold">
                  Resume &copy;
                  <script>
                    document.write(new Date().getFullYear());
                  </script>
                </p>
                <p class="inline-flex items-center gap-1">
                  <span>Crafted with</span>
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 20 20"
                    fill="currentColor"
                    data-slot="icon"
                    class="hi-mini hi-heart inline-block size-5 text-rose-500"
                  >
                    <path
                      d="m9.653 16.915-.005-.003-.019-.01a20.759 20.759 0 0 1-1.162-.682 22.045 22.045 0 0 1-2.582-1.9C4.045 12.733 2 10.352 2 7.5a4.5 4.5 0 0 1 8-2.828A4.5 4.5 0 0 1 18 7.5c0 2.852-2.044 5.233-3.885 6.82a22.049 22.049 0 0 1-3.744 2.582l-.019.01-.005.003h-.002a.739.739 0 0 1-.69.001l-.002-.001Z"
                    />
                  </svg>
                  <span
                    >by
                    <a
                      href="https://pixelcave.com"
                      class="font-medium text-black underline hover:text-black/75 dark:text-white dark:hover:text-white/75"
                    >
                      pixelcave
                    </a></span
                  >
                </p>
              </footer>
              <!-- END Footer -->
            </div>
            <!-- END Social -->
          </div>
          <!-- END Bio -->
        </div>
      </div>
    </div>
    <!-- END Page Container -->
  </body>
</html>
