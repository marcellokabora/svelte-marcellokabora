<script>
  import Gallery from "$lib/Gallery.svelte";
  import Section from "$lib/Section.svelte";
  import Header from "$lib/Header.svelte";
  import Carousel from "$lib/Carousel.svelte";
  import Projects from "$lib/Projects.svelte";

  const company = {
    cover: "/photo/back2.jpg",
    title: "CAREER",
    slogan: "I worked for different startup in Berlin and Italy",
    items: [
      {
        logo: "/company/evaglobal.jpg",
        company: "Eva Global",
        title: "Frontend Engineer",
        time: "Oct 2022 - May 2024",
        link: "//evaglobal.com",
      },
      {
        logo: "/company/linus.png",
        company: "Linus",
        title: "Frontend Engineer",
        time: "Sep 2021 - Aug 2022",
        link: "//linus-finance.com",
      },
      {
        logo: "/company/buildingminds.png",
        company: "Buildingminds",
        title: "Frontend Developer ",
        time: "Jan 2020 - Aug 2021",
        link: "//buildingminds.com",
      },
      {
        logo: "/company/yukkalab.png",
        company: "Yukkalab",
        title: "Frontend Developer",
        time: "Jun 2017 - Nov 2019",
        link: "//yukkalab.com",
      },
      {
        logo: "/company/smava.png",
        company: "Smava",
        title: "Frontend Developer",
        time: "Feb 2016 - Nov 2016",
        link: "//smava.de",
      },
      {
        logo: "/company/tanglang.png",
        company: "Tang Lang",
        title: "Fullstack Developer",
        time: "Apr 2014 - Dec 2015",
      },
      {
        logo: "/company/maggiolino.png",
        company: "Maggiolino",
        title: "Fullstack Developer",
        time: "Aug 2013 - Jan 2015",
      },
      // {
      // 	logo: '/company/petdog.png',
      // 	company: 'Annunci Animali',
      // 	title: 'Frontend Developer',
      // 	time: 'Mar 2013 - Oct 2014'
      // },
      {
        logo: "/company/airesis.png",
        company: "Airesis",
        title: "UI Designer",
        time: "Apr 2011 - Apr 2012",
      },
    ],
  };

  const language = {
    cover: "/gallery/back2.jpg",
    title: "LANGUAGE",
    items: [
      {
        logo: "/flag/it.png",
        company: "Italian",
        title: "100%",
      },
      {
        logo: "/flag/en.png",
        company: "English",
        title: "100% ",
      },
      {
        logo: "/flag/sp.png",
        company: "Spanish",
        title: "40%",
      },
    ],
  };
</script>

<svelte:head>
  <title>Marcello Kabora | Fronted Engineer</title>
  <meta
    name="description"
    content="Frontend Engineer with over 12 years of experience in frontend development, user interface, graphic design, data visualization, and progressive web app"
  />
  <meta
    name="keywords"
    content="Software, Engineer, Frontend, Fullstack, Developer, UI/UX, Nodejs, Svelte, Angular, Material, D3,, NX, Firebase, Data Visualization"
  />
  <meta name="thumbnail" content="/gallery/keyboard.jpg" />
  <meta property="og:image" content="/gallery/keyboard.jpg" />
</svelte:head>

<Gallery />

<section>
  <Header
    classe="headtito"
    title="ABOUT"
    slogan="I am passionate about user interface and user experience"
  />

  <div class="space" />

  <Section photo="/photo/software.jpg" title="Software">
    <p>
      A web application is internet-based software accessed via web browsers,
      offering platform-independent access, centralized maintenance, and diverse
      functionalities. It uses web technologies and ensures cross-browser
      compatibility and security. Staying updated with the current technology,
      using tools like <a href="//code.visualstudio.com/" target="_blank">VSC</a
      >
      and <a href="//google.com/chrome/" target="_blank">Chrome</a>, enables
      <b>real-time testing</b> and simplifies <b>complex layout design</b>.
    </p>
  </Section>
  <Section photo="/photo/develop.jpeg" title="Framework" aside>
    <p>
      Using an appropriate framework is essential for a developer because it
      saves important time and effort in building an app. I like to work using
      <b>object-oriented</b> programming languages to build complex features and
      maintain scalable functionality using different frameworks like
      <a href="//svelte.com" target="_blank">Svelte</a>,
      <a href="//reactjs.org" target="_blank">React</a>,
      <a href="//vuejs.org" target="_blank">Vue</a> and
      <a href="//angular.io" target="_blank">Angular</a>.
    </p>
  </Section>
  <Section photo="/photo/styling.jpg" title="Styling">
    <p>
      CSS or Cascading Style Sheets is a style sheet language used for
      describing the presentation of a document written in a markup language
      such as HTML, in particular, SCSS is used in different libraries like
      <b>material design</b>. For me is extremely easy to develop complex
      layouts using this technology with the help of auto complete and nested
      classes.
    </p>
  </Section>
  <Section photo="/photo/visualization.jpeg" title="Visualization" aside>
    <p>
      Data visualization is an interdisciplinary field that deals with the
      graphic representation of data and it is a particularly efficient way of
      communicating when the data is numerous for example a <b>Time Series</b>.
      I use
      <a href="//d3js.org" target="_blank">D3js</a> or
      <a href="//highcharts.com" target="_blank">Highcharts</a> to communicate information
      clearly and efficiently building statistical graphics, plots, or information
      graphics.
    </p>
  </Section>

  <div class="space" />
</section>

<Carousel
  title={company.title}
  slogan={company.slogan}
  cover={company.cover}
  items={company.items}
  perpage={4}
/>

<section>
  <div class="space" />

  <Header
    classe="headtito"
    title="ENVIROMENT"
    slogan="Develop programs by analysing and identifying areas for modification"
  />

  <div class="space" />

  <Section
    photo="/photo/angular.png"
    title="Framework"
    color="#1976d2"
    link="//angular.io"
  >
    <p>
      <a href="//angular.io" target="_blank">Angular</a> and
      <a href="https://svelte.dev" target="_blank">Svelte</a> are my preferred framework
      because they are great for scalable projects and allow me to interact with
      the best providers in the market. I can build any projects with unitest and
      extend it with authentication and pipes to control any single feature.
    </p>
  </Section>
  <Section
    photo="/photo/layer.png"
    title="Material"
    color="#00e89d"
    link="//material.angular.io"
    aside
  >
    <p>
      <a href="//material.angular.io" target="_blank">Material</a> is the best
      framework for styling it offers a large list of components ready to be
      used perfect built-in responsive designing integration for any
      <a href="//angular.io" target="_blank">Angular</a> project, it provide tools
      that help developers build their own custom components with common interaction
      patterns.
    </p>
  </Section>

  <Section
    photo="/photo/highchart.png"
    title="Visualization"
    color="#ffb8b8"
    link="//web.dev/progressive-web-apps"
  >
    <p>
      To communicate information clearly and efficiently, data visualization
      uses statistical graphics, plots, information graphics and other tools.
      Numerical data may be encoded using dots, lines, or bars, to visually
      communicate a quantitative message. <a href="/">Highcharts</a>
      and <a href="/">D3</a> are my favorites library to create and explore new ideas.
    </p>
  </Section>

  <Section
    photo="/photo/firebase.webp"
    title="Database"
    color="#4fb7e8"
    link="//firebase.google.com"
    aside
  >
    <p>
      <a href="//firebase.google.com" target="_blank">Firebase</a> and
      <a href="https://aws.amazon.com/" target="_blank">AWS</a> are my favorite tools
      for working with databases that allow me to deliver richer app experiences.
      Firebase manages its own infrastructure with a nice set of tools to simplify
      the workflow of the developer by providing them with development kits and an
      online dashboard.
    </p>
  </Section>

  <Section
    photo="/photo/webapp.png"
    title="Webapp"
    color="#ffdf00"
    link="//web.dev/progressive-web-apps"
  >
    <p>
      A web application is application software that runs on a web server,
      unlike computer-based software programs that are run locally on the
      operating system of the device, web applications are accessed by the user
      through a web browser with an active network connection.
    </p>
  </Section>

  <div class="space" />
</section>

<Carousel
  title={language.title}
  cover={language.cover}
  items={language.items}
  perpage={3}
/>

<section>
  <div class="space" />
  <Header title="PROJECTS" slogan="A collection of most successful projects" />
  <br /><br />
  <Projects />
</section>

<style>
  .space {
    height: 70px;
  }
</style>
