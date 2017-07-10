<template>

    <div class="tooltip_templates">
      <span id="clear-results">
          Clear Results
      </span>

      <span id="info-scalability">
        <p>
          <span class="criteria-options-meaning">Scalability: </span>Consistency in performance with growing number of requests and application size.
        </p>
        <hr>
        <p>
          <span class="criteria-options-meaning">Very Important: </span>My app is made for masses and will surely grow in size (number of records to be handled). For example: Social network websites.
        </p>
        <p>
          <span class="criteria-options-meaning">Moderately Important: </span>My app is for a large audience but does not need to process big data.
        </p>
        <p>
          <span class="criteria-options-meaning">Not Important: </span>No need for handling large number of records.
        </p>
      </span>

      <span id="info-modularity">
        <p>
          <span class="criteria-options-meaning">Modularity: </span>Support for separation of files / modules responsible for a specific task.
        </p>
        <hr>
        <p>
          <span class="criteria-options-meaning">Very Important: </span>Big website/application with large number of modules/tasks.
        </p>
        <p>
          <span class="criteria-options-meaning">Moderately Important: </span>Not a very large application.
        </p>
        <p>
          <span class="criteria-options-meaning">Not Important: </span>Small application.
        </p>
      </span>

      <span id="info-backwards-compatibility">
        <p>
          <span class="criteria-options-meaning">Backwards Compatibility: </span>Ability to convert code to new version of framework.
        </p>
        <hr>
        <p>
          <span class="criteria-options-meaning">Very Important: </span>Must be able to migrate.
        </p>
        <p>
          <span class="criteria-options-meaning">Moderately Important: </span>Not sure about it.
        </p>
        <p>
          <span class="criteria-options-meaning">Not Important: </span>Do not need any migrations.
        </p>
      </span>

      <span id="info-testability">
        <p>
          <span class="criteria-options-meaning">Testability: </span>Quality of built-in testability.
        </p>
        <hr>
        <p>
          <span class="criteria-options-meaning">Very Important: </span>Requires best available implementation of tests.
        </p>
        <p>
          <span class="criteria-options-meaning">Moderately Important: </span>Framework should provide tests mechanism.
        </p>
        <p>
          <span class="criteria-options-meaning">Not Important: </span>Do not need to write tests.
        </p>
      </span>

      <span id="info-support">
        <p>
          <span class="criteria-options-meaning">Support: </span>Quality of documentation and how much online support is available for troubleshooting.
        </p>
        <hr>
        <p>
          <span class="criteria-options-meaning">Very Important: </span>Must have a huge online community.
        </p>
        <p>
          <span class="criteria-options-meaning">Moderately Important: </span>Should provide some help on develop's networking websites.
        </p>
        <p>
          <span class="criteria-options-meaning">Not Important: </span>Official documentation is enough.
        </p>
      </span>

      <span id="info-future">
        <p>
          <span class="criteria-options-meaning">Future: </span>How long framework will survive in market.
        </p>
        <hr>
        <p>
          <span class="criteria-options-meaning">Very Important: </span>I am sure about my app's long life.
        </p>
        <p>
          <span class="criteria-options-meaning">Moderately Important: </span>Not sure.
        </p>
        <p>
          <span class="criteria-options-meaning">Not Important: </span>I will be able to switch framework if needed.
        </p>
      </span>

      <span id="info-performance">
        <p>
          <span class="criteria-options-meaning">Performance: </span>How fast framework executes user requests.
        </p>
        <hr>
        <p>
          <span class="criteria-options-meaning">Very Important: </span>Fastest possible (large data sets).
        </p>
        <p>
          <span class="criteria-options-meaning">Moderately Important: </span>Should be fast.
        </p>
        <p>
          <span class="criteria-options-meaning">Not Important: </span>Doesn't need to fetch or render a lot of data on page.
        </p>
      </span>

      <span id="info-customizability">
        <p>
          <span class="criteria-options-meaning">Customizability: </span>Support for custom selection of libraries for different components (Model/View/Controller) of application.
        </p>
        <hr>
        <p>
          <span class="criteria-options-meaning">Very Important: </span>I want to be able to choose or change any component anytime.
        </p>
        <p>
          <span class="criteria-options-meaning">Moderately Important: </span>Should be flexible at least in the beginning of project.
        </p>
        <p>
          <span class="criteria-options-meaning">Not Important: </span>I am not so techy. Framework should provide everything.
        </p>
      </span>

      <span id="info-readability">
        <p>
          <span class="criteria-options-meaning">Readability: </span>How natural / human readable is framework's language.
        </p>
        <hr>
        <p>
          <span class="criteria-options-meaning">Very Important: </span>Easiest framework for switching code between developers.
        </p>
        <p>
          <span class="criteria-options-meaning">Moderately Important: </span>Should be fairly easy on eyes.
        </p>
        <p>
          <span class="criteria-options-meaning">Not Important: </span>Complexity doesn't matter.
        </p>
      </span>

      <span id="info-framework-size">
        <p>
          <span class="criteria-options-meaning">Framework Size: </span>Size in KiloBytes which framework will add to project. For example, Angular 2 = 566K.
        </p>
        <hr>
        <p>
          <span class="criteria-options-meaning">Very Important: </span>Must have least possible download time for end user.
        </p>
        <p>
          <span class="criteria-options-meaning">Moderately Important: </span>Should not be the largest.
        </p>
        <p>
          <span class="criteria-options-meaning">Not Important: </span>Doesn't matter.
        </p>
      </span>

      <span id="info-time-in-hand">
        <p>
          <span class="criteria-options-meaning">Time in Hand: </span>Available time for development.
        </p>
        <hr>
        <p>
          <span class="criteria-options-meaning">No Time Constraint: </span>Enough time for team to learn.
        </p>
        <p>
          <span class="criteria-options-meaning">Routine: </span>Can not spend long time to learn.
        </p>
        <p>
          <span class="criteria-options-meaning">Urgent: </span>Absolutely no time to learn.
        </p>
      </span>

      <span id="info-language">
        <p>
          <span class="criteria-options-meaning">Language: </span>Supported  ECMAScript (ES) version or its superset.
        </p>
        <hr>
        <p>
          <span class="criteria-options-meaning">ES6: </span>Do not need TypeScript.
        </p>
        <p>
          <span class="criteria-options-meaning">TypeScript: </span>Requires built in TypeScript compatibility.
        </p>
      </span>

      <span id="info-app-size">
        <p>
          <span class="criteria-options-meaning">App Size: </span>How big do you think your application might become?
        </p>
        <hr>
        <p>
          <span class="criteria-options-meaning">Big: </span>My website will beat facebook.
        </p>
        <p>
          <span class="criteria-options-meaning">Medium: </span>Enterprise level application.
        </p>
        <p>
          <span class="criteria-options-meaning">Small: </span>Personal project.
        </p>
      </span>

      <span id="info-learning-curve">
        <p>
          <span class="criteria-options-meaning">Learning Curve: </span>How long will it take to learn framework.
        </p>
        <hr>
        <p>
          <span class="criteria-options-meaning">Very Important: </span>Must be the easiest one.
        </p>
        <p>
          <span class="criteria-options-meaning">Moderately Important: </span>Should be fairly simple.
        </p>
        <p>
          <span class="criteria-options-meaning">Not Important: </span>Doesn't matter. (smart developers  and time is available)
        </p>
      </span>

      <span id="info-standards-complaint">
        <p>
          <span class="criteria-options-meaning">Standards Complaint: </span>W3C web components support.
        </p>
        <hr>
        <p>
          <span class="criteria-options-meaning">Very Important: </span>Must work without any dependencies or polyfills.
        </p>
        <p>
          <span class="criteria-options-meaning">Moderately Important: </span>Can have polyfills.
        </p>
        <p>
          <span class="criteria-options-meaning">Not Important: </span>No such requirement.
        </p>
      </span>

    </div>

</template>


<script>

  export default {

    name: 'Tooltips-Templates',

    data () {
      return {
      }
    }

  }

</script>




<style>

  .tooltip_templates { display: none; }

  .tooltipster-sidetip.tooltipster-shadow.tooltipster-shadow-customized .tooltipster-content {
    font-family: 'Quicksand', sans-serif;
    letter-spacing: 1px;
    line-height: 1.5em;
  }

  .criteria-options-meaning
  {
    color: black;
    font-style: italic;
  }


</style>
