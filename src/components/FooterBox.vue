<template>
  <div class="container">
    <div class="row">
      <section>
        <div class="university" v-for="(item, i) in university" :key="i">
          <h2>{{ item.title }}</h2>
          <span> <i :class="item.icon"></i> {{ item.text }}</span>
        </div>
      </section>
      <section>
        <div class="posts" v-for="(question, x) in post" :key="x">
          <div class="title">
            <h2>{{ question.title }}</h2>
          </div>
          <div class="border-bottom">
            <p>{{ question.testo }}</p>
            <span>{{ question.date }}</span>
          </div>
        </div>
      </section>
      <section class="big">
        <div class="top">
          <div>
            <div class="courses" v-for="(course, k) in courses" :key="k">
              <h2>{{ course.title }}</h2>
              <span>{{ course.text }}</span>
            </div>
          </div>
          <div></div>
          <div
            class="admission"
            v-for="(admission, index) in admissions"
            :key="index"
          >
            <h2>{{ admission.titolo }}</h2>
            <span>{{ admission.texts }}</span>
          </div>
        </div>
        <div class="bottom">
          <div>
            <div
              class="resources"
              v-for="(resource, index) in resources"
              :key="index"
            >
              <h2>{{ resource.title }}</h2>
              <span>{{ resource.text }}</span>
            </div>
          </div>
          <div>
            <div
              class="quick"
              v-for="(quick, index) in quickLinks"
              :key="index"
            >
              <h2>{{ quick.title }}</h2>
              <span>{{ quick.text }}</span>
            </div>
          </div>
        </div>
      </section>
      <section>
        <div class="events">
          <div class="card" v-for="(card, index) in events" :key="index">
            <h2>{{ card.title }}</h2>
            <div class="seminar">
              <div class="number">
                <div class="day">
                  {{ card.day }}
                </div>
                {{ card.num }}
              </div>

              <div class="testo">
                <h4>{{ card.tinyTitle }}</h4>
                <span>{{ card.text }}</span>
                <p>{{ card.place }}</p>
              </div>
            </div>
          </div>
        </div>
        <br />
        View More...
      </section>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      university: [
        {
          title: "AVADA UNIVERSITY",
          icon: "fas fa-home",
          text: "Residential Location 9521 Broadsberry Avenue Paddington RC7 9ZA",
        },
        {
          icon: "fas fa-phone",
          text: "1.800.458.556",
        },
        {
          icon: "fas fa-envelope",
          text: "info@your-domain.com",
        },
        {
          icon: "fas fa-clock",
          text: "Monday - Friday: 8:00 AM - 10:00 PM",
        },
      ],

      post: [
        {
          title: "RECENT POSTS",
          testo: "> What do successful grads think you should study?",
          date: "March 16, 2016",
        },
        {
          testo: "> Former student discuses success in the fashion industry",
          date: "March 15, 2016",
        },
        {
          testo: "> How do you prepare for university?",
          date: "March 15, 2016",
        },
      ],

      courses: [
        {
          title: "COURSES",
          text: "Arts & Humanities",
        },
        {
          text: "Business & Management",
        },
        {
          text: "Engineering & Technology",
        },
        {
          text: "Life Sciences & Medicine",
        },
        {
          text: "Natural sciences",
        },
      ],
      admissions: [
        {
          titolo: "ADMISSIONS",
          texts: "Eligibility",
        },
        {
          texts: "Application",
        },
        {
          texts: "Review Process",
        },
        {
          texts: "How to Apply",
        },
      ],
      resources: [
        {
          title: "RESOURCES",
          text: "Campus Directory",
        },
        {
          text: "Academic Calendar",
        },
        {
          text: "Sport Clubs",
        },
        {
          text: "Graduate Programs",
        },
        {
          text: "Faculty & Staff",
        },
      ],
      quickLinks: [
        {
          title: "QUICKLINKS",
          text: "University Library",
        },
        {
          text: "Campus Services",
        },
        {
          text: "Careers",
        },
      ],
      events: [
        {
          title: "UPCOMING EVENTS",
          tinyTitle: "Business Seminar",
          text: "July 1, 2019 @ 8:00 am - July 1, 2021 @ 5:00 pm",
          place: "United States",
          day: "FRI",
          num: "27",
        },
        {
          tinyTitle: "Politics Seminar",
          text: "November 6, 2019 @ 8:00 am - November 6, 2021 @ 5:00 pm",
          place: "United Kingdom",
          day: "FRI",
          num: "27",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/FooterBox.scss";
</style>