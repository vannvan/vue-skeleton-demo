<template>
    <div class="skeleton-wrapper">
          <div class="header"></div>
          <div class="content">
            <div class="content-left"></div>
            <div class="content-right"></div>
          </div>
    </div>
</template>

<script>
export default {
    name: 'skeleton'
};
</script>

<style lang="scss">
.skeleton-wrapper {
      height: 100%;
      background: #fff;
    .header{
      height: 80px;
      width: 100%;
      background: #f6f6f6;
    }
    .content{
      width: 100%;
      background: #fff;
      display: table;
      height: calc(100vh - 80px);
      border-spacing:0 30px;
      .content-left{
        display: table-cell;
        width: 20%;
        height: 100%;
        border-right:30px #fff solid;
        background: #f6f6f6;
      }
      .content-right{
        display: table-cell;
        width: 80%;
        background: #f6f6f6;
      }
    }

}
</style>
