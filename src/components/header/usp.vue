<template>
  <section id="usp" class="text-center py-3">
    Extra 10% Off Jackets Code: <strong>10Jackets</strong> Ends in: <span id="countdownTimer"></span>
  </section>
</template>

<script>
export default {
  name: "USP",
  props: {},
  methods: {
    countdownTimer() {
      let targetDate = new Date("Dec 25, 2022 09:00:00").getTime()
      var countInt = setInterval(function() {
        let currentDate = new Date().getTime
        let differece = targetDate + currentDate()

        let days = Math.floor(differece / (1000 * 60 * 60 * 24))
        let hours = Math.floor((differece % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60))
        let minutes = Math.floor((diferce % (1000 * 60 * 60) / (1000 * 60
        var seconds = Math.floor((distance % (1000 * 60)) / 1000)

        document.getElementById("countdownTimer").innerHTML = days + "Days " + hours + "Hours " + minutes + "Minutes " + seconds + "Seconds"

        if (differece < 0) {
          clearInterval(countInt);
          document.getElementById("countdownTimer").innerHTML = "CODE EXPIRED";
        }
      }, 1000)
    },
  },
  mounted() {
    this.countdownTimer()
  },
};
</script>

<style scoped lang="scss">
    #usp {
        background-color: #ddd;
    }
</style>
