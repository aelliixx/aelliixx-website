<script setup lang="ts">
import ProjectCard from "../components/ProjectCard.vue";
import Testimony from "@/components/Testimony.vue";
</script>

<template>
  <main>
    <section class="hero">
      <div class="title">
        <p>Hey! My name is</p>
        <h1>Donatas Mockus</h1>
        <p>Full-stack Web Developer \\ Software Engineer \\ Game Developer</p>
      </div>
    </section>
    <section id="experience">
      <h2>experience.</h2>
      <div class="experience-container">
        <div>
          <h3 class="underline-blue">software engineering</h3>
          <div class="card">
            <p>
              Experienced in developing highly scalable and robust desktop applications and embedded
              software.
            </p>
            <div class="tools">
              <h4>Languages</h4>
              <p>C++, C#, Rust, Python, Java</p>
            </div>
          </div>
        </div>
        <div>
          <h3 class="underline-red">web development</h3>
          <p>
            Passionate about beautiful and accessible websites. I'm highly experienced in web design
            for both small and enterprise scale websites, writing supporting back-end APIs,
            deployment, and on-going support.
          </p>
          <div class="tools">
            <h4>Languages & frameworks</h4>
            <p>Typescript, HTML, CSS, React, NextJS, Vue</p>
            <h4>Back-end tech & databases</h4>
            <p>Node, Python, MySql, ProstgreSQL, Redis, DynamoDB</p>
            <h4>Devops</h4>
            <p>AWS, Azure, Google Cloud, Vercel, Heroku</p>
          </div>
        </div>
        <div>
          <h3 class="underline-green">game development</h3>
          <p>
            Unreal Engine 5 and Unity generalist. I have worked on and shipped more than 6 titles
            both at indie studios and with individual clients. I specialise in gameplay development
            and level design.
          </p>
          <div class="tools">
            <h4>Engines & languages</h4>
            <p>Unreal Engine 4 and 5, Unity, C++, C#</p>
          </div>
        </div>
      </div>
    </section>
    <section id="projects">
      <h2>projects.</h2>
      <p>
        Unfortunately most of my projects are covered by an NDA and so I can't share them, but
        here's a small handful that I can!
      </p>
      <div class="projects-container">
        <div>
          <h3 class="underline-red">web</h3>
          <div class="card-container">
            <ProjectCard
              style="grid-row: span 1; grid-column: span 2"
              image-url="/uedocs_website.png"
              title="UE Docs"
              tech="NextJS, Typescript, Contentlayer"
            >
              <p>
                After working with Unreal Engine for over 5 years, I became frustrated with the poor
                quality of the official documentation, so I decided to create my own open sourced
                documentation for it. Anyone with some knowledge of markdown and who wishes to
                contribute can submit documentation.
              </p>
            </ProjectCard>
            <ProjectCard
              style="grid-column: span 4"
              image-url="/allographic_website.png"
              title="allographic.io"
              link="https://allographic.io"
              tech="NextJS, Typescript, Auth.js, PostgreSQL"
            >
              <p>
                In late 2022, I along with a business partner started a tech consultancy firm. We
                specialise in software development, and full-stack web application development and
                support.
              </p>
              <p>
                The website, beyond the everyday user facing side, offers a fully featured dashboard
                for tracking projects, invoices, quotes, and business metrics.
              </p>
            </ProjectCard>
            <ProjectCard
              title="Searchify"
              style="grid-row: span 2"
              tech="NextJS, Spotify API, Rust"
            >
              <p>
                A small website I made for parsing through a user's Spotify playlists and allowing
                them to search for songs by their lyrics.
              </p>
            </ProjectCard>
            <ProjectCard
              style="grid-column: span 4"
              title="Virtuverse.io"
              image-url="/virtuverse_website.png"
              link="https://virtuverse.io"
              tech="Vue"
            >
              <p>
                I have worked at Virtuverse as a game developer for over four years now. I also
                contributed to the development of the website
              </p>
            </ProjectCard>
          </div>
        </div>

        <div>
          <h3 class="underline-green">games</h3>
          <div class="card-container">
            <ProjectCard
              style="grid-column: span 3"
              title="Virtuverse"
              link="https://virtuverse.io"
              image-url="/virtuverse_game.png"
              tech="Unreal Engine 5, C++"
            >
              <p>
                Virtuverse is an RCE MMO-RPG set in a virtual world. A sort of sandbox-on-rails,
                Virtuverse allows players to specialise in different professions: crafting, mining,
                hunting, and many more; go on quests, ally or fight different factions, and explore
                the large and open worlds.
              </p>
              <p>
                I have worked on Virtuverse for more than four years along with a team of extremely
                talented developers and artists. Over the course of these four years, we have
                shipped more than 6 major updates and are currently working on the 7th, which is a
                complete rewrite in Unreal Engine 5.
              </p>
            </ProjectCard>
            <ProjectCard
              style="grid-row: span 1; grid-column: span 3"
              title="Terraforma"
              tech="Unity 2D, C#"
            >
              <p>
                Terraforma is a 2D, hex-tile based game where the player controls an intricate
                network of plant roots and must restore the soil's thriving ecosystem. The game
                explores the nuances of soil science and underlines the importance of taking care of
                our planet and the environment.
              </p>
            </ProjectCard>
            <ProjectCard
              style="grid-row: span 1; grid-column: span 3"
              title="No Man's North"
              link="https://nomansnorth.com"
              image-url="/nmn_game.png"
              tech="Unity 3D, C#"
            >
              <p>
                No Man's North explores the saga of James Heresy, an average man living in British
                Columbia who finds himself in the midst of the next ice-age. Accompanied only by his
                dog Monty, he must survive the harsh wilderness before the oncoming storm makes him
                perish.
              </p>
            </ProjectCard>
          </div>
        </div>
      </div>
    </section>
    <section id="work">
      <h2>work.</h2>
      <div class="table">
        <div class="row header">
          <i>Date</i>
          <i>Position</i>
          <i>Description</i>
        </div>
        <div class="row">
          <p>Dec. 2022 - Present</p>
          <p>Director, MB Allographic</p>
          <p>
            Allographic is a company I co-founded which focuses on B2B software consulting and
            enterprise software development. Personally I am focused on the technology side of the
            business where I maintain our backend infrastructure and develop enterprise software for
            business and project management.
          </p>
        </div>
        <div class="row">
          <p>Jun. 2022 - Present</p>
          <p>Software Engineering Consultant, Magna Ludum Creative</p>
          <p>
            I have worked with a number of clients on a variety of games, be it mobile, desktop,
            using Unity or Unreal, 2D, 3D, multiplayer or otherwise. My contributions to these
            projects include feature design and development, bug fixing, and QA. I work extremely
            closely with the individual clients to ensure I can deliver exactly what they have
            imagined on time and on budget.
          </p>
        </div>
        <div class="row">
          <p>May 2020 - Present</p>
          <p>Lead World Designer, Virtuverse A.B.</p>
          <p>
            In mid-2020 I took the lead responsibility of world level design, with primary
            responsibilities of natural and urban open world design. This, in combination with my
            experience in programming, allowed me to create dynamic, and in places procedural, maps
            that adapt to player’s behaviour.
          </p>
        </div>
        <div class="row">
          <p>Feb. 2019 - Present</p>
          <p>Senior Developer, Virtuverse A.B.</p>
          <p>
            Over the more than four years as a developer at Virtuverse, I helped build a
            massively-multiplayer role-playing game. With such a task come huge challenges, and
            together with my team, we faced them head on by implementing a robust network
            architecture to facilitate thousands of users joining at once, designing a flexible user
            interface, and creating expansive and performant world maps.
          </p>
        </div>
      </div>
    </section>
    <section id="testimony">
      <h2>testimonies.</h2>
      <Testimony name="Sam" image-url="https://cdn.discordapp.com/avatars/965958179437576202/1b768414d38e7a2fecd1aac77f636d76.webp?size=128"
                 source="Lead Producer at Mindflair Games">
        Donatas is a talented developer who comprehends assigned tasks. He willingly offers suggestions and technical assistance to ensure well-executed features. He's efficient and organized in his coding work.
      </Testimony>
    </section>
    <section id="contact">
      <h2>contact.</h2>
      <div class="contact">
        <p style="max-width: 70ch">
          Need my expertise? Whether it's designing a website, creating enterprise applications, or
          developing your next game title, I have the experience to bring your project from start to
          finish.
        </p>
        <p>You can reach out to me by email:</p>
        <a href="mailto:donatas@allographic.io" class="underline-blue email link-subdued"
        >donatas@allographic.io</a
        >
        <p style="margin-block-start: 1rem; margin-block-end: 0.25rem">
          Or find me on these platforms:
        </p>
        <a href="https://github.com/aelliixx" class="underline-red">github.</a>
        <a href="https://www.linkedin.com/in/donatas-mockus-a62945162/" class="underline-blue"
        >linkedin.</a
        >
      </div>
    </section>
  </main>
</template>

<style scoped lang="scss">
.hero {
  display: grid;
  grid-template-columns: 1fr 1fr;
  place-items: center;
  height: 80dvh;

  .title {
    line-height: 1;

    h1 {
      font-size: 3em;
      font-weight: 500;
    }
  }
}

section:not(:first-of-type) {
  margin-block: 10rem;
}

.experience-container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 3rem;
  margin-block-start: 1rem;

  h3 {
    margin-block-end: 1rem;
  }

  .tools {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-block-start: 0.5rem;

    p, h4 {
      margin-block-start: 1rem;
      text-align: center;
    }
  }
}

.projects-container {
  display: grid;
  gap: 3rem;
  margin-block-start: 1rem;

  .card-container {
    display: grid;
    grid-template-columns: repeat(6, 1fr);
    gap: 2rem;
    margin-block: 1rem;
  }
}

.table {
  margin-block: 1rem;

  .row {
    display: grid;
    grid-template-columns: 0.25fr 0.5fr 1fr;
    grid-column-gap: 0.5rem;
    padding-block: 0.75rem;
    border-bottom: 1px dashed var(--clr-fg);

    p {
      margin: 0;
    }
  }

  .header,
  .row:last-of-type {
    border-bottom: 2px solid var(--clr-fg);
  }
}

.contact {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;

  .email {
    text-decoration-line: underline;
    text-decoration-thickness: 0.25rem;
    font-size: 1.75rem;
  }
}

@media (max-width: 622px) {
  .experience-container {
    grid-template-columns: 1fr;
  }

  .projects-container {
    .card-container {
      grid-template-columns: 1fr;

      > * {
        grid-column: span 1 !important;
        grid-row: span 1 !important;
      }
    }
  }
}

@media (max-width: 425px) {
  .table {
    .row {
      grid-template-columns: 1fr;
      gap: 0.75rem;
      &:first-of-type {
        display: none;
      }

      p:nth-of-type(1), p:nth-of-type(2) {
        font-weight: 700;
      }
    }
  }

  .email {
    font-size: 1rem !important;
  }
}
</style>
