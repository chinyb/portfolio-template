<template>
  <div class="flex flex-col w-screen h-full">
    <!-- Your name, profile picture and contact -->
    <HeadWrapper
      name="Chin"
      title="Full Stack Developer"
      userImgURL="../img/imgex.jpeg"
      phone="+60 164433610"
      email="mynamesyong@live.com"
    />
    <!-- About Me -->
    <AboutWrapper
      aboutMe="Hello Hello Hello"
      linkedInURL="https://www.linkedin.com/in/yong-bin-chin-3a053b113/"
      languages="English, Malay, Chinese, French, Korean, Japanese"
      nationality="Malaysian"
      interest="fun"
    />
    <!-- Working Experience -->
    <CareerWrapper>
      <template v-slot:career>
        <Career
          companyName="BASF-Petronas Chemicals"
          title="Production Engineer"
          startDate="June 2019"
          endDate="present"
        >
          <!-- List of what you had did in the company -->
          <template v-slot:experience>
            <ul class="text-gray-600 list-inside list-disc mt-2 px-4">
              <li>Created web application for streamlined information extraction.</li>
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
            </ul>
          </template>
        </Career>

        <Career
          companyName="Company Name"
          title="Your Job Title"
          startDate="Start Date"
          endDate="End Date"
        >
          <!-- List of what you had did in the company -->
          <template v-slot:experience>
            <ul class="text-gray-600 list-inside list-disc mt-2 px-4">
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
            </ul>
          </template>
        </Career>

        <Career
          companyName="Company Name"
          title="Your Job Title"
          startDate="Start Date"
          endDate="End Date"
        >
          <!-- List of what you had did in the company -->
          <template v-slot:experience>
            <ul class="text-gray-600 list-inside list-disc mt-2 px-4">
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
            </ul>
          </template>
        </Career>
      </template>
    </CareerWrapper>
    <!-- Achievement -->
    <AchievementWrapper project="2" client="3" award="1"/>
    <!-- Portfolio -->
    <PortfolioWrapper>
      <template v-slot:portfolio>
        <div class="grid grid-cols-1 md:grid-cols-3">
          <ProjectCard
            imgUrl="../img/github.png"
            name="Project Name"
            project="Project Type"
            projectURL="https://github.com"
          />

          <ProjectCard
            imgUrl="../img/github.png"
            name="Project Name"
            project="Project Type"
            projectURL="https://github.com"
          />

          <ProjectCard
            imgUrl="../img/github.png"
            name="Project Name"
            project="Project Type"
            projectURL="https://github.com"
          />
        </div>
      </template>
    </PortfolioWrapper>
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: "Chin Yong Bin"
    };
  }
};
</script>