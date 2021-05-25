<template>
  <div class="col-md-4 testimony">
    <div class="row">
        <div class="col-1">
            <img :src="'/images/blockquote.svg'" alt="blockquote">
        </div>
        <div class="col-9 testimony-content">
            <div class="testimony-text">
                {{ text }}
            </div>
            <div class="testimony-user">
                {{ name }}
            </div>
            <div class="testimony-user-role">
                {{ role }}
            </div>
        </div>
    </div>
  </div>
</template>

<script>
  export default {
      props: ['text', 'name', 'role']
  }
</script>

<style>
    .testimony{
        color: var(--white);
    }
    .testimony-content{
        padding: 20px !important;
    }
    .testimony-text{
        font-size: 16px;
        font-weight: 300;
        margin-bottom: 20px;
        font-weight: lighter;
    }
    .testimony-user{
        font-size: 13px;
        font-weight: 700;
        margin-bottom: 5px;
    }
    .testimony-user-role{
        font-size: 13px;
        font-weight: lighter;
        margin-bottom: 5px;
        color: #B8B8B8;
    }
    @media screen and (max-width: 500px) {
        .testimony{
            margin-bottom: 20px;
            border-bottom: 1px solid rgba(204, 204, 204, 0.2);
            padding: 0 0 30px 0 !important;
        }
        .testimony:last-child{
            border-bottom: none;
        }
    }
</style>