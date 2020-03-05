<template>
  <div class="wrapper">
    <header class="container-fluid">
      <h1 class="text-center">vue-skeleton-layout</h1>
    </header>

    <main class="container-fluid">
      <h2 class="h4">Generic placeholder</h2>

      <div class="skeleton-item">
        <div class="skeleton-col-12">
          <div class="skeleton-picture"></div>
          <div class="skeleton-row">
            <div class="skeleton-col-6 big"></div>
            <div class="skeleton-col-4 empty big"></div>
            <div class="skeleton-col-2 big"></div>
            <div class="skeleton-col-4"></div>
            <div class="skeleton-col-8 empty"></div>
            <div class="skeleton-col-6"></div>
            <div class="skeleton-col-6 empty"></div>
            <div class="skeleton-col-12"></div>
          </div>
        </div>
      </div>

      <h2 class="h4">Placeholder in a external twitter bootstrap grid</h2>

      <div class="row">
        <div class="col-12 col-sm-6">
          <div class="skeleton-item">
            <div class="skeleton-col-12">
              <div class="skeleton-picture"></div>
              <div class="skeleton-row">
                <div class="skeleton-col-4"></div>
                <div class="skeleton-col-8 empty"></div>
                <div class="skeleton-col-12"></div>
              </div>
            </div>
            <div class="skeleton-col-2">
              <div class="skeleton-avatar"></div>
            </div>
            <div>
              <div class="skeleton-row">
                <div class="skeleton-col-12"></div>
                <div class="skeleton-col-2"></div>
                <div class="skeleton-col-10 empty"></div>
                <div class="skeleton-col-8 big"></div>
                <div class="skeleton-col-4 big empty"></div>
              </div>
            </div>
          </div>
        </div>

        <div class="col-12 col-sm-6">
          <div class="skeleton-item">
            <div class="skeleton-col-12">
              <div class="skeleton-picture"></div>
              <div class="skeleton-row">
                <div class="skeleton-col-4"></div>
                <div class="skeleton-col-8 empty"></div>
                <div class="skeleton-col-12"></div>
              </div>
            </div>
            <div class="skeleton-col-2">
              <div class="skeleton-avatar"></div>
            </div>
            <div>
              <div class="skeleton-row">
                <div class="skeleton-col-12"></div>
                <div class="skeleton-col-2"></div>
                <div class="skeleton-col-10 empty"></div>
                <div class="skeleton-col-8 big"></div>
                <div class="skeleton-col-4 big empty"></div>
              </div>
            </div>
          </div>
        </div>
      </div>

      <h2 class="h4">Other placeholder examples</h2>

      <div class="skeleton-item">
        <div class="skeleton-col-12">
          <div class="skeleton-picture"></div>
        </div>

        <div class="skeleton-col-2">
          <div class="skeleton-avatar"></div>
        </div>

        <div>
          <div class="skeleton-row">
            <div class="skeleton-col-4"></div>
            <div class="skeleton-col-8 empty"></div>
            <div class="skeleton-col-6"></div>
            <div class="skeleton-col-6 empty"></div>
            <div class="skeleton-col-2"></div>
            <div class="skeleton-col-10 empty"></div>
          </div>
        </div>

        <div class="skeleton-col-12">
          <div class="skeleton-row">
            <div class="skeleton-col-10 big"></div>
            <div class="skeleton-col-2 empty big"></div>
            <div class="skeleton-col-4"></div>
            <div class="skeleton-col-8 empty"></div>
            <div class="skeleton-col-6"></div>
            <div class="skeleton-col-6 empty"></div>
            <div class="skeleton-col-12"></div>
          </div>
        </div>
      </div>

      <div class="skeleton-item">
        <div class="skeleton-col-2">
          <div class="skeleton-avatar"></div>
        </div>

        <div>
          <div class="skeleton-row">
            <div class="skeleton-col-4"></div>
            <div class="skeleton-col-8 empty"></div>
            <div class="skeleton-col-6"></div>
            <div class="skeleton-col-6 empty"></div>
            <div class="skeleton-col-2"></div>
            <div class="skeleton-col-10 empty"></div>
          </div>
        </div>

        <div class="skeleton-col-12">
          <div class="skeleton-picture"></div>
          <div class="skeleton-row">
            <div class="skeleton-col-10 big"></div>
            <div class="skeleton-col-2 empty big"></div>
            <div class="skeleton-col-4"></div>
            <div class="skeleton-col-8 empty"></div>
            <div class="skeleton-col-6"></div>
            <div class="skeleton-col-6 empty"></div>
            <div class="skeleton-col-12"></div>
          </div>
        </div>

        <div class="skeleton-col-4">
          <div class="skeleton-picture"></div>
        </div>

        <div>
          <div class="skeleton-row">
            <div class="skeleton-col-6"></div>
            <div class="skeleton-col-6 empty"></div>
            <div class="skeleton-col-2"></div>
            <div class="skeleton-col-10 empty"></div>
            <div class="skeleton-col-8"></div>
            <div class="skeleton-col-4 empty"></div>
            <div class="skeleton-col-12"></div>
          </div>
        </div>
      </div>

      <div class="skeleton-item">
        <div class="skeleton-col-2">
          <div class="skeleton-avatar"></div>
        </div>

        <div>
          <div class="skeleton-row">
            <div class="skeleton-col-4"></div>
            <div class="skeleton-col-8 empty"></div>
            <div class="skeleton-col-6"></div>
            <div class="skeleton-col-6 empty"></div>
            <div class="skeleton-col-2"></div>
            <div class="skeleton-col-10 empty"></div>
          </div>
        </div>

        <div class="skeleton-col-12">
          <div class="skeleton-picture"></div>
          <div class="skeleton-row">
            <div class="skeleton-col-10 big"></div>
            <div class="skeleton-col-2 empty big"></div>
            <div class="skeleton-col-4"></div>
            <div class="skeleton-col-8 empty"></div>
            <div class="skeleton-col-6"></div>
            <div class="skeleton-col-6 empty"></div>
            <div class="skeleton-col-12"></div>
          </div>
        </div>
      </div>
    </main>

    <div class="content">
      <skeleton-layout>
        <skeleton-ticket-item
          v-for="skeleton in 15"
          :key="skeleton"
        />
      </skeleton-layout>
    </div>
  </div>
</template>

<script>
import SkeletonLayout, {
  SkeletonTicketItem,
} from './components/SkeletonLayout/index.vue';

export default {
  name: 'App',

  components: {
    SkeletonLayout,
    SkeletonTicketItem,
  },
};
</script>

<style lang="scss">
  @import "./assets/styles/index";

  body {
    background-color: #e9ecef;
    font-family: 'Arial', sans-serif;
    font-size: 14px;
    line-height: 1;
  }

  header,
  footer {
    padding: 20px 0;
  }

  .text-center {
    text-align: center;
  }

  .container-fluid {
    max-width: 600px;
    margin-left: auto;
    margin-right: auto;
  }
</style>
