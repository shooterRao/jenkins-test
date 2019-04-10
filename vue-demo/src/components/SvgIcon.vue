<template>
  <svg :style="svgColor" fill="currentColor" :class="svgClass" aria-hidden="true">
    <use :xlink:href="iconName"></use>
  </svg>
</template>

<script>
export default {
  name: "SvgIcon",
  props: {
    iconClass: {
      type: String,
      required: true
    },
    className: {
      type: String
    },
    color: {
      type: String
    }
  },
  computed: {
    iconName() {
      return `#${this.iconClass}`;
    },
    svgClass() {
      if (this.className) {
        return `SvgIcon ${this.className}`;
      }
      return "SvgIcon";
    },
    svgColor() {
      if (this.color) {
        return {
          color: this.color
        };
      }
      return "";
    }
  }
};
</script>

<style scoped>
.SvgIcon {
  width: 1em;
  height: 1em;
  vertical-align: -0.15rem;
  fill: currentColor;
  overflow: hidden;
}
</style>
