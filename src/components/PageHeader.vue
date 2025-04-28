<script setup>
import NavLink from './NavLink.vue';
</script>

<template>
  <header class="page-header">
    <div class="page-wrapper">
      <h1 class="page-title">Ocean Conservation Trust</h1>

      <nav>
        <ul class="nav-list">
          <NavLink text="About Us" link="#" />
          <NavLink text="Experiences" link="#" />
          <NavLink text="Advocacy" link="#" />
          <NavLink text="Habitats" link="#" />
          <NavLink text="Donate" link="#" isButton="true" />
        </ul>
      </nav>
    </div>
  </header>
</template>