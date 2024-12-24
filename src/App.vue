<template>
  <div id="wrapper" class="h-full md:w-2/3 lg:w-4/5 mx-auto justify-center flex flex-col space-y-10 pt-10 pb-10">
    <SectionComponent>
      <SectionTitle>
        <template #icon>
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="h-8 w-8 lg:h-10 lg:w-10">
            <path fill-rule="evenodd" d="M18.685 19.097A9.723 9.723 0 0021.75 12c0-5.385-4.365-9.75-9.75-9.75S2.25 6.615 2.25 12a9.723 9.723 0 003.065 7.097A9.716 9.716 0 0012 21.75a9.716 9.716 0 006.685-2.653zm-12.54-1.285A7.486 7.486 0 0112 15a7.486 7.486 0 015.855 2.812A8.224 8.224 0 0112 20.25a8.224 8.224 0 01-5.855-2.438zM15.75 9a3.75 3.75 0 11-7.5 0 3.75 3.75 0 017.5 0z" clip-rule="evenodd" />
          </svg>
        </template>
        <template #title>About Me</template>
      </SectionTitle>
      <div id="content" class="flex lg:space-x-10 justify-center bg-gray-300 py-2">
        <img src="./assets/Profile.jpg" class="w-36 h-36 lg:w-64 lg:h-64 rounded-full object-cover object-middle">
        <div class="flex flex-col space-y-2 lg:space-y-7 my-auto">
          <span class="text-xl lg:text-3xl">
            Hello! My name is <div class="text-3xl lg:text-5xl mt-2 text-slate-800">Ng Jia Liang</div>
          </span>
          <span class="text-lg lg:text-xl">
            I am a software engineer and programmer
          </span>
        </div>
      </div>
    </SectionComponent>

    <SectionComponent>
      <SectionTitle>
        <template #icon>
          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="h-8 w-8 lg:h-10 lg:w-10">
            <path stroke-linecap="round" stroke-linejoin="round" d="M11.42 15.17L17.25 21A2.652 2.652 0 0021 17.25l-5.877-5.877M11.42 15.17l2.496-3.03c.317-.384.74-.626 1.208-.766M11.42 15.17l-4.655 5.653a2.548 2.548 0 11-3.586-3.586l6.837-5.63m5.108-.233c.55-.164 1.163-.188 1.743-.14a4.5 4.5 0 004.486-6.336l-3.276 3.277a3.004 3.004 0 01-2.25-2.25l3.276-3.276a4.5 4.5 0 00-6.336 4.486c.091 1.076-.071 2.264-.904 2.95l-.102.085m-1.745 1.437L5.909 7.5H4.5L2.25 3.75l1.5-1.5L7.5 4.5v1.409l4.26 4.26m-1.745 1.437l1.745-1.437m6.615 8.206L15.75 15.75M4.867 19.125h.008v.008h-.008v-.008z" />
          </svg>
        </template>
        <template #title>Skills</template>
      </SectionTitle>
      <div id="content" class="flex flex-col mx-5 space-y-5 lg:mx-0 lg:flex-row lg:space-x-5 lg:space-y-0 justify-center">
        <SkillCard>
          <template #icon>
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="skill-icon">
              <path stroke-linecap="round" stroke-linejoin="round" d="M4.26 10.147a60.436 60.436 0 00-.491 6.347A48.627 48.627 0 0112 20.904a48.627 48.627 0 018.232-4.41 60.46 60.46 0 00-.491-6.347m-15.482 0a50.57 50.57 0 00-2.658-.813A59.905 59.905 0 0112 3.493a59.902 59.902 0 0110.399 5.84c-.896.248-1.783.52-2.658.814m-15.482 0A50.697 50.697 0 0112 13.489a50.702 50.702 0 017.74-3.342M6.75 15a.75.75 0 100-1.5.75.75 0 000 1.5zm0 0v-3.675A55.378 55.378 0 0112 8.443m-7.007 11.55A5.981 5.981 0 006.75 15.75v-1.5" />
            </svg>
          </template>
          <template #title>
            Programming Language
          </template>
          <template #content>
            <div>- PHP, JavaScript, Java</div>
            <div>- HTML, CSS</div>
            <div>- MySQL/SQL Database</div>
          </template>
        </SkillCard>

        <SkillCard>
          <template #icon>
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="skill-icon">
              <path stroke-linecap="round" stroke-linejoin="round" d="M6 6.878V6a2.25 2.25 0 012.25-2.25h7.5A2.25 2.25 0 0118 6v.878m-12 0c.235-.083.487-.128.75-.128h10.5c.263 0 .515.045.75.128m-12 0A2.25 2.25 0 004.5 9v.878m13.5-3A2.25 2.25 0 0119.5 9v.878m0 0a2.246 2.246 0 00-.75-.128H5.25c-.263 0-.515.045-.75.128m15 0A2.25 2.25 0 0121 12v6a2.25 2.25 0 01-2.25 2.25H5.25A2.25 2.25 0 013 18v-6c0-.98.626-1.813 1.5-2.122" />
            </svg>
          </template>
          <template #title>
            Framework/Libraries
          </template>
          <template #content>
            <div>- Laravel (PHP)</div>
            <div>- TailwindCSS/Bootstrap (CSS)</div>
            <div>- jQuery/VueJS (JS)</div>
          </template>
        </SkillCard>

        <SkillCard>
          <template #icon>
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="skill-icon">
              <path stroke-linecap="round" stroke-linejoin="round" d="M12 18v-5.25m0 0a6.01 6.01 0 001.5-.189m-1.5.189a6.01 6.01 0 01-1.5-.189m3.75 7.478a12.06 12.06 0 01-4.5 0m3.75 2.383a14.406 14.406 0 01-3 0M14.25 18v-.192c0-.983.658-1.823 1.508-2.316a7.5 7.5 0 10-7.517 0c.85.493 1.509 1.333 1.509 2.316V18" />
            </svg>
          </template>
          <template #title>
            Soft Skill
          </template>
          <template #content>
            <div>- Fast Learner</div>
            <div>- Friendly team player</div>
            <div>- Fluent in English, Mandarin</div>
            <div>& Bahasa Melayu</div>
          </template>
        </SkillCard>
      </div>
    </SectionComponent>

    <SectionComponent>
      <SectionTitle>
        <template #icon>
          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="h-8 w-8 lg:h-10 lg:w-10">
            <path stroke-linecap="round" stroke-linejoin="round" d="M14.25 6.087c0-.355.186-.676.401-.959.221-.29.349-.634.349-1.003 0-1.036-1.007-1.875-2.25-1.875s-2.25.84-2.25 1.875c0 .369.128.713.349 1.003.215.283.401.604.401.959v0a.64.64 0 01-.657.643 48.39 48.39 0 01-4.163-.3c.186 1.613.293 3.25.315 4.907a.656.656 0 01-.658.663v0c-.355 0-.676-.186-.959-.401a1.647 1.647 0 00-1.003-.349c-1.036 0-1.875 1.007-1.875 2.25s.84 2.25 1.875 2.25c.369 0 .713-.128 1.003-.349.283-.215.604-.401.959-.401v0c.31 0 .555.26.532.57a48.039 48.039 0 01-.642 5.056c1.518.19 3.058.309 4.616.354a.64.64 0 00.657-.643v0c0-.355-.186-.676-.401-.959a1.647 1.647 0 01-.349-1.003c0-1.035 1.008-1.875 2.25-1.875 1.243 0 2.25.84 2.25 1.875 0 .369-.128.713-.349 1.003-.215.283-.4.604-.4.959v0c0 .333.277.599.61.58a48.1 48.1 0 005.427-.63 48.05 48.05 0 00.582-4.717.532.532 0 00-.533-.57v0c-.355 0-.676.186-.959.401-.29.221-.634.349-1.003.349-1.035 0-1.875-1.007-1.875-2.25s.84-2.25 1.875-2.25c.37 0 .713.128 1.003.349.283.215.604.401.96.401v0a.656.656 0 00.658-.663 48.422 48.422 0 00-.37-5.36c-1.886.342-3.81.574-5.766.689a.578.578 0 01-.61-.58v0z" />
          </svg>
        </template>
        <template #title>Projects</template>
      </SectionTitle>
      <div id="content" class="flex flex-col space-y-5 justify-center items-center">
        <!-- First project -->
        <div class="left-right">
          <div class="left flex flex-col text-2xl bg-white p-2 rounded-lg shadow-md my-auto py-10 items-center">
            <div>
              Formative Assessment System
            </div>
            <div class="text-lg mt-5">
              A quiz-based assessment system built in PHP with Laravel framework as the backend and Blade/TailwindCSS for the frontend.
            </div>
            <div class="text-lg mt-2 flex items-center">
              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 mr-2">
                <path stroke-linecap="round" d="M15.75 10.5l4.72-4.72a.75.75 0 011.28.53v11.38a.75.75 0 01-1.28.53l-4.72-4.72M4.5 18.75h9a2.25 2.25 0 002.25-2.25v-9a2.25 2.25 0 00-2.25-2.25h-9A2.25 2.25 0 002.25 7.5v9a2.25 2.25 0 002.25 2.25z" />
              </svg>
              <a class="demo-button" href="https://drive.google.com/file/d/1GcP2rKCQZOexKQtdCeh9uqtU4P2sUvU1/view?usp=sharing" target="_blank">Demo</a>
            </div>
          </div>
          <div id="carousel-1" class="right carousel slide relative lg:w-2/3" data-bs-ride="carousel">
            <div class="carousel-indicators absolute right-0 bottom-0 left-0 flex justify-center p-0 mb-4">
              <button
                type="button"
                data-bs-target="#carousel-1"
                data-bs-slide-to="0"
                class="active"
                aria-current="true"
                aria-label="Slide 1"
              ></button>
              <button
                type="button"
                data-bs-target="#carousel-1"
                data-bs-slide-to="1"
                aria-label="Slide 2"
              ></button>
              <button
                type="button"
                data-bs-target="#carousel-1"
                data-bs-slide-to="2"
                aria-label="Slide 3"
              ></button>
              <button
                type="button"
                data-bs-target="#carousel-1"
                data-bs-slide-to="3"
                aria-label="Slide 4"
              ></button>
              <button
                type="button"
                data-bs-target="#carousel-1"
                data-bs-slide-to="4"
                aria-label="Slide 5"
              ></button>
              <button
                type="button"
                data-bs-target="#carousel-1"
                data-bs-slide-to="5"
                aria-label="Slide 6"
              ></button>
              <button
                type="button"
                data-bs-target="#carousel-1"
                data-bs-slide-to="6"
                aria-label="Slide 7"
              ></button>
            </div>
            <div class="carousel-inner relative w-full overflow-hidden">
              <div class="carousel-item active relative float-left w-full">
                <div class="relative overflow-hidden bg-no-repeat bg-cover" style="background-position: 50%;">
                  <img src="./assets/fas/quiz_edit.png" class="block w-full" />
                  <div class="absolute top-0 right-0 bottom-0 left-0 w-full h-full overflow-hidden bg-fixed bg-black opacity-20"></div>
                </div>
                <div class="carousel-caption hidden md:block absolute text-center">
                  <h5 class="text-xl">Quiz editing</h5>
                </div>
              </div>
              <div class="carousel-item relative float-left w-full">
                <div class="relative overflow-hidden bg-no-repeat bg-cover" style="background-position: 50%;">
                  <img src="./assets/fas/assignment_detail.png" class="block w-full" />
                  <div class="absolute top-0 right-0 bottom-0 left-0 w-full h-full overflow-hidden bg-fixed bg-black opacity-20"></div>
                </div>
                <div class="carousel-caption hidden md:block absolute text-center">
                  <h5 class="text-xl">Quiz evaluation</h5>
                </div>
              </div>
              <div class="carousel-item relative float-left w-full">
                <div class="relative overflow-hidden bg-no-repeat bg-cover" style="background-position: 50%;">
                  <img src="./assets/fas/quiz-1.png" class="block w-full" />
                  <div class="absolute top-0 right-0 bottom-0 left-0 w-full h-full overflow-hidden bg-fixed bg-black opacity-20"></div>
                </div>
                <div class="carousel-caption hidden md:block absolute text-center">
                  <h5 class="text-xl">Multiple choice question</h5>
                </div>
              </div>
              <div class="carousel-item relative float-left w-full">
                <div class="relative overflow-hidden bg-no-repeat bg-cover" style="background-position: 50%;">
                  <img src="./assets/fas/quiz-2.png" class="block w-full" />
                  <div class="absolute top-0 right-0 bottom-0 left-0 w-full h-full overflow-hidden bg-fixed bg-black opacity-20"></div>
                </div>
                <div class="carousel-caption hidden md:block absolute text-center">
                  <h5 class="text-xl">Open-ended question</h5>
                </div>
              </div>
              <div class="carousel-item relative float-left w-full">
                <div class="relative overflow-hidden bg-no-repeat bg-cover" style="background-position: 50%;">
                  <img src="./assets/fas/response-detail.png" class="block w-full" />
                  <div class="absolute top-0 right-0 bottom-0 left-0 w-full h-full overflow-hidden bg-fixed bg-black opacity-20"></div>
                </div>
                <div class="carousel-caption hidden md:block absolute text-center">
                  <h5 class="text-xl">Quiz grading (MCQ)</h5>
                </div>
              </div>
              <div class="carousel-item relative float-left w-full">
                <div class="relative overflow-hidden bg-no-repeat bg-cover" style="background-position: 50%;">
                  <img src="./assets/fas/response-detail-2.png" class="block w-full" />
                  <div class="absolute top-0 right-0 bottom-0 left-0 w-full h-full overflow-hidden bg-fixed bg-black opacity-20"></div>
                </div>
                <div class="carousel-caption hidden md:block absolute text-center">
                  <h5 class="text-xl">Quiz grading (OEQ)</h5>
                </div>
              </div>
            </div>
            <button
              class="carousel-control-prev absolute top-0 bottom-0 flex items-center justify-center p-0 text-center border-0 hover:outline-none hover:no-underline focus:outline-none focus:no-underline left-0"
              type="button"
              data-bs-target="#carousel-1"
              data-bs-slide="prev"
            >
              <span class="carousel-control-prev-icon inline-block bg-no-repeat" aria-hidden="true"></span>
              <span class="visually-hidden">Previous</span>
            </button>
            <button
              class="carousel-control-next absolute top-0 bottom-0 flex items-center justify-center p-0 text-center border-0 hover:outline-none hover:no-underline focus:outline-none focus:no-underline right-0"
              type="button"
              data-bs-target="#carousel-1"
              data-bs-slide="next"
            >
              <span class="carousel-control-next-icon inline-block bg-no-repeat" aria-hidden="true"></span>
              <span class="visually-hidden">Next</span>
            </button>
          </div>
        </div>
        <!-- Second Project -->
        <div class="left-right">
          <div id="carousel-2" class="right carousel slide relative lg:w-2/3" data-bs-ride="carousel">
            <div class="carousel-indicators absolute right-0 bottom-0 left-0 flex justify-center p-0 mb-4">
              <button
                type="button"
                data-bs-target="#carousel-2"
                data-bs-slide-to="0"
                class="active"
                aria-current="true"
                aria-label="Slide 1"
              ></button>
              <button
                type="button"
                data-bs-target="#carousel-2"
                data-bs-slide-to="1"
                aria-label="Slide 2"
              ></button>
              <button
                type="button"
                data-bs-target="#carousel-2"
                data-bs-slide-to="2"
                aria-label="Slide 3"
              ></button>
            </div>
            <div class="carousel-inner relative w-full overflow-hidden">
              <div class="carousel-item active relative float-left w-full">
                <div class="relative overflow-hidden bg-no-repeat bg-cover" style="background-position: 50%;">
                  <img src="./assets/ffos/main-page.png" class="block w-full" />
                  <div class="absolute top-0 right-0 bottom-0 left-0 w-full h-full overflow-hidden bg-fixed bg-black opacity-20"></div>
                </div>
                <div class="carousel-caption hidden md:block absolute text-center">
                  <h5 class="text-xl">Food Ordering Homepage</h5>
                </div>
              </div>
              <div class="carousel-item relative float-left w-full">
                <div class="relative overflow-hidden bg-no-repeat bg-cover" style="background-position: 50%;">
                  <img src="./assets/ffos/menu-view.png" class="block w-full" />
                  <div class="absolute top-0 right-0 bottom-0 left-0 w-full h-full overflow-hidden bg-fixed bg-black opacity-20"></div>
                </div>
                <div class="carousel-caption hidden md:block absolute text-center">
                  <h5 class="text-xl">Menu Details</h5>
                </div>
              </div>
              <div class="carousel-item relative float-left w-full">
                <div class="relative overflow-hidden bg-no-repeat bg-cover" style="background-position: 50%;">
                  <img src="./assets/ffos/shopping-cart.png" class="block w-full" />
                  <div class="absolute top-0 right-0 bottom-0 left-0 w-full h-full overflow-hidden bg-fixed bg-black opacity-20"></div>
                </div>
                <div class="carousel-caption hidden md:block absolute text-center">
                  <h5 class="text-xl">Checkout Page</h5>
                </div>
              </div>
            </div>
            <button
              class="carousel-control-prev absolute top-0 bottom-0 flex items-center justify-center p-0 text-center border-0 hover:outline-none hover:no-underline focus:outline-none focus:no-underline left-0"
              type="button"
              data-bs-target="#carousel-2"
              data-bs-slide="prev"
            >
              <span class="carousel-control-prev-icon inline-block bg-no-repeat" aria-hidden="true"></span>
              <span class="visually-hidden">Previous</span>
            </button>
            <button
              class="carousel-control-next absolute top-0 bottom-0 flex items-center justify-center p-0 text-center border-0 hover:outline-none hover:no-underline focus:outline-none focus:no-underline right-0"
              type="button"
              data-bs-target="#carousel-2"
              data-bs-slide="next"
            >
              <span class="carousel-control-next-icon inline-block bg-no-repeat" aria-hidden="true"></span>
              <span class="visually-hidden">Next</span>
            </button>
          </div>
          <div class="left flex flex-col text-2xl bg-white p-2 rounded-lg shadow-md my-auto py-10 items-center">
            <div>
              Fast Food Ordering System
            </div>
            <div class="text-lg mt-5">
              A basic food ordering website written in HTML,CSS and PHP with MySQL as database running on XAMPP.
            </div>
            <div class="text-lg mt-2 flex items-center">
              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 mr-2">
                <path stroke-linecap="round" d="M15.75 10.5l4.72-4.72a.75.75 0 011.28.53v11.38a.75.75 0 01-1.28.53l-4.72-4.72M4.5 18.75h9a2.25 2.25 0 002.25-2.25v-9a2.25 2.25 0 00-2.25-2.25h-9A2.25 2.25 0 002.25 7.5v9a2.25 2.25 0 002.25 2.25z" />
              </svg>
              <a class="demo-button" href="https://drive.google.com/file/d/1sFDq7HMdVMkItm6PdeDUhTjPOm0UBtgR/view?usp=sharing" target="_blank">Demo</a>
            </div>
          </div>
        </div>
      </div>
    </SectionComponent>
  </div>

  <footer class="flex flex-col justify-center items-center p-5 bg-white rounded-sm shadow-md text-lg w-full space-y-2">
    <div class="flex space-x-5">
      <a href="https://github.com/CyanKelv" target="_blank">
        <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="w-12 h-12" viewBox="0 0 16 16">
          <path d="M15.698 7.287 8.712.302a1.03 1.03 0 0 0-1.457 0l-1.45 1.45 1.84 1.84a1.223 1.223 0 0 1 1.55 1.56l1.773 1.774a1.224 1.224 0 0 1 1.267 2.025 1.226 1.226 0 0 1-2.002-1.334L8.58 5.963v4.353a1.226 1.226 0 1 1-1.008-.036V5.887a1.226 1.226 0 0 1-.666-1.608L5.093 2.465l-4.79 4.79a1.03 1.03 0 0 0 0 1.457l6.986 6.986a1.03 1.03 0 0 0 1.457 0l6.953-6.953a1.031 1.031 0 0 0 0-1.457"/>
        </svg>
      </a>
      <a href="mailto:jialiang88@gmail.com">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="w-12 h-12">
          <path d="M1.5 8.67v8.58a3 3 0 003 3h15a3 3 0 003-3V8.67l-8.928 5.493a3 3 0 01-3.144 0L1.5 8.67z" />
          <path d="M22.5 6.908V6.75a3 3 0 00-3-3h-15a3 3 0 00-3 3v.158l9.714 5.978a1.5 1.5 0 001.572 0L22.5 6.908z" />
        </svg>
      </a>
    </div>
    <div class="relative flex py-1 items-center w-full">
      <div class="flex-grow border-t border-gray-400"></div>
      <span class="flex-shrink mx-4 text-gray-400">© 2022 Made by Ng Jia Liang</span>
      <div class="flex-grow border-t border-gray-400"></div>
    </div>
  </footer>
</template>

<script>
import SkillCard from './components/SkillCard.vue';
import SectionTitle from './components/SectionTitle.vue';
import SectionComponent from './components/SectionComponent.vue';

export default {
  name: 'App',
  components: {
    SkillCard,
    SectionTitle,
    SectionComponent
}
}
</script>

<style>
html, body {
  @apply h-auto min-w-fit min-h-fit;
}

#app {
  @apply font-sans;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-image: linear-gradient(to bottom right, indigo, white);
}

.left-right {
  @apply flex flex-col lg:flex-row justify-center w-5/6 rounded-2xl bg-gray-300 space-y-2 lg:space-x-5 p-5 items-center;
}

.left {
  @apply w-full h-full lg:w-1/3;
}
.right {
  @apply w-full h-full lg:w-2/3;
}

.demo-button {
  @apply bg-blue-500 text-white px-2 rounded-2xl hover:scale-110 duration-700 ease-in-out;
}

.skill-card {
 @apply flex flex-col bg-gray-300 rounded-lg p-5 justify-center items-center space-y-3;
}

.skill-icon {
  @apply w-32 h-32 bg-white rounded-full p-2;
}

#left {

}
</style>
