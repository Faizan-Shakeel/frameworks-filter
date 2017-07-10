<template>

  <!-- Modal Clear Form Confirmation -->
  <div class="modal fade" id="clearFormConfirmationModal" tabindex="-1" role="dialog" aria-labelledby="requestFrameworkFormModalLabel" data-backdrop="static" aria-hidden="true">
    <div class="modal-dialog modal-sm" role="document">
      <div class="modal-content">
        <div class="modal-header">
          <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
          <h4 class="modal-title text-center" id="requestFrameworkFormModalLabel2">Clear Form</h4>
        </div>
        <div class="modal-body">
          <p>Are you sure you want to clear the form?</p>
        </div>
        <div class="modal-footer">
          <button type="button" class="btn btn-default" data-dismiss="modal">Close</button>
          <button type="button" class="btn btn-success" v-on:click="clearForm(0)">Clear Form</button>
        </div>
      </div>
    </div>
  </div>

</template>


<script>

  export default {

    name: 'Clear-Form-Modal',

    props: ['clearForm'],

    data () {
      return {
      }
    },

    methods:{}

  }

</script>




<style>



</style>
