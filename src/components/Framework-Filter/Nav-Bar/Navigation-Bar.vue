<template>

  <div>

    <Clear-Form-Modal v-bind:clear-form=clearForm></Clear-Form-Modal>
    <Request-Framework-Modal></Request-Framework-Modal>

    <nav class="navbar navbar-default navbar-static-top">
      <div class="container-fluid">
        <div class="navbar-header">
          <a class="navbar-brand" href="#">JavaScript Framework Filter</a>
        </div>
        <div class="" id="bs-example-navbar-collapse-2">
          <ul class="nav navbar-nav navbar-right">
            <li class=""><span class="glyphicon glyphicon-ban-circle hidden-xs clear-data clear-button-disabled tooltips" data-tooltip-content="#clear-results" aria-hidden="true" v-on:click="checkFormStatus()"></span></li>
            <li class="recommend-framework-mobile"><a href="#" data-toggle="modal" data-target="#requestFrameworkFormModal" v-on:click="clearFormOnModalOpen()">Recommend Framework</a></li>
            <li class=""><span class="glyphicon glyphicon-ban-circle hidden-lg hidden-md hidden-sm pull-right clear-data-mobile clear-button-disabled tooltips" data-tooltip-content="#clear-results" aria-hidden="true" v-on:click="checkFormStatus()"></span></li>
          </ul>
        </div>
      </div>
    </nav>

  </div>

</template>


<script>

  import ClearFormModal from './Clear-Form-Modal'
  import RequestFrameworkModal from './Request-Framework-Modal'

    export default {

      name: 'Navigation-Bar',

      props: ['checkFormStatus', 'clearForm'],

        components: {
          ClearFormModal,
          RequestFrameworkModal
      },

      data () {
        return {
        }
    },

    methods:{
          clearFormOnModalOpen: function () {
            for (var i = 0; i < this.$children.length; i++) {
              if (this.$children[i].$options.name == 'Request-Framework-Modal') {
                this.$children[i].clearFormFields();
                break;
              }
            }
          },
    }

  }

</script>




<style>

  .clear-data
  {
  font-size: 20px;
  cursor: pointer;
  color: darkred;
  margin: 15px 25px 0 0;
  border-right: 1px solid lightgrey;
  padding-right: 35px;
  }

  .clear-data-mobile
  {
  font-size: 20px;
  cursor: pointer;
  color: darkred;
  margin: -30px 15px 0 0;
  }

  .clear-button-disabled
  {
  color: lightgrey;
  cursor: default;
  }


  @media screen and (max-width: 767px){

    .recommend-framework-mobile
    {
      width: 70%;
    }

  }

</style>
