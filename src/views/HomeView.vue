<template>
  <div class='home'>

    <div class="flex-container">
      <v-card id="cathCard" class="mx-auto" max-width="240" @click="goAct">
        <v-img src="@/assets/activityhobby.png" height="200px" cover></v-img>

        <v-card-title>
          Activity
        </v-card-title>

      </v-card>
      <v-card id="cathCard" class="mx-auto" max-width="240" @click="goArt">
        <v-img src="@/assets/artshobby.png" height="200px" cover></v-img>

        <v-card-title>
          Arts
        </v-card-title>

      </v-card>
      <v-card id="cathCard" class="mx-auto" max-width="240" @click="goCol">
        <v-img src="@/assets/collectinghobby.png" height="200px" cover></v-img>

        <v-card-title>
          Collecting
        </v-card-title>

      </v-card>
      <v-card id="cathCard" class="mx-auto" max-width="240" @click="goMak">
        <v-img src="@/assets/makinghobby.png" height="200px" cover></v-img>

        <v-card-title>
          Making
        </v-card-title>

      </v-card>
      <v-card id="cathCard" class="mx-auto" max-width="240" @click="goPla">
        <v-img src="@/assets/playhobby.png" height="200px" cover></v-img>

        <v-card-title>
          Play
        </v-card-title>

      </v-card>
    </div>

  </div>
</template>

<script>

export default {
  name: 'Home',
  methods: {
    goAct() {
      this.$router.push({ name: "activity" })
    },
    goArt() {
      this.$router.push({ name: "art" })
    },
    goCol() {
      this.$router.push({ name: "collect" })
    },
    goMak() {
      this.$router.push({ name: "make" })
    },
    goPla() {
      this.$router.push({ name: "play" })
    }
  }
}

</script>
<style lang="scss">
.flex-container {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: flex-start;
  margin-top: 150px;
}

#cathCard {
  margin: 30px;
}

#cathCard:hover {
  cursor: pointer;
}
</style>
