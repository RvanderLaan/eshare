<template>
  <div class="impact">
    <span class="title">Impact</span>
    <span class="sub-title">See your impact in numbers</span>
    <div class="impact-grid">
      <div class="impact-number">
        <div class="impact-wrapper">
          <span class="large-value">2</span>
          <span class="label">Consumers</span>
        </div>
      </div>
      <div class="impact-number">
        <div class="impact-wrapper">
          <span class="large-value">160</span>
          <span class="small-label">kWh</span>
          <span class="label">Donated</span>
        </div>
      </div>
      <div class="impact-number">
        <div class="impact-wrapper">
          <span class="large-value">540</span>
          <span class="small-label">hours</span>
          <span class="label">Sun hours</span>
        </div>
      </div>
      <div class="impact-number">
        <div class="impact-wrapper">
          <span class="large-value">310</span>
          <span class="small-label">kWh</span>
          <span class="label">Consumed</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Impact',
  props: {
  }
}
</script>

<style scoped lang="scss">
@import "../global.scss";

.impact {
  background: transparent;
  box-shadow: none;
  display: flex;
  flex-direction: column;

  .impact-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-gap: 5px;

    .impact-number {
      background: #00ffcc;
      box-shadow: 0 2px 12px -5px #00e7b8;
      border-radius: 5px;
      padding: 30px;
      transition: all 0.2s ease;

      .impact-wrapper {
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        height: 100%;

        .large-value {
          font-size: 1.8em;
          color: white;
          font-weight: 500;
        }

        .label {
          font-weight: 700;
          font-size: 0.8em;
          color: white;
          margin-top: 5px;
        }

        .small-label {
          font-weight: 500;
          font-size: 0.8em;
          color: white;
          margin-top: 5px;
          opacity: 0.9;
        }
      }
    }

    .impact-number:hover {
      background-color: $primary-dark;
    }
  }
}
</style>
