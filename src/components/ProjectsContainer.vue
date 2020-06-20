<template>
  <div class="container">
    <div class="columns">
      <ProjectCard
        projectTitle="This is my title for project1"
        projectDetails="some details"
        projectGithubUrl="some url"
        projectUrl="some url2"
      />
      <ProjectCard projectTitle="This is my title for project2" />
      <ProjectCard projectTitle="This is my title for project3" />
    </div>
    <div class="container columns">
      <ProjectCard projectTitle="This is my title for project4" />
      <ProjectCard projectTitle="This is my title for project5" />
      <ProjectCard projectTitle="This is my title for project6" />
    </div>
  </div>
</template>

<script>
import ProjectCard from "./ProjectCard";
export default {
  name: "ProjectsContainer",
  components: {
    ProjectCard
  }
};
</script>

<style scoped>
.columns {
  border: 2px solid purple;
  margin-right: auto;
  margin-left: auto;
  padding-bottom: 5vh;
}
</style>