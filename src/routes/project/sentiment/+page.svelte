<script lang="ts">
  import { language } from "$lib/interfaces";
  import Project from "$lib/Project.svelte";
  const data = {
    banner: {
      cover: "/project/sentiment/_cover.jpg",
      title: "Yukka Lab",
      slogan: "Sentiment",
    },
    date: "April 2018",
    gallery: [
      "/project/sentiment/yukkalab-sentiment-01.png",
      "/project/sentiment/yukkalab-sentiment-02.png",
      "/project/sentiment/yukkalab-sentiment-03.png",
      "/project/sentiment/yukkalab-sentiment-04.png",
    ],
    lang: [language.angular, language.material, language.highchart],
    more: [
      {
        name: "Network",
        link: "network",
      },
      {
        name: "Chartmap",
        link: "chartmap",
      },
      {
        name: "Signals",
        link: "signals",
      },
    ],
  };
</script>

<Project {data}>
  <p>
    This project was part of the cockpit of Yukkalab it displays the stock of
    different markets using Highcharts, Angular, and Material. The chart is
    composed of 3 series in 2 different axes, 2 of them combined together
    showing the negative or positive evaluation with an area chart with
    different colors and the last one at the bottom display the investment in
    percentage.
  </p>
</Project>
