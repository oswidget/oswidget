<template>
  <a href="https://github.com/oswidget/oswidget" target="_blank" class="logo">
    <b>OS</b>widget
  </a>
</template>

<script>
export default {
  name: 'Logo',
};
</script>

<style lang="scss">
.logo {
  position: absolute;
  bottom: 30px;
  left: 30px;
  font-size: 25px;
  line-height: 30px;
  color: #D6D6D6;
  font-weight: 500;
  z-index: $logoIndex-desktop;
  transition: all .3s;
  cursor: pointer;
  text-decoration: none;

  &:hover {
    color: $gray;
  }

  @include for-tablet {
    bottom: $m-tablet;
    left: $m-tablet;
  }

  @include for-phone {
    left: 0;
    right: 0;
    text-align: center;
    z-index: $logoIndex-phone;
  }
}
</style>
