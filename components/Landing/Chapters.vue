<template>
  <div class="section container">
    <div class="columns is-centered">
      <div class="column is-4" v-for="(item, index) in row1" :key="index">
        <div class="card">
          <div class="card-content">
            <div class="level">
              <div class="level-item">
                <figure class="image is-48x48">
                  <font-awesome-icon :icon="item.icon" size="3x" />
                </figure>
              </div>
            </div>
            <h1 class="title is-size-4 has-text-centered">
              {{ item.header }}
            </h1>
            <p class="subtitle has-text-centered">
              {{ item.subheader }}
            </p>
          </div>
        </div>
      </div>
    </div>
    <div class="columns is-centered">
      <div class="column is-4" v-for="(item, index) in row2" :key="index">
        <div class="card">
          <div class="card-content">
            <div class="level">
              <div class="level-item">
                <figure class="image is-48x48">
                  <font-awesome-icon :icon="item.icon" size="3x" />
                </figure>
              </div>
            </div>
            <h1 class="title is-size-4 has-text-centered">
              {{ item.header }}
            </h1>
            <p class="subtitle has-text-centered text-primary">
              {{ item.subheader }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.card {
  min-height: 180px;
  padding-top: 1.5rem;
  padding-bottom: 1.5rem;
  background-color: #ade9ec;
  box-shadow: 5px 5px 10px #888888;
}

</style>
<script>
export default {
  data() {
    return {
      row1: [
        {
          header: "Competitive Programming",
          subheader:
            "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Architecto, voluptatum.",
          icon: ["fas", "code"]
        },
        {
          header: "Security",
          subheader:
            "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Architecto, voluptatum.",
          icon: ["fas", "user-secret"]
        },
        {
          header: "Web Development",
          subheader:
            "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Architecto, voluptatum.",
          icon: ["fab", "html5"]
        }
      ],
      row2: [
        {
          header: "Machine Learning",
          subheader:
            "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Architecto, voluptatum.",
          icon: ["fas", "robot"]
        },
        {
          header: "Development",
          subheader:
            "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Architecto, voluptatum.",
          icon: ["fab", "android"]
        },
      ]
    };
  }
};
</script>
