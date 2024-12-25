<template>
  <header class="flex items-center justify-between p-4 text-gray-400">
    <div class="flex items-center">
      <div class="p-2 border-gray-400 border-2 rounded-full">
        <svg class="w-4 h-4 text-gray-400" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none"
          viewBox="0 0 24 24">
          <path stroke="currentColor" stroke-linecap="round" stroke-width="2"
            d="m3.5 5.5 7.893 6.036a1 1 0 0 0 1.214 0L20.5 5.5M4 19h16a1 1 0 0 0 1-1V6a1 1 0 0 0-1-1H4a1 1 0 0 0-1 1v12a1 1 0 0 0 1 1Z" />
        </svg>

      </div>
      <a href="mailto:jialiang88@gmail.com">
        <span
          class="px-4 py-0 rounded-md text-gray-400 hover:text-white transition duration-300">jialiang88@gmail.com</span>
      </a>
    </div>
    <LinksComponent />
  </header>
  <div id="wrapper" class="h-full md:w-2/3 lg:w-4/5 mx-auto justify-center flex flex-col pb-10 space-y-20">
    <SectionComponent>
      <div class="profile-container">
        <img class="profile-picture" src="./assets/Profile.jpg" alt="Profile Picture" />
        <p>Hi, I'm Kelvin! 👋 <br> Multimedia University Graduate</p>
        <h1 class="profile-header">Software Engineer,<br> Web Developer</h1>
      </div>
    </SectionComponent>

    <SectionComponent>
      <SectionTitle>
        <template #title>Tech Stack & Framework</template>
      </SectionTitle>
      <div id="content"
        class="flex flex-col mx-5 space-y-5 lg:mx-0 lg:flex-row lg:space-x-5 lg:space-y-0 justify-center">
        <SkillCard>
          <template #icon>
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
              stroke="currentColor" class="skill-icon">
              <path stroke-linecap="round" stroke-linejoin="round"
                d="M4.26 10.147a60.436 60.436 0 00-.491 6.347A48.627 48.627 0 0112 20.904a48.627 48.627 0 018.232-4.41 60.46 60.46 0 00-.491-6.347m-15.482 0a50.57 50.57 0 00-2.658-.813A59.905 59.905 0 0112 3.493a59.902 59.902 0 0110.399 5.84c-.896.248-1.783.52-2.658.814m-15.482 0A50.697 50.697 0 0112 13.489a50.702 50.702 0 017.74-3.342M6.75 15a.75.75 0 100-1.5.75.75 0 000 1.5zm0 0v-3.675A55.378 55.378 0 0112 8.443m-7.007 11.55A5.981 5.981 0 006.75 15.75v-1.5" />
            </svg>
          </template>
          <template #title>
            Programming Languages
          </template>
          <template #content>
            <div>• JavaScript, TypeScript, HTML, CSS</div>
            <div>• MySQL/SQL Database/Oracle</div>
            <div>• PHP, Java, Python</div>
          </template>
        </SkillCard>

        <SkillCard>
          <template #icon>
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
              stroke="currentColor" class="skill-icon">
              <path stroke-linecap="round" stroke-linejoin="round"
                d="M6 6.878V6a2.25 2.25 0 012.25-2.25h7.5A2.25 2.25 0 0118 6v.878m-12 0c.235-.083.487-.128.75-.128h10.5c.263 0 .515.045.75.128m-12 0A2.25 2.25 0 004.5 9v.878m13.5-3A2.25 2.25 0 0119.5 9v.878m0 0a2.246 2.246 0 00-.75-.128H5.25c-.263 0-.515.045-.75.128m15 0A2.25 2.25 0 0121 12v6a2.25 2.25 0 01-2.25 2.25H5.25A2.25 2.25 0 013 18v-6c0-.98.626-1.813 1.5-2.122" />
            </svg>
          </template>
          <template #title>
            Framework
          </template>
          <template #content>
            <div>• Angular/VueJS/Webix (JS/TS)</div>
            <div>• Laravel (PHP)</div>
            <div>• TailwindCSS/Bootstrap (CSS)</div>
          </template>
        </SkillCard>

        <SkillCard>
          <template #icon>
            <svg class="skill-icon" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="currentColor"
              viewBox="0 0 24 24">
              <path fill-rule="evenodd"
                d="M20.337 3.664c.213.212.354.486.404.782.294 1.711.657 5.195-.906 6.76-1.77 1.768-8.485 5.517-10.611 6.683a.987.987 0 0 1-1.176-.173l-.882-.88-.877-.884a.988.988 0 0 1-.173-1.177c1.165-2.126 4.913-8.841 6.682-10.611 1.562-1.563 5.046-1.198 6.757-.904.296.05.57.191.782.404ZM5.407 7.576l4-.341-2.69 4.48-2.857-.334a.996.996 0 0 1-.565-1.694l2.112-2.111Zm11.357 7.02-.34 4-2.111 2.113a.996.996 0 0 1-1.69-.565l-.422-2.807 4.563-2.74Zm.84-6.21a1.99 1.99 0 1 1-3.98 0 1.99 1.99 0 0 1 3.98 0Z"
                clip-rule="evenodd" />
            </svg>
          </template>
          <template #title>
            Development
          </template>
          <template #content>
            <div>• Docker for build/deployment</div>
            <div>• Git/Github/Gitlab</div>
            <div>• Jasmine Unit Testing</div>
          </template>
        </SkillCard>

        <SkillCard>
          <template #icon>
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
              stroke="currentColor" class="skill-icon">
              <path stroke-linecap="round" stroke-linejoin="round"
                d="M12 18v-5.25m0 0a6.01 6.01 0 001.5-.189m-1.5.189a6.01 6.01 0 01-1.5-.189m3.75 7.478a12.06 12.06 0 01-4.5 0m3.75 2.383a14.406 14.406 0 01-3 0M14.25 18v-.192c0-.983.658-1.823 1.508-2.316a7.5 7.5 0 10-7.517 0c.85.493 1.509 1.333 1.509 2.316V18" />
            </svg>
          </template>
          <template #title>
            Soft Skill
          </template>
          <template #content>
            <div>• Fast Learner</div>
            <div>• Friendly team player</div>
            <div>• Fluent in English, Mandarin</div>
            <div>& Bahasa Melayu</div>
          </template>
        </SkillCard>
      </div>
    </SectionComponent>

    <SectionComponent>
      <SectionTitle>
        <template #icon>
          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
            stroke="currentColor" class="h-8 w-8 lg:h-10 lg:w-10">
            <path stroke-linecap="round" stroke-linejoin="round"
              d="M14.25 6.087c0-.355.186-.676.401-.959.221-.29.349-.634.349-1.003 0-1.036-1.007-1.875-2.25-1.875s-2.25.84-2.25 1.875c0 .369.128.713.349 1.003.215.283.401.604.401.959v0a.64.64 0 01-.657.643 48.39 48.39 0 01-4.163-.3c.186 1.613.293 3.25.315 4.907a.656.656 0 01-.658.663v0c-.355 0-.676-.186-.959-.401a1.647 1.647 0 00-1.003-.349c-1.036 0-1.875 1.007-1.875 2.25s.84 2.25 1.875 2.25c.369 0 .713-.128 1.003-.349.283-.215.604-.401.959-.401v0c.31 0 .555.26.532.57a48.039 48.039 0 01-.642 5.056c1.518.19 3.058.309 4.616.354a.64.64 0 00.657-.643v0c0-.355-.186-.676-.401-.959a1.647 1.647 0 01-.349-1.003c0-1.035 1.008-1.875 2.25-1.875 1.243 0 2.25.84 2.25 1.875 0 .369-.128.713-.349 1.003-.215.283-.4.604-.4.959v0c0 .333.277.599.61.58a48.1 48.1 0 005.427-.63 48.05 48.05 0 00.582-4.717.532.532 0 00-.533-.57v0c-.355 0-.676.186-.959.401-.29.221-.634.349-1.003.349-1.035 0-1.875-1.007-1.875-2.25s.84-2.25 1.875-2.25c.37 0 .713.128 1.003.349.283.215.604.401.96.401v0a.656.656 0 00.658-.663 48.422 48.422 0 00-.37-5.36c-1.886.342-3.81.574-5.766.689a.578.578 0 01-.61-.58v0z" />
          </svg>
        </template>
        <template #title>Projects Showcase</template>
      </SectionTitle>
      <div id="content" class="flex flex-col space-y-5 justify-center items-center">
        <!-- First project -->
        <ProjectComponent :carousel="carousel1" />

        <!-- Second Project -->
        <ProjectComponent :carousel="carousel2" />

        <!-- Third Project -->
        <ProjectComponent :carousel="carousel3" />
      </div>
    </SectionComponent>
  </div>

  <footer class="flex items-center justify-between p-4 bg-zinc-800 text-gray-400">
    <div class="flex items-center space-x-2">
      <span>&copy; 2024 Ng Jia Liang</span>
    </div>

    <LinksComponent />
  </footer>
</template>

<script>
import SkillCard from './components/SkillCard.vue';
import SectionTitle from './components/SectionTitle.vue';
import SectionComponent from './components/SectionComponent.vue';
import LinksComponent from './components/LinksComponent.vue';
import ProjectComponent from './components/ProjectComponent.vue';
import "./assets/style.css";

export default {
  name: 'App',
  components: {
    SkillCard,
    SectionTitle,
    SectionComponent,
    LinksComponent,
    ProjectComponent
  },
  data() {
    return {
      carousel1: {
        id: 1,
        type: "left-right",
        title: "Formative Assessment System",
        description: "A quiz-based assessment system built in PHP with Laravel framework as the backend and Blade/TailwindCSS for the frontend.",
        buttonType: "demo",
        link: "https://drive.google.com/file/d/1GcP2rKCQZOexKQtdCeh9uqtU4P2sUvU1/view?usp=sharing",
        images: [
          { link: require("./assets/fas/quiz_edit.png"), description: "Quiz editing" },
          { link: require("./assets/fas/assignment_detail.png"), description: "Quiz evaluation" },
          { link: require("./assets/fas/quiz-1.png"), description: "Multiple choice question" },
          { link: require("./assets/fas/quiz-2.png"), description: "Open-ended question" },
          { link: require("./assets/fas/response-detail.png"), description: "Quiz grading (MCQ)" },
          { link: require("./assets/fas/response-detail-2.png"), description: "Quiz grading (OEQ)" }
        ]
      },
      carousel2: {
        id: 2,
        type: "right-left",
        title: "Fast Food Ordering System",
        description: "A basic food ordering website written in HTML,CSS and PHP with MySQL as database running on XAMPP.",
        buttonType: "demo",
        link: "https://drive.google.com/file/d/1sFDq7HMdVMkItm6PdeDUhTjPOm0UBtgR/view?usp=sharing",
        images: [
          { link: require("./assets/ffos/main-page.png"), description: "Food Ordering Homepage" },
          { link: require("./assets/ffos/menu-view.png"), description: "Menu Details" },
          { link: require("./assets/ffos/shopping-cart.png"), description: "Checkout Page" }
        ]
      },
      carousel3: {
        id: 3,
        type: "left-right",
        title: "TMFORCE Workforce Management System",
        description: "System widely used by Telekom Malaysia Organization to manage day-to-day workforce operations.",
        buttonType: "link",
        link: "https://www.tmrnd.com.my/workforce-management-system/",
        images: [
          { link: require("./assets/force.jpg"), description: "TMFORCE" },
        ]
      }
    }
  }
}
</script>
