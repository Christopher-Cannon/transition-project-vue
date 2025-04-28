<script setup>
import PageHeader from './components/PageHeader.vue';
import PageFooter from './components/PageFooter.vue';
import Hero from './components/Hero.vue';
import Main from './components/Main.vue';
import Wrapper from './components/Wrapper.vue';
import NewsItem from './components/NewsItem.vue';
import Newsletter from './components/Newsletter.vue';

const newsItems = [
  {
    image: "/images/underwater-1.jpg",
    heading: "We are Ocean Optimists...",
    description: "Connecting as many people with Ocean as possible, creating accessible and inclusive experiences, and showcasing the sea and all it has to offer.",
    subtitle: "Explore our experience work...",
    arrow: "/images/arrow-right-solid-white.svg",
    inverted: false
  },
  {
    image: "/images/underwater-2.jpg",
    heading: "Protecting Ocean Habitats...",
    description: "Our Ocean Habitats programme aims to protect vital Ocean ecosystems allowing them to regenerate. We are looking to restore them back to full health.",
    subtitle: "Explore our habitats work...",
    arrow: "/images/arrow-right-solid-dark-grey.svg",
    inverted: false
  },
  {
    image: "/images/underwater-3.jpg",
    heading: "A Voice for the Ocean...",
    description: "We're encouraging everyone, from individuals to communities, industry to government, to think about their impact on the Ocean throughout the day and make choices with the health of the Ocean in mind.",
    subtitle: "Explore our advocacy work...",
    arrow: "/images/arrow-right-solid-white.svg",
    inverted: false
  },
];
</script>

<template>
  <PageHeader />

  <Main>
    <Hero />

    <Wrapper>
      <NewsItem
        v-for="(items, index) in newsItems"
        :key="index"
        :items="items"
      />
    </Wrapper>

    <Newsletter />
  </Main>

  <PageFooter />
</template>
