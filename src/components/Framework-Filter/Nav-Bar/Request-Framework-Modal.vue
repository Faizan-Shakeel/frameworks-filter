<template>

  <div class="modal fade" id="requestFrameworkFormModal" tabindex="-1" role="dialog" aria-labelledby="requestFrameworkFormModalLabel" data-backdrop="static" aria-hidden="true">
    <div class="modal-dialog" role="document">
      <div class="modal-content">
        <div class="modal-header">
          <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
          <h4 class="modal-title text-center" id="requestFrameworkFormModalLabel">Recommend Framework for Comparison</h4>
        </div>
        <form action="https://formspree.io/faizan.sg@gmail.com" method="post">
          <div class="modal-body">
            <div class="form-group">
              <label for="frameworkName">Framework Name</label>
              <input v-model="recommendedFrameworkByUser" type="text" class="form-control" id="frameworkName" placeholder="Framework Name" name="Framework Name" required>
            </div>
            <div class="form-group">
              <label for="optionalMessage">Message <span class="optional-message">(Optional)</span></label>
              <textarea v-model="emailFormOptionalMessage" class="form-control" rows="3" id="optionalMessage" placeholder="Message" name="Message"></textarea>
            </div>
          </div>
          <div class="modal-footer">
            <button type="button" class="btn btn-default" data-dismiss="modal">Close</button>
            <button type="button" class="btn btn-success" v-on:click="sendMail(recommendedFrameworkByUser, emailFormOptionalMessage)">Submit Recommendation</button>
          </div>
        </form>
      </div>
    </div>
  </div>

</template>


<script>

  export default {

    name: 'Request-Framework-Modal',

    data () {
      return {
        recommendedFrameworkByUser: '',
        emailFormOptionalMessage: ''
      }
    },

    methods:{
      clearFormFields: function () {
        this.recommendedFrameworkByUser = '';
        this.emailFormOptionalMessage = '';
      },

      sendMail: function (recommendedFrameworkByUser, optionalMessage)
      {
        if($('#frameworkName')[0].checkValidity())
        {
          $.ajax({
            url: "https://formspree.io/faizan.sg@gmail.com",
            method: "POST",
            data:
              {
                'Recommended Framework': recommendedFrameworkByUser,
                'Message': optionalMessage,
                _subject: recommendedFrameworkByUser
              },
            dataType: "json"
          });

          $("#requestFrameworkFormModal").modal('hide');
          toastr.success('Thank you for the recommendation.', 'Email Sent', {timeOut: 3000});
        }
        else
        {
          toastr.warning('Please provide a framework name.', 'Required', {timeOut: 3000});
        }
      },
    }
  }

</script>




<style>

  .optional-message
  {
    font-size: smaller;
    font-weight: lighter;
    font-style: italic;
  }


</style>
