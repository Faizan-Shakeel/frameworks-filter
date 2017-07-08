<template>

  <div class="filter-container">

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

    <nav class="navbar navbar-default navbar-static-top">
      <div class="container-fluid">
        <div class="navbar-header">
          <a class="navbar-brand" href="#">JavaScript Framework Filter</a>
        </div>
        <div class="" id="bs-example-navbar-collapse-2">
          <ul class="nav navbar-nav navbar-right">
            <li class=""><span class="glyphicon glyphicon-ban-circle hidden-xs clear-data clear-button-disabled tooltips" data-tooltip-content="#clear-results" aria-hidden="true" v-on:click="checkFormStatus()"></span></li>
            <li class="recommend-framework-mobile"><a href="#" data-toggle="modal" data-target="#requestFrameworkFormModal">Recommend Framework</a></li>
            <li class=""><span class="glyphicon glyphicon-ban-circle hidden-lg hidden-md hidden-sm pull-right clear-data-mobile clear-button-disabled tooltips" data-tooltip-content="#clear-results" aria-hidden="true" v-on:click="checkFormStatus()"></span></li>
          </ul>
        </div>
      </div>
    </nav>

    <!-- Modal -->
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
              <button type="button" class="btn btn-default" data-dismiss="modal" v-on:click="clearFormFields()">Close</button>
              <button type="button" class="btn btn-success" v-on:click="sendMail(recommendedFrameworkByUser, emailFormOptionalMessage)">Submit Recommendation</button>
            </div>
          </form>
        </div>
      </div>
    </div>


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

    <div class="row whole-page">

      <div class="floating-form">
        <a class="contact-opener" href="https://goo.gl/forms/6sakUAormUq3IkU43" target="_blank">Feedback</a>
      </div>

      <div class="col-sm-6 col-md-6 col-lg-6">

        <form class="form-horizontal">
          <div class="form-group">
            <label class="col-xs-5 col-sm-5 col-md-5 col-lg-3 control-label" for="scalability">Scalability</label>
            <div class="col-xs-6 col-sm-6 col-md-6 col-lg-8">
              <!--<select v-model="scalability" class="form-control" id="scalability" v-on:change="frameworkFilter('scalability', scalability)">-->
              <select v-model="scalability" id="scalability" class="form-control" v-on:change="frameworkFilter('scalability', scalability)">
                <option class="testing-options-text-color" disabled value="">Select...</option>
                <option>Very Important</option>
                <option>Moderately Important</option>
                <option>Not Important</option>
              </select>
            </div>
            <span class="col-xs-1 col-sm-1 col-md-1 col-lg-1 glyphicon glyphicon-info-sign criteria-description-in-tooltip tooltips" data-tooltip-content="#info-scalability"></span>
          </div>
          <div class="form-group">
            <label class="col-xs-5 col-sm-5 col-md-5 col-lg-3 control-label" for="modularity">Modularity</label>
            <div class="col-xs-6 col-sm-6 col-md-6 col-lg-8">
              <select v-model="modularity" class="form-control" id="modularity" v-on:change="frameworkFilter('modularity', modularity)">
                <option disabled value="">Select...</option>
                <option>Very Important</option>
                <option>Moderately Important</option>
                <option>Not Important</option>
              </select>
            </div>
            <span class="col-xs-1 col-sm-1 col-md-1 col-lg-1 glyphicon glyphicon-info-sign criteria-description-in-tooltip tooltips" data-tooltip-content="#info-modularity"></span>
          </div>
          <div class="form-group">
            <label class="col-xs-5 col-sm-5 col-md-5 col-lg-3 control-label" for="backwardscompatibility">Backwards Compatibility</label>
            <div class="col-xs-6 col-sm-6 col-md-6 col-lg-8">
              <select v-model="backwardsCompatibility" class="form-control" id="backwardscompatibility" v-on:change="frameworkFilter('backwardsCompatibility', backwardsCompatibility)">
                <option disabled value="">Select...</option>
                <option>Very Important</option>
                <option>Moderately Important</option>
                <option>Not Important</option>
              </select>
            </div>
            <span class="col-xs-1 col-sm-1 col-md-1 col-lg-1 glyphicon glyphicon-info-sign criteria-description-in-tooltip tooltips" data-tooltip-content="#info-backwards-compatibility"></span>
          </div>
          <div class="form-group">
            <label class="col-xs-5 col-sm-5 col-md-5 col-lg-3 control-label" for="testability">Testability</label>
            <div class="col-xs-6 col-sm-6 col-md-6 col-lg-8">
              <select v-model="testability" class="form-control" id="testability" v-on:change="frameworkFilter('testability', testability)">
                <option disabled value="">Select...</option>
                <option>Very Important</option>
                <option>Moderately Important</option>
                <option>Not Important</option>
              </select>
            </div>
            <span class="col-xs-1 col-sm-1 col-md-1 col-lg-1 glyphicon glyphicon-info-sign criteria-description-in-tooltip tooltips" data-tooltip-content="#info-testability"></span>
          </div>
          <div class="form-group">
            <label class="col-xs-5 col-sm-5 col-md-5 col-lg-3 control-label" for="support">Support</label>
            <div class="col-xs-6 col-sm-6 col-md-6 col-lg-8">
              <select v-model="support" class="form-control" id="support" v-on:change="frameworkFilter('support', support)">
                <option disabled value="">Select...</option>
                <option>Very Important</option>
                <option>Moderately Important</option>
                <option>Not Important</option>
              </select>
            </div>
            <span class="col-xs-1 col-sm-1 col-md-1 col-lg-1 glyphicon glyphicon-info-sign criteria-description-in-tooltip tooltips" data-tooltip-content="#info-support"></span>
          </div>
          <div class="form-group">
            <label class="col-xs-5 col-sm-5 col-md-5 col-lg-3 control-label" for="future">Future</label>
            <div class="col-xs-6 col-sm-6 col-md-6 col-lg-8">
              <select v-model="future" class="form-control" id="future" v-on:change="frameworkFilter('future', future)">
                <option disabled value="">Select...</option>
                <option>Very Important</option>
                <option>Moderately Important</option>
                <option>Not Important</option>
              </select>
            </div>
            <span class="col-xs-1 col-sm-1 col-md-1 col-lg-1 glyphicon glyphicon-info-sign criteria-description-in-tooltip tooltips" data-tooltip-content="#info-future"></span>
          </div>
          <div class="form-group">
            <label class="col-xs-5 col-sm-5 col-md-5 col-lg-3 control-label" for="performance">Performance</label>
            <div class="col-xs-6 col-sm-6 col-md-6 col-lg-8">
              <select v-model="performance" class="form-control" id="performance" v-on:change="frameworkFilter('performance', performance)">
                <option disabled value="">Select...</option>
                <option>Very Important</option>
                <option>Moderately Important</option>
                <option>Not Important</option>
              </select>
            </div>
            <span class="col-xs-1 col-sm-1 col-md-1 col-lg-1 glyphicon glyphicon-info-sign criteria-description-in-tooltip tooltips" data-tooltip-content="#info-performance"></span>
          </div>
          <div class="form-group">
            <label class="col-xs-5 col-sm-5 col-md-5 col-lg-3 control-label" for="customizability">Customizability</label>
            <div class="col-xs-6 col-sm-6 col-md-6 col-lg-8">
              <select v-model="customizability" class="form-control" id="customizability" v-on:change="frameworkFilter('customizability', customizability)">
                <option disabled value="">Select...</option>
                <option>Very Important</option>
                <option>Moderately Important</option>
                <option>Not Important</option>
              </select>
            </div>
            <span class="col-xs-1 col-sm-1 col-md-1 col-lg-1 glyphicon glyphicon-info-sign criteria-description-in-tooltip tooltips" data-tooltip-content="#info-customizability"></span>
          </div>
          <div class="form-group">
            <label class="col-xs-5 col-sm-5 col-md-5 col-lg-3 control-label" for="readability">Readability</label>
            <div class="col-xs-6 col-sm-6 col-md-6 col-lg-8">
              <select v-model="readability" class="form-control" id="readability" v-on:change="frameworkFilter('readability', readability)">
                <option disabled value="">Select...</option>
                <option>Very Important</option>
                <option>Moderately Important</option>
                <option>Not Important</option>
              </select>
            </div>
            <span class="col-xs-1 col-sm-1 col-md-1 col-lg-1 glyphicon glyphicon-info-sign criteria-description-in-tooltip tooltips" data-tooltip-content="#info-readability"></span>
          </div>
          <div class="form-group">
            <label class="col-xs-5 col-sm-5 col-md-5 col-lg-3 control-label" for="frameworkSize">Framework Size</label>
            <div class="col-xs-6 col-sm-6 col-md-6 col-lg-8">
              <select v-model="frameworkSize" class="form-control" id="frameworkSize" v-on:change="frameworkFilter('frameworkSize', frameworkSize)">
                <option disabled value="">Select...</option>
                <option>Very Important</option>
                <option>Moderately Important</option>
                <option>Not Important</option>
              </select>
            </div>
            <span class="col-xs-1 col-sm-1 col-md-1 col-lg-1 glyphicon glyphicon-info-sign criteria-description-in-tooltip tooltips" data-tooltip-content="#info-framework-size"></span>
          </div>
          <div class="form-group">
            <label class="col-xs-5 col-sm-5 col-md-5 col-lg-3 control-label" for="timeInHand">Time in hand</label>
            <div class="col-xs-6 col-sm-6 col-md-6 col-lg-8">
              <select v-model="timeInHand" class="form-control" id="timeInHand" v-on:change="frameworkFilter('timeInHand', timeInHand)">
                <option disabled value="">Select...</option>
                <option>No Time Constraint</option>
                <option>Routine</option>
                <option>Urgent</option>
              </select>
            </div>
            <span class="col-xs-1 col-sm-1 col-md-1 col-lg-1 glyphicon glyphicon-info-sign criteria-description-in-tooltip tooltips" data-tooltip-content="#info-time-in-hand"></span>
          </div>
          <div class="form-group">
            <label class="col-xs-5 col-sm-5 col-md-5 col-lg-3 control-label" for="language">Language</label>
            <div class="col-xs-6 col-sm-6 col-md-6 col-lg-8">
              <select v-model="language" class="form-control" id="language" v-on:change="frameworkFilter('language'+language, language)">
                <option disabled value="">Select...</option>
                <option>ES6</option>
                <option>TypeScript</option>
              </select>
            </div>
            <span class="col-xs-1 col-sm-1 col-md-1 col-lg-1 glyphicon glyphicon-info-sign criteria-description-in-tooltip tooltips" data-tooltip-content="#info-language"></span>
          </div>
          <div class="form-group">
            <label class="col-xs-5 col-sm-5 col-md-5 col-lg-3 control-label" for="appSize">App Size</label>
            <div class="col-xs-6 col-sm-6 col-md-6 col-lg-8">
              <select v-model="appSize" class="form-control" id="appSize" v-on:change="frameworkFilter('appSize', appSize)">
                <option disabled value="">Select...</option>
                <option>Small</option>
                <option>Medium</option>
                <option>Big</option>
              </select>
            </div>
            <span class="col-xs-1 col-sm-1 col-md-1 col-lg-1 glyphicon glyphicon-info-sign criteria-description-in-tooltip tooltips" data-tooltip-content="#info-app-size"></span>
          </div>
          <div class="form-group">
            <label class="col-xs-5 col-sm-5 col-md-5 col-lg-3 control-label" for="learningCurve">Learning Curve</label>
            <div class="col-xs-6 col-sm-6 col-md-6 col-lg-8">
              <select v-model="learningCurve" class="form-control" id="learningCurve" v-on:change="frameworkFilter('learningCurve', learningCurve)">
                <option disabled value="">Select...</option>
                <option>Very Important</option>
                <option>Moderately Important</option>
                <option>Not Important</option>
              </select>
            </div>
            <span class="col-xs-1 col-sm-1 col-md-1 col-lg-1 glyphicon glyphicon-info-sign criteria-description-in-tooltip tooltips" data-tooltip-content="#info-learning-curve"></span>
          </div>
          <div class="form-group">
            <label class="col-xs-5 col-sm-5 col-md-5 col-lg-3 control-label" for="standardsComplaint">Standards Complaint</label>
            <div class="col-xs-6 col-sm-6 col-md-6 col-lg-8">
              <select v-model="standardsComplaint" class="form-control" id="standardsComplaint" v-on:change="frameworkFilter('standardsComplaint', standardsComplaint)">
                <option disabled value="">Select...</option>
                <option>Very Important</option>
                <option>Moderately Important</option>
                <option>Not Important</option>
              </select>
            </div>
            <span class="col-xs-1 col-sm-1 col-md-1 col-lg-1 glyphicon glyphicon-info-sign criteria-description-in-tooltip tooltips" data-tooltip-content="#info-standards-complaint"></span>
          </div>
        </form>
      </div>


      <!--Accordion Start-->

      <div class="col-sm-6 col-md-6 col-lg-6">
        <div class="panel-group" id="accordion" role="tablist" aria-multiselectable="true">
          <div class="panel panel-default">
            <div class="panel-heading" role="tab" id="headingOne">
              <h4 class="panel-title">
                <a role="button" data-toggle="collapse" data-parent="#accordion" href="#collapseOne" aria-expanded="true" aria-controls="collapseOne" class="test-accordion-style">
                  Angular 2
                  <span class="total-percentage">
                                        {{this.totalPercentageAngular}}%
                                    </span>
                </a>
              </h4>
            </div>
            <div id="collapseOne" class="panel-collapse collapse in" role="tabpanel" aria-labelledby="headingOne">
              <div class="panel-body">
                <table class="table table-striped table-hover test-table-style">
                  <tbody>
                  <tr>
                    <th>Scalability</th>
                    <td class="col-xs-1 col-sm-2 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularScalabilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularScalabilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularScalabilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Modularity</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularModularityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularModularityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularModularityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Backwards Compatibility</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularBackwardsCompatibilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularBackwardsCompatibilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularBackwardsCompatibilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Testability</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularTestabilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularTestabilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularTestabilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Support</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularSupportLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularSupportMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularSupportHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Future</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularFutureLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularFutureMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularFutureHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Performance</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularPerformanceLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularPerformanceMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularPerformanceHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Customizability</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularCustomizabilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularCustomizabilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularCustomizabilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Readability</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularReadabilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularReadabilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularReadabilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Framework Size</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularFrameworkSizeLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularFrameworkSizeMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularFrameworkSizeHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Time in hand</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularTimeInHandLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularTimeInHandMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularTimeInHandHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Language</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularLanguageLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularLanguageMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularLanguageHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>App Size</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularAppSizeLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularAppSizeMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularAppSizeHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Learning Curve</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularLearningCurveLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularLearningCurveMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularLearningCurveHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Standards Complaint</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularStandardsComplaintLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularStandardsComplaintMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularStandardsComplaintHigh"></div>
                      </div>
                    </td>
                  </tr>
                  </tbody>
                </table>
              </div>
            </div>
          </div>
          <div class="panel panel-default">
            <div class="panel-heading" role="tab" id="headingTwo">
              <h4 class="panel-title">
                <a class="collapsed" role="button" data-toggle="collapse" data-parent="#accordion" href="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
                  React
                  <span class="total-percentage">
                    {{this.totalPercentageReact}}%
                  </span>
                </a>
              </h4>
            </div>
            <div id="collapseTwo" class="panel-collapse collapse" role="tabpanel" aria-labelledby="headingTwo">
              <div class="panel-body">

                <table class="table table-striped table-hover">
                  <tbody>
                  <tr>
                    <th>Scalability</th>
                    <td class="col-xs-1 col-sm-2 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactScalabilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactScalabilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactScalabilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Modularity</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactModularityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactModularityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactModularityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Backwards Compatibility</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactBackwardsCompatibilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactBackwardsCompatibilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactBackwardsCompatibilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Testability</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactTestabilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactTestabilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactTestabilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Support</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactSupportLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactSupportMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactSupportHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Future</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactFutureLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactFutureMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactFutureHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Performance</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactPerformanceLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactPerformanceMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactPerformanceHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Customizability</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactCustomizabilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactCustomizabilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactCustomizabilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Readability</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactReadabilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactReadabilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactReadabilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Framework Size</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactFrameworkSizeLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactFrameworkSizeMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactFrameworkSizeHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Time in hand</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactTimeInHandLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactTimeInHandMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactTimeInHandHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Language</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactLanguageLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactLanguageMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactLanguageHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>App Size</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactAppSizeLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactAppSizeMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactAppSizeHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Learning Curve</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactLearningCurveLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactLearningCurveMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactLearningCurveHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Standards Complaint</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactStandardsComplaintLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactStandardsComplaintMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactStandardsComplaintHigh"></div>
                      </div>
                    </td>
                  </tr>
                  </tbody>
                </table>

              </div>
            </div>
          </div>
          <div class="panel panel-default">
            <div class="panel-heading" role="tab" id="headingThree">
              <h4 class="panel-title">
                <a class="collapsed" role="button" data-toggle="collapse" data-parent="#accordion" href="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
                  Vue 2
                  <span class="total-percentage">
                    {{this.totalPercentageVue}}%
                  </span>
                </a>
              </h4>
            </div>
            <div id="collapseThree" class="panel-collapse collapse" role="tabpanel" aria-labelledby="headingThree">
              <div class="panel-body">

                <table class="table table-striped table-hover">
                  <tbody>
                  <tr>
                    <th>Scalability</th>
                    <td class="col-xs-1 col-sm-2 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueScalabilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueScalabilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueScalabilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Modularity</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueModularityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueModularityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueModularityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Backwards Compatibility</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueBackwardsCompatibilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueBackwardsCompatibilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueBackwardsCompatibilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Testability</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueTestabilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueTestabilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueTestabilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Support</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueSupportLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueSupportMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueSupportHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Future</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueFutureLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueFutureMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueFutureHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Performance</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vuePerformanceLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vuePerformanceMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vuePerformanceHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Customizability</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueCustomizabilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueCustomizabilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueCustomizabilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Readability</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueReadabilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueReadabilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueReadabilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Framework Size</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueFrameworkSizeLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueFrameworkSizeMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueFrameworkSizeHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Time in hand</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueTimeInHandLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueTimeInHandMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueTimeInHandHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Language</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueLanguageLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueLanguageMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueLanguageHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>App Size</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueAppSizeLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueAppSizeMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueAppSizeHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Learning Curve</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueLearningCurveLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueLearningCurveMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueLearningCurveHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Standards Complaint</th>
                    <td class="col-xs-5 col-sm-5 col-md-5 col-lg-5">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueStandardsComplaintLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueStandardsComplaintMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueStandardsComplaintHigh"></div>
                      </div>
                    </td>
                  </tr>
                  </tbody>
                </table>

              </div>
            </div>
          </div>
        </div>

        <div class="important-note-about-total-percentage">
          <h4 class="important-note-title">Important Note</h4>
          <p class="criteria-description-in-tooltip important-note">Percentage shows overall result, which <span class="criteria-options-meaning">doesn't necessarily mean</span> that the higher the percentage the higher the suitability.</p>
          <p class="criteria-description-in-tooltip important-note">Please check <span class="criteria-options-meaning">individual results</span> for most important criteria for your project.</p>

          <br>

          <h4 class="important-note-title">Criteria Strength Bar</h4>
          <p class="criteria-description-in-tooltip important-note"><span class="criteria-options-meaning" style="color: #d9534f;">RED: </span>Not important for user <span class="criteria-options-meaning">OR</span> Weak support in framework.</p>
          <p class="criteria-description-in-tooltip important-note"><span class="criteria-options-meaning" style="color: #5cb85c;">GREEN: </span>Moderately important for user <span class="criteria-options-meaning">OR</span> Moderate support in framework.</p>
          <p class="criteria-description-in-tooltip important-note"><span class="criteria-options-meaning" style="color: #5bc0de;">BLUE: </span>Very important for user <span class="criteria-options-meaning">AND</span> Strong support in framework.</p>
        </div>

      </div>


      <!--Accordion End-->

    </div>

    <div id="footer">
      <a class="git-link" href="https://goo.gl/forms/6sakUAormUq3IkU43" target="_blank">Feedback</a>
    </div>

  </div>

</template>

<script>

  export default {
    beforeMount(){

      $(function () {
        let footerHeight = 0,
          footerTop = 0,
          $footer = $("#footer");
        positionFooter();
        function positionFooter() {
          footerHeight = $footer.height();
          footerTop = ($(window).scrollTop()+$(window).height()-footerHeight)+"px";
          if ( ($(document.body).height()+footerHeight) < $(window).height()) {
            $footer.css({
              position: "absolute",
              top: footerTop
            })
          } else {
            $footer.css({
              position: "static"
            })
          }
        }
        $(window)
          .scroll(positionFooter)
          .resize(positionFooter)
      });

      $(function () {
        $('.tooltips').tooltipster({
          theme: ['tooltipster-shadow', 'tooltipster-shadow-customized'],
          delay: 0,
          maxWidth: 500,
          side: "left",
          trigger: 'custom',
          triggerOpen: {
            mouseenter: true,
            tap: true,
            delayTouch: 0,
          },
          triggerClose: {
            scroll: true,
            tap: true,
            mouseleave: true,
          }
        });
      });

    },

    name: 'hello',
    data () {
      return {
        recommendedFrameworkByUser: this.recommendedFrameworkByUser,
        emailFormOptionalMessage: this.emailFormOptionalMessage,
        scalability: '',
        modularity: '',
        backwardsCompatibility: '',
        testability: '',
        support: '',
        future: '',
        performance: '',
        customizability: '',
        readability: '',
        frameworkSize: '',
        timeInHand: '',
        language: '',
        appSize: '',
        learningCurve: '',
        standardsComplaint: '',

        totalCriteria: 16,
        totalPercentageAngular: 0,
        totalPercentageReact: 0,
        totalPercentageVue: 0,
        formEdited: false,

        angularScalabilityPercentage: 0,
        angularModularityPercentage: 0,
        angularBackwardsCompatibilityPercentage: 0,
        angularTestabilityPercentage: 0,
        angularSupportPercentage: 0,
        angularFuturePercentage: 0,
        angularPerformancePercentage: 0,
        angularCustomizabilityPercentage: 0,
        angularReadabilityPercentage: 0,
        angularFrameworkSizePercentage: 0,
        angularTimeInHandPercentage: 0,
        angularLanguagePercentage: 0,
        angularAppSizePercentage: 0,
        angularLearningCurvePercentage: 0,
        angularStandardsComplaintPercentage: 0,

        reactScalabilityPercentage: 0,
        reactModularityPercentage: 0,
        reactBackwardsCompatibilityPercentage: 0,
        reactTestabilityPercentage: 0,
        reactSupportPercentage: 0,
        reactFuturePercentage: 0,
        reactPerformancePercentage: 0,
        reactCustomizabilityPercentage: 0,
        reactReadabilityPercentage: 0,
        reactFrameworkSizePercentage: 0,
        reactTimeInHandPercentage: 0,
        reactLanguagePercentage: 0,
        reactAppSizePercentage: 0,
        reactLearningCurvePercentage: 0,
        reactStandardsComplaintPercentage: 0,

        vueScalabilityPercentage: 0,
        vueModularityPercentage: 0,
        vueBackwardsCompatibilityPercentage: 0,
        vueTestabilityPercentage: 0,
        vueSupportPercentage: 0,
        vueFuturePercentage: 0,
        vuePerformancePercentage: 0,
        vueCustomizabilityPercentage: 0,
        vueReadabilityPercentage: 0,
        vueFrameworkSizePercentage: 0,
        vueTimeInHandPercentage: 0,
        vueLanguagePercentage: 0,
        vueAppSizePercentage: 0,
        vueLearningCurvePercentage: 0,
        vueStandardsComplaintPercentage: 0,

        angularScalabilityLow: this.angularScalabilityLow,
        angularScalabilityMid: this.angularScalabilityMid,
        angularScalabilityHigh: this.angularScalabilityHigh,
        angularModularityLow: this.angularModularityLow,
        angularModularityMid: this.angularModularityMid,
        angularModularityHigh: this.angularModularityHigh,
        angularBackwardsCompatibilityLow: this.angularBackwardsCompatibilityLow,
        angularBackwardsCompatibilityMid: this.angularBackwardsCompatibilityMid,
        angularBackwardsCompatibilityHigh: this.angularBackwardsCompatibilityHigh,
        angularTestabilityLow: this.angularTestabilityLow,
        angularTestabilityMid: this.angularTestabilityMid,
        angularTestabilityHigh: this.angularTestabilityHigh,
        angularSupportLow: this.angularSupportLow,
        angularSupportMid: this.angularSupportMid,
        angularSupportHigh: this.angularSupportHigh,
        angularFutureLow: this.angularFutureLow,
        angularFutureMid: this.angularFutureMid,
        angularFutureHigh: this.angularFutureHigh,
        angularPerformanceLow: this.angularPerformanceLow,
        angularPerformanceMid: this.angularPerformanceMid,
        angularPerformanceHigh: this.angularPerformanceHigh,
        angularCustomizabilityLow: this.angularCustomizabilityLow,
        angularCustomizabilityMid: this.angularCustomizabilityMid,
        angularCustomizabilityHigh: this.angularCustomizabilityHigh,
        angularReadabilityLow: this.angularReadabilityLow,
        angularReadabilityMid: this.angularReadabilityMid,
        angularReadabilityHigh: this.angularReadabilityHigh,
        angularFrameworkSizeLow: this.angularFrameworkSizeLow,
        angularFrameworkSizeMid: this.angularFrameworkSizeMid,
        angularFrameworkSizeHigh: this.angularFrameworkSizeHigh,
        angularTimeInHandLow: this.angularTimeInHandLow,
        angularTimeInHandMid: this.angularTimeInHandMid,
        angularTimeInHandHigh: this.angularTimeInHandHigh,
        angularLanguageLow: this.angularLanguageLow,
        angularLanguageMid: this.angularLanguageMid,
        angularLanguageHigh: this.angularLanguageHigh,
        angularAppSizeLow: this.angularAppSizeLow,
        angularAppSizeMid: this.angularAppSizeMid,
        angularAppSizeHigh: this.angularAppSizeHigh,
        angularLearningCurveLow: this.angularLearningCurveLow,
        angularLearningCurveMid: this.angularLearningCurveMid,
        angularLearningCurveHigh: this.angularLearningCurveHigh,
        angularStandardsComplaintLow: this.angularStandardsComplaintLow,
        angularStandardsComplaintMid: this.angularStandardsComplaintMid,
        angularStandardsComplaintHigh: this.angularStandardsComplaintHigh,

        reactScalabilityLow: this.reactScalabilityLow,
        reactScalabilityMid: this.reactScalabilityMid,
        reactScalabilityHigh: this.reactScalabilityHigh,
        reactModularityLow: this.reactModularityLow,
        reactModularityMid: this.reactModularityMid,
        reactModularityHigh: this.reactModularityHigh,
        reactBackwardsCompatibilityLow: this.reactBackwardsCompatibilityLow,
        reactBackwardsCompatibilityMid: this.reactBackwardsCompatibilityMid,
        reactBackwardsCompatibilityHigh: this.reactBackwardsCompatibilityHigh,
        reactTestabilityLow: this.reactTestabilityLow,
        reactTestabilityMid: this.reactTestabilityMid,
        reactTestabilityHigh: this.reactTestabilityHigh,
        reactSupportLow: this.reactSupportLow,
        reactSupportMid: this.reactSupportMid,
        reactSupportHigh: this.reactSupportHigh,
        reactFutureLow: this.reactFutureLow,
        reactFutureMid: this.reactFutureMid,
        reactFutureHigh: this.reactFutureHigh,
        reactPerformanceLow: this.reactPerformanceLow,
        reactPerformanceMid: this.reactPerformanceMid,
        reactPerformanceHigh: this.reactPerformanceHigh,
        reactCustomizabilityLow: this.reactCustomizabilityLow,
        reactCustomizabilityMid: this.reactCustomizabilityMid,
        reactCustomizabilityHigh: this.reactCustomizabilityHigh,
        reactReadabilityLow: this.reactReadabilityLow,
        reactReadabilityMid: this.reactReadabilityMid,
        reactReadabilityHigh: this.reactReadabilityHigh,
        reactFrameworkSizeLow: this.reactFrameworkSizeLow,
        reactFrameworkSizeMid: this.reactFrameworkSizeMid,
        reactFrameworkSizeHigh: this.reactFrameworkSizeHigh,
        reactTimeInHandLow: this.reactTimeInHandLow,
        reactTimeInHandMid: this.reactTimeInHandMid,
        reactTimeInHandHigh: this.reactTimeInHandHigh,
        reactLanguageLow: this.reactLanguageLow,
        reactLanguageMid: this.reactLanguageMid,
        reactLanguageHigh: this.reactLanguageHigh,
        reactAppSizeLow: this.reactAppSizeLow,
        reactAppSizeMid: this.reactAppSizeMid,
        reactAppSizeHigh: this.reactAppSizeHigh,
        reactLearningCurveLow: this.reactLearningCurveLow,
        reactLearningCurveMid: this.reactLearningCurveMid,
        reactLearningCurveHigh: this.reactLearningCurveHigh,
        reactStandardsComplaintLow: this.reactStandardsComplaintLow,
        reactStandardsComplaintMid: this.reactStandardsComplaintMid,
        reactStandardsComplaintHigh: this.reactStandardsComplaintHigh,

        vueScalabilityLow: this.vueScalabilityLow,
        vueScalabilityMid: this.vueScalabilityMid,
        vueScalabilityHigh: this.vueScalabilityHigh,
        vueModularityLow: this.vueModularityLow,
        vueModularityMid: this.vueModularityMid,
        vueModularityHigh: this.vueModularityHigh,
        vueBackwardsCompatibilityLow: this.vueBackwardsCompatibilityLow,
        vueBackwardsCompatibilityMid: this.vueBackwardsCompatibilityMid,
        vueBackwardsCompatibilityHigh: this.vueBackwardsCompatibilityHigh,
        vueTestabilityLow: this.vueTestabilityLow,
        vueTestabilityMid: this.vueTestabilityMid,
        vueTestabilityHigh: this.vueTestabilityHigh,
        vueSupportLow: this.vueSupportLow,
        vueSupportMid: this.vueSupportMid,
        vueSupportHigh: this.vueSupportHigh,
        vueFutureLow: this.vueFutureLow,
        vueFutureMid: this.vueFutureMid,
        vueFutureHigh: this.vueFutureHigh,
        vuePerformanceLow: this.vuePerformanceLow,
        vuePerformanceMid: this.vuePerformanceMid,
        vuePerformanceHigh: this.vuePerformanceHigh,
        vueCustomizabilityLow: this.vueCustomizabilityLow,
        vueCustomizabilityMid: this.vueCustomizabilityMid,
        vueCustomizabilityHigh: this.vueCustomizabilityHigh,
        vueReadabilityLow: this.vueReadabilityLow,
        vueReadabilityMid: this.vueReadabilityMid,
        vueReadabilityHigh: this.vueReadabilityHigh,
        vueFrameworkSizeLow: this.vueFrameworkSizeLow,
        vueFrameworkSizeMid: this.vueFrameworkSizeMid,
        vueFrameworkSizeHigh: this.vueFrameworkSizeHigh,
        vueTimeInHandLow: this.vueTimeInHandLow,
        vueTimeInHandMid: this.vueTimeInHandMid,
        vueTimeInHandHigh: this.vueTimeInHandHigh,
        vueLanguageLow: this.vueLanguageLow,
        vueLanguageMid: this.vueLanguageMid,
        vueLanguageHigh: this.vueLanguageHigh,
        vueAppSizeLow: this.vueAppSizeLow,
        vueAppSizeMid: this.vueAppSizeMid,
        vueAppSizeHigh: this.vueAppSizeHigh,
        vueLearningCurveLow: this.vueLearningCurveLow,
        vueLearningCurveMid: this.vueLearningCurveMid,
        vueLearningCurveHigh: this.vueLearningCurveHigh,
        vueStandardsComplaintLow: this.vueStandardsComplaintLow,
        vueStandardsComplaintMid: this.vueStandardsComplaintMid,
        vueStandardsComplaintHigh: this.vueStandardsComplaintHigh,

        frameworksData:
          {
            Angular: {
              scalability:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              modularity:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              backwardsCompatibility:
                {
                  strength: "Not Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              testability:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              support:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              future:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              performance:
                {
                  strength: "Partially Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              customizability:
                {
                  strength: "Not Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              readability:
                {
                  strength: "Partially Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              frameworkSize:
                {
                  strength: "Not Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              timeInHand:
                {
                  strength: "Not Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              languageES6:
                {
                  strength: "Partially Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              languageTypeScript:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              appSize:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              learningCurve:
                {
                  strength: "Not Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              standardsComplaint:
                {
                  strength: "Not Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              meanTotalScore: 0,
              totalPercentage: 0
            },
            React: {
              scalability:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              modularity:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              backwardsCompatibility:
                {
                  strength: "Partially Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              testability:
                {
                  strength: "Not Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              support:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              future:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              performance:
                {
                  strength: "Partially Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              customizability:
                {
                  strength: "Partially Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              readability:
                {
                  strength: "Partially Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              frameworkSize:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              timeInHand:
                {
                  strength: "Partially Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              languageES6:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              languageTypeScript:
                {
                  strength: "Not Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              appSize:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              learningCurve:
                {
                  strength: "Partially Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              standardsComplaint:
                {
                  strength: "Not Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              meanTotalScore: 0,
              totalPercentage: 0
            },
            Vue:{
              scalability:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              modularity:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              backwardsCompatibility:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              testability:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              support:
                {
                  strength: "Partially Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              future:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              performance:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              customizability:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              readability:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              frameworkSize:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              timeInHand:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              languageES6:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              languageTypeScript:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              appSize:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              learningCurve:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              standardsComplaint:
                {
                  strength: "Available",
                  goalMet: 1,
                  score: 0,
                  percentage: 0
                },
              meanTotalScore: 0,
              totalPercentage: 0
            }
          }
      }
    },

    methods:{
        frameworkFilter: function (selectedCriteria, userSelection)
        {
          $('.clear-data').removeClass('clear-button-disabled');
          $('.clear-data-mobile').removeClass('clear-button-disabled');
          this.formEdited = true;
          let fdParent = this.frameworksData;
          let weightPerCriteria = this.getWeightPerCriteria(this.totalCriteria);
          let maxCriteriaScore = 3 * weightPerCriteria;

          for (let keyParent in fdParent)
          {
            if (fdParent.hasOwnProperty(keyParent))
            {
              let framework = keyParent;
              let fdChild = fdParent[keyParent];

              for (let keyChild in fdChild)
              {
                if (fdChild.hasOwnProperty(keyChild))
                {
                  let fdSubChild = fdChild[keyChild];

                  if (keyChild === selectedCriteria) {

                    fdSubChild["goalMet"] = this.calculateGoalMet(framework, selectedCriteria, userSelection, fdSubChild['strength']);
                    fdSubChild["score"] = fdSubChild["goalMet"] * weightPerCriteria;
                    fdSubChild["percentage"] = Math.round(fdSubChild["score"] / (maxCriteriaScore) * 100);
                    this.setIndividualPercentage(framework, selectedCriteria, fdSubChild["percentage"]);
                  }
                }
              }
            }
          }

          this.setMeanTotalScore(maxCriteriaScore, this.language);
  //                this.generateReport();
      },

      setIndividualPercentage: function (currentFramework, currentCriteria, currentCriteriaPercentage)
      {
        if (currentFramework === "Angular")
        {
          if (currentCriteria === "scalability")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularScalabilityLow = 'width: 33%;';
              this.angularScalabilityMid = 'width: 0%;';
              this.angularScalabilityHigh = 'width: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularScalabilityLow = 'width: 33%;';
              this.angularScalabilityMid = 'width: 33%;';
              this.angularScalabilityHigh = 'width: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularScalabilityLow = 'width: 33%;';
              this.angularScalabilityMid = 'width: 33%;';
              this.angularScalabilityHigh = 'width: 34%;';
            }

          }
          else if (currentCriteria === "modularity")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularModularityLow = 'width: 33%;';
              this.angularModularityMid = 'height: 0%;';
              this.angularModularityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularModularityLow = 'width: 33%;';
              this.angularModularityMid = 'width: 33%;';
              this.angularModularityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularModularityLow = 'width: 33%;';
              this.angularModularityMid = 'width: 33%;';
              this.angularModularityHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "backwardsCompatibility")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularBackwardsCompatibilityLow = 'width: 33%;';
              this.angularBackwardsCompatibilityMid = 'height: 0%;';
              this.angularBackwardsCompatibilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularBackwardsCompatibilityLow = 'width: 33%;';
              this.angularBackwardsCompatibilityMid = 'width: 33%;';
              this.angularBackwardsCompatibilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularBackwardsCompatibilityLow = 'width: 33%;';
              this.angularBackwardsCompatibilityMid = 'width: 33%;';
              this.angularBackwardsCompatibilityHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "testability")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularTestabilityLow = 'width: 33%;';
              this.angularTestabilityMid = 'height: 0%;';
              this.angularTestabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularTestabilityLow = 'width: 33%;';
              this.angularTestabilityMid = 'width: 33%;';
              this.angularTestabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularTestabilityLow = 'width: 33%;';
              this.angularTestabilityMid = 'width: 33%;';
              this.angularTestabilityHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "support")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularSupportLow = 'width: 33%;';
              this.angularSupportMid = 'height: 0%;';
              this.angularSupportHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularSupportLow = 'width: 33%;';
              this.angularSupportMid = 'width: 33%;';
              this.angularSupportHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularSupportLow = 'width: 33%;';
              this.angularSupportMid = 'width: 33%;';
              this.angularSupportHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "future")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularFutureLow = 'width: 33%;';
              this.angularFutureMid = 'height: 0%;';
              this.angularFutureHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularFutureLow = 'width: 33%;';
              this.angularFutureMid = 'width: 33%;';
              this.angularFutureHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularFutureLow = 'width: 33%;';
              this.angularFutureMid = 'width: 33%;';
              this.angularFutureHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "performance")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularPerformanceLow = 'width: 33%;';
              this.angularPerformanceMid = 'height: 0%;';
              this.angularPerformanceHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularPerformanceLow = 'width: 33%;';
              this.angularPerformanceMid = 'width: 33%;';
              this.angularPerformanceHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularPerformanceLow = 'width: 33%;';
              this.angularPerformanceMid = 'width: 33%;';
              this.angularPerformanceHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "customizability")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularCustomizabilityLow = 'width: 33%;';
              this.angularCustomizabilityMid = 'height: 0%;';
              this.angularCustomizabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularCustomizabilityLow = 'width: 33%;';
              this.angularCustomizabilityMid = 'width: 33%;';
              this.angularCustomizabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularCustomizabilityLow = 'width: 33%;';
              this.angularCustomizabilityMid = 'width: 33%;';
              this.angularCustomizabilityHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "readability")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularReadabilityLow = 'width: 33%;';
              this.angularReadabilityMid = 'height: 0%;';
              this.angularReadabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularReadabilityLow = 'width: 33%;';
              this.angularReadabilityMid = 'width: 33%;';
              this.angularReadabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularReadabilityLow = 'width: 33%;';
              this.angularReadabilityMid = 'width: 33%;';
              this.angularReadabilityHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "frameworkSize")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularFrameworkSizeLow = 'width: 33%;';
              this.angularFrameworkSizeMid = 'height: 0%;';
              this.angularFrameworkSizeHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularFrameworkSizeLow = 'width: 33%;';
              this.angularFrameworkSizeMid = 'width: 33%;';
              this.angularFrameworkSizeHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularFrameworkSizeLow = 'width: 33%;';
              this.angularFrameworkSizeMid = 'width: 33%;';
              this.angularFrameworkSizeHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "timeInHand")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularTimeInHandLow = 'width: 33%;';
              this.angularTimeInHandMid = 'height: 0%;';
              this.angularTimeInHandHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularTimeInHandLow = 'width: 33%;';
              this.angularTimeInHandMid = 'width: 33%;';
              this.angularTimeInHandHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularTimeInHandLow = 'width: 33%;';
              this.angularTimeInHandMid = 'width: 33%;';
              this.angularTimeInHandHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "languageES6")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularLanguageLow = 'width: 33%;';
              this.angularLanguageMid = 'height: 0%;';
              this.angularLanguageHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularLanguageLow = 'width: 33%;';
              this.angularLanguageMid = 'width: 33%;';
              this.angularLanguageHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularLanguageLow = 'width: 33%;';
              this.angularLanguageMid = 'width: 33%;';
              this.angularLanguageHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "languageTypeScript")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularLanguageLow = 'width: 33%;';
              this.angularLanguageMid = 'height: 0%;';
              this.angularLanguageHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularLanguageLow = 'width: 33%;';
              this.angularLanguageMid = 'width: 33%;';
              this.angularLanguageHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularLanguageLow = 'width: 33%;';
              this.angularLanguageMid = 'width: 33%;';
              this.angularLanguageHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "appSize")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularAppSizeLow = 'width: 33%;';
              this.angularAppSizeMid = 'height: 0%;';
              this.angularAppSizeHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularAppSizeLow = 'width: 33%;';
              this.angularAppSizeMid = 'width: 33%;';
              this.angularAppSizeHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularAppSizeLow = 'width: 33%;';
              this.angularAppSizeMid = 'width: 33%;';
              this.angularAppSizeHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "learningCurve")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularLearningCurveLow = 'width: 33%;';
              this.angularLearningCurveMid = 'height: 0%;';
              this.angularLearningCurveHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularLearningCurveLow = 'width: 33%;';
              this.angularLearningCurveMid = 'width: 33%;';
              this.angularLearningCurveHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularLearningCurveLow = 'width: 33%;';
              this.angularLearningCurveMid = 'width: 33%;';
              this.angularLearningCurveHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "standardsComplaint")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularStandardsComplaintLow = 'width: 33%;';
              this.angularStandardsComplaintMid = 'height: 0%;';
              this.angularStandardsComplaintHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularStandardsComplaintLow = 'width: 33%;';
              this.angularStandardsComplaintMid = 'width: 33%;';
              this.angularStandardsComplaintHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularStandardsComplaintLow = 'width: 33%;';
              this.angularStandardsComplaintMid = 'width: 33%;';
              this.angularStandardsComplaintHigh = 'width: 34%;';
            }
          }
        }
        else if (currentFramework === "React")
        {
          if (currentCriteria === "scalability")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactScalabilityLow = 'width: 33%;';
              this.reactScalabilityMid = 'height: 0%;';
              this.reactScalabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactScalabilityLow = 'width: 33%;';
              this.reactScalabilityMid = 'width: 33%;';
              this.reactScalabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactScalabilityLow = 'width: 33%;';
              this.reactScalabilityMid = 'width: 33%;';
              this.reactScalabilityHigh = 'width: 34%;';
            }

          }
          else if (currentCriteria === "modularity")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactModularityLow = 'width: 33%;';
              this.reactModularityMid = 'height: 0%;';
              this.reactModularityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactModularityLow = 'width: 33%;';
              this.reactModularityMid = 'width: 33%;';
              this.reactModularityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactModularityLow = 'width: 33%;';
              this.reactModularityMid = 'width: 33%;';
              this.reactModularityHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "backwardsCompatibility")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactBackwardsCompatibilityLow = 'width: 33%;';
              this.reactBackwardsCompatibilityMid = 'height: 0%;';
              this.reactBackwardsCompatibilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactBackwardsCompatibilityLow = 'width: 33%;';
              this.reactBackwardsCompatibilityMid = 'width: 33%;';
              this.reactBackwardsCompatibilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactBackwardsCompatibilityLow = 'width: 33%;';
              this.reactBackwardsCompatibilityMid = 'width: 33%;';
              this.reactBackwardsCompatibilityHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "testability")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactTestabilityLow = 'width: 33%;';
              this.reactTestabilityMid = 'height: 0%;';
              this.reactTestabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactTestabilityLow = 'width: 33%;';
              this.reactTestabilityMid = 'width: 33%;';
              this.reactTestabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactTestabilityLow = 'width: 33%;';
              this.reactTestabilityMid = 'width: 33%;';
              this.reactTestabilityHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "support")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactSupportLow = 'width: 33%;';
              this.reactSupportMid = 'height: 0%;';
              this.reactSupportHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactSupportLow = 'width: 33%;';
              this.reactSupportMid = 'width: 33%;';
              this.reactSupportHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactSupportLow = 'width: 33%;';
              this.reactSupportMid = 'width: 33%;';
              this.reactSupportHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "future")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactFutureLow = 'width: 33%;';
              this.reactFutureMid = 'height: 0%;';
              this.reactFutureHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactFutureLow = 'width: 33%;';
              this.reactFutureMid = 'width: 33%;';
              this.reactFutureHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactFutureLow = 'width: 33%;';
              this.reactFutureMid = 'width: 33%;';
              this.reactFutureHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "performance")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactPerformanceLow = 'width: 33%;';
              this.reactPerformanceMid = 'height: 0%;';
              this.reactPerformanceHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactPerformanceLow = 'width: 33%;';
              this.reactPerformanceMid = 'width: 33%;';
              this.reactPerformanceHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactPerformanceLow = 'width: 33%;';
              this.reactPerformanceMid = 'width: 33%;';
              this.reactPerformanceHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "customizability")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactCustomizabilityLow = 'width: 33%;';
              this.reactCustomizabilityMid = 'height: 0%;';
              this.reactCustomizabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactCustomizabilityLow = 'width: 33%;';
              this.reactCustomizabilityMid = 'width: 33%;';
              this.reactCustomizabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactCustomizabilityLow = 'width: 33%;';
              this.reactCustomizabilityMid = 'width: 33%;';
              this.reactCustomizabilityHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "readability")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactReadabilityLow = 'width: 33%;';
              this.reactReadabilityMid = 'height: 0%;';
              this.reactReadabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactReadabilityLow = 'width: 33%;';
              this.reactReadabilityMid = 'width: 33%;';
              this.reactReadabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactReadabilityLow = 'width: 33%;';
              this.reactReadabilityMid = 'width: 33%;';
              this.reactReadabilityHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "frameworkSize")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactFrameworkSizeLow = 'width: 33%;';
              this.reactFrameworkSizeMid = 'height: 0%;';
              this.reactFrameworkSizeHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactFrameworkSizeLow = 'width: 33%;';
              this.reactFrameworkSizeMid = 'width: 33%;';
              this.reactFrameworkSizeHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactFrameworkSizeLow = 'width: 33%;';
              this.reactFrameworkSizeMid = 'width: 33%;';
              this.reactFrameworkSizeHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "timeInHand")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactTimeInHandLow = 'width: 33%;';
              this.reactTimeInHandMid = 'height: 0%;';
              this.reactTimeInHandHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactTimeInHandLow = 'width: 33%;';
              this.reactTimeInHandMid = 'width: 33%;';
              this.reactTimeInHandHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactTimeInHandLow = 'width: 33%;';
              this.reactTimeInHandMid = 'width: 33%;';
              this.reactTimeInHandHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "languageES6")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactLanguageLow = 'width: 33%;';
              this.reactLanguageMid = 'height: 0%;';
              this.reactLanguageHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactLanguageLow = 'width: 33%;';
              this.reactLanguageMid = 'width: 33%;';
              this.reactLanguageHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactLanguageLow = 'width: 33%;';
              this.reactLanguageMid = 'width: 33%;';
              this.reactLanguageHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "languageTypeScript")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactLanguageLow = 'width: 33%;';
              this.reactLanguageMid = 'height: 0%;';
              this.reactLanguageHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactLanguageLow = 'width: 33%;';
              this.reactLanguageMid = 'width: 33%;';
              this.reactLanguageHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactLanguageLow = 'width: 33%;';
              this.reactLanguageMid = 'width: 33%;';
              this.reactLanguageHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "appSize")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactAppSizeLow = 'width: 33%;';
              this.reactAppSizeMid = 'height: 0%;';
              this.reactAppSizeHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactAppSizeLow = 'width: 33%;';
              this.reactAppSizeMid = 'width: 33%;';
              this.reactAppSizeHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactAppSizeLow = 'width: 33%;';
              this.reactAppSizeMid = 'width: 33%;';
              this.reactAppSizeHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "learningCurve")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactLearningCurveLow = 'width: 33%;';
              this.reactLearningCurveMid = 'height: 0%;';
              this.reactLearningCurveHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactLearningCurveLow = 'width: 33%;';
              this.reactLearningCurveMid = 'width: 33%;';
              this.reactLearningCurveHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactLearningCurveLow = 'width: 33%;';
              this.reactLearningCurveMid = 'width: 33%;';
              this.reactLearningCurveHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "standardsComplaint")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactStandardsComplaintLow = 'width: 33%;';
              this.reactStandardsComplaintMid = 'height: 0%;';
              this.reactStandardsComplaintHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactStandardsComplaintLow = 'width: 33%;';
              this.reactStandardsComplaintMid = 'width: 33%;';
              this.reactStandardsComplaintHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactStandardsComplaintLow = 'width: 33%;';
              this.reactStandardsComplaintMid = 'width: 33%;';
              this.reactStandardsComplaintHigh = 'width: 34%;';
            }
          }
        }
        else if (currentFramework === "Vue")
        {
          if (currentCriteria === "scalability")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueScalabilityLow = 'width: 33%;';
              this.vueScalabilityMid = 'height: 0%;';
              this.vueScalabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueScalabilityLow = 'width: 33%;';
              this.vueScalabilityMid = 'width: 33%;';
              this.vueScalabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueScalabilityLow = 'width: 33%;';
              this.vueScalabilityMid = 'width: 33%;';
              this.vueScalabilityHigh = 'width: 34%;';
            }

          }
          else if (currentCriteria === "modularity")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueModularityLow = 'width: 33%;';
              this.vueModularityMid = 'height: 0%;';
              this.vueModularityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueModularityLow = 'width: 33%;';
              this.vueModularityMid = 'width: 33%;';
              this.vueModularityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueModularityLow = 'width: 33%;';
              this.vueModularityMid = 'width: 33%;';
              this.vueModularityHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "backwardsCompatibility")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueBackwardsCompatibilityLow = 'width: 33%;';
              this.vueBackwardsCompatibilityMid = 'height: 0%;';
              this.vueBackwardsCompatibilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueBackwardsCompatibilityLow = 'width: 33%;';
              this.vueBackwardsCompatibilityMid = 'width: 33%;';
              this.vueBackwardsCompatibilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueBackwardsCompatibilityLow = 'width: 33%;';
              this.vueBackwardsCompatibilityMid = 'width: 33%;';
              this.vueBackwardsCompatibilityHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "testability")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueTestabilityLow = 'width: 33%;';
              this.vueTestabilityMid = 'height: 0%;';
              this.vueTestabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueTestabilityLow = 'width: 33%;';
              this.vueTestabilityMid = 'width: 33%;';
              this.vueTestabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueTestabilityLow = 'width: 33%;';
              this.vueTestabilityMid = 'width: 33%;';
              this.vueTestabilityHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "support")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueSupportLow = 'width: 33%;';
              this.vueSupportMid = 'height: 0%;';
              this.vueSupportHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueSupportLow = 'width: 33%;';
              this.vueSupportMid = 'width: 33%;';
              this.vueSupportHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueSupportLow = 'width: 33%;';
              this.vueSupportMid = 'width: 33%;';
              this.vueSupportHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "future")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueFutureLow = 'width: 33%;';
              this.vueFutureMid = 'height: 0%;';
              this.vueFutureHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueFutureLow = 'width: 33%;';
              this.vueFutureMid = 'width: 33%;';
              this.vueFutureHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueFutureLow = 'width: 33%;';
              this.vueFutureMid = 'width: 33%;';
              this.vueFutureHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "performance")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vuePerformanceLow = 'width: 33%;';
              this.vuePerformanceMid = 'height: 0%;';
              this.vuePerformanceHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vuePerformanceLow = 'width: 33%;';
              this.vuePerformanceMid = 'width: 33%;';
              this.vuePerformanceHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vuePerformanceLow = 'width: 33%;';
              this.vuePerformanceMid = 'width: 33%;';
              this.vuePerformanceHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "customizability")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueCustomizabilityLow = 'width: 33%;';
              this.vueCustomizabilityMid = 'height: 0%;';
              this.vueCustomizabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueCustomizabilityLow = 'width: 33%;';
              this.vueCustomizabilityMid = 'width: 33%;';
              this.vueCustomizabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueCustomizabilityLow = 'width: 33%;';
              this.vueCustomizabilityMid = 'width: 33%;';
              this.vueCustomizabilityHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "readability")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueReadabilityLow = 'width: 33%;';
              this.vueReadabilityMid = 'height: 0%;';
              this.vueReadabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueReadabilityLow = 'width: 33%;';
              this.vueReadabilityMid = 'width: 33%;';
              this.vueReadabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueReadabilityLow = 'width: 33%;';
              this.vueReadabilityMid = 'width: 33%;';
              this.vueReadabilityHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "frameworkSize")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueFrameworkSizeLow = 'width: 33%;';
              this.vueFrameworkSizeMid = 'height: 0%;';
              this.vueFrameworkSizeHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueFrameworkSizeLow = 'width: 33%;';
              this.vueFrameworkSizeMid = 'width: 33%;';
              this.vueFrameworkSizeHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueFrameworkSizeLow = 'width: 33%;';
              this.vueFrameworkSizeMid = 'width: 33%;';
              this.vueFrameworkSizeHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "timeInHand")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueTimeInHandLow = 'width: 33%;';
              this.vueTimeInHandMid = 'height: 0%;';
              this.vueTimeInHandHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueTimeInHandLow = 'width: 33%;';
              this.vueTimeInHandMid = 'width: 33%;';
              this.vueTimeInHandHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueTimeInHandLow = 'width: 33%;';
              this.vueTimeInHandMid = 'width: 33%;';
              this.vueTimeInHandHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "languageES6")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueLanguageLow = 'width: 33%;';
              this.vueLanguageMid = 'height: 0%;';
              this.vueLanguageHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueLanguageLow = 'width: 33%;';
              this.vueLanguageMid = 'width: 33%;';
              this.vueLanguageHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueLanguageLow = 'width: 33%;';
              this.vueLanguageMid = 'width: 33%;';
              this.vueLanguageHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "languageTypeScript")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueLanguageLow = 'width: 33%;';
              this.vueLanguageMid = 'height: 0%;';
              this.vueLanguageHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueLanguageLow = 'width: 33%;';
              this.vueLanguageMid = 'width: 33%;';
              this.vueLanguageHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueLanguageLow = 'width: 33%;';
              this.vueLanguageMid = 'width: 33%;';
              this.vueLanguageHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "appSize")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueAppSizeLow = 'width: 33%;';
              this.vueAppSizeMid = 'height: 0%;';
              this.vueAppSizeHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueAppSizeLow = 'width: 33%;';
              this.vueAppSizeMid = 'width: 33%;';
              this.vueAppSizeHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueAppSizeLow = 'width: 33%;';
              this.vueAppSizeMid = 'width: 33%;';
              this.vueAppSizeHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "learningCurve")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueLearningCurveLow = 'width: 33%;';
              this.vueLearningCurveMid = 'height: 0%;';
              this.vueLearningCurveHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueLearningCurveLow = 'width: 33%;';
              this.vueLearningCurveMid = 'width: 33%;';
              this.vueLearningCurveHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueLearningCurveLow = 'width: 33%;';
              this.vueLearningCurveMid = 'width: 33%;';
              this.vueLearningCurveHigh = 'width: 34%;';
            }
          }
          else if (currentCriteria === "standardsComplaint")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueStandardsComplaintLow = 'width: 33%;';
              this.vueStandardsComplaintMid = 'height: 0%;';
              this.vueStandardsComplaintHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueStandardsComplaintLow = 'width: 33%;';
              this.vueStandardsComplaintMid = 'width: 33%;';
              this.vueStandardsComplaintHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueStandardsComplaintLow = 'width: 33%;';
              this.vueStandardsComplaintMid = 'width: 33%;';
              this.vueStandardsComplaintHigh = 'width: 34%;';
            }
          }
        }
      },

      setMeanTotalScore: function (maxCriteriaScore, selectedLanguage)
      {
        let fdParent = this.frameworksData;
        let localScoreSum;
        let counter;

        for (let keyParent in fdParent)
        {
          counter = 0;
          localScoreSum = 0;

          if (fdParent.hasOwnProperty(keyParent))
          {
            let fdChild = fdParent[keyParent];

            for (let keyChild in fdChild)
            {
              if (fdChild.hasOwnProperty(keyChild))
              {
                let fdSubChild = fdChild[keyChild];

                counter++;

                if((keyChild.search('language') !== -1) && ((keyChild.replace(/language/i, '')) !== selectedLanguage))
                {
                  continue;
                }

                if(counter <= this.totalCriteria)
                {
                  localScoreSum += fdSubChild['score'];
                }
              }
            }

            fdChild['meanTotalScore'] = localScoreSum / this.totalCriteria;
            fdChild['totalPercentage'] = Math.round((fdChild['meanTotalScore'] / maxCriteriaScore) * 100);

            if(keyParent === "Angular")
            {
              this.totalPercentageAngular = fdChild['totalPercentage'];
            }
            else if(keyParent === "React")
            {
              this.totalPercentageReact = fdChild['totalPercentage'];
            }
            else if(keyParent === "Vue")
            {
              this.totalPercentageVue = fdChild['totalPercentage'];
            }

          }
        }
      },

      calculateGoalMet: function (framework, selectedCriteria, userSelection, criteriaStrength)
      {
        let criteriaGoalMet;

        if ((userSelection === "Not Important") || (userSelection === "No Time Constraint") || (userSelection === "Small"))
        {
          criteriaGoalMet = 1;
        }
        else if ((userSelection === "Moderately Important") || (userSelection === "Routine") || (userSelection === "Medium"))
        {
          if (criteriaStrength === "Not Available")
          {
            criteriaGoalMet = 1;
          }
          else if (criteriaStrength === "Partially Available")
          {
            criteriaGoalMet = 2;
          }
          else if (criteriaStrength === "Available")
          {
            criteriaGoalMet = 2;
          }
        }
        else if ((userSelection === "Very Important") || (userSelection === "Urgent") || (userSelection === "ES6") || (userSelection === "TypeScript") || (userSelection === "Big"))
        {
          if (criteriaStrength === "Not Available")
          {
            criteriaGoalMet = 1;
          }
          else if (criteriaStrength === "Partially Available")
          {
            criteriaGoalMet = 2;
          }
          else if (criteriaStrength === "Available")
          {
            criteriaGoalMet = 3;
          }
        }

        return criteriaGoalMet;

      },

      getWeightPerCriteria: function (totalNumberOfCriteria) {
        return 100 / totalNumberOfCriteria;
      },

      clearConsole: function () {
        if (typeof console._commandLineAPI !== 'undefined') {
          console.API = console._commandLineAPI; //chrome
        } else if (typeof console._inspectorCommandLineAPI !== 'undefined') {
          console.API = console._inspectorCommandLineAPI; //Safari
        } else if (typeof console.clear !== 'undefined') {
          console.API = console;
        }
        console.API.clear();
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

        this.clearFormFields();

      },

      clearFormFields: function () {
        this.recommendedFrameworkByUser = '';
        this.emailFormOptionalMessage = '';
      },

      checkFormStatus: function () {
        if(this.formEdited) {
          $("#clearFormConfirmationModal").modal('show');
        }
      },

      clearForm: function (count) {
        Object.assign(this.$data, this.$options.data());
        count++;

        if(count < 2)
        {
          let that = this;
          setTimeout(function () {
            that.clearForm(count);
            console.log("akshdioa sdiouh aiosuh dioauh iosuhda")
          }, 500);
        }

        $('.clear-data').addClass('clear-button-disabled');
        $('.clear-data-mobile').addClass('clear-button-disabled');
        this.formEdited = false;
        $("#clearFormConfirmationModal").modal('hide');
      },

//      generateReport: function () {
//                let PDFDocument = require('pdfkit');
//                let blobStream = require('blob-stream');
//
//                // create a document and pipe to a blob
//                let doc = new PDFDocument();
//                let stream = doc.pipe(blobStream());
//
//// draw some text
//                doc.fontSize(25)
//                    .text('Here is some vector graphics...', 100, 80);
//
//// some vector graphics
//                doc.save()
//                    .moveTo(100, 150)
//                    .lineTo(100, 250)
//                    .lineTo(200, 250)
//                    .fill("#FF3300");
//
//                doc.circle(280, 200, 50)
//                    .fill("#6600FF");
//
//// an SVG path
//                doc.scale(0.6)
//                    .translate(470, 130)
//                    .path('M 250,75 L 323,301 131,161 369,161 177,301 z')
//                    .fill('red', 'even-odd')
//                    .restore();
//
//// and some justified text wrapped into columns
//                doc.text('And here is some wrapped text...', 100, 300)
//                    .font('Times-Roman', 13)
//                    .moveDown()
//                    .text(lorem, {
//                        width: 412,
//                        align: 'justify',
//                        indent: 30,
//                        columns: 2,
//                        height: 300,
//                        ellipsis: true
//                    });
//
//// end and display the document in the iframe to the right
//                doc.end();
//                stream.on('finish', function() {
//                    iframe.src = stream.toBlobURL('application/pdf');
//                });
//      }

    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>

  .whole-page
  {
    width: 95%;
    margin: 0 auto;
    font-family: 'Quicksand', sans-serif;
    letter-spacing: 2px;
  }

  .total-percentage
  {
    float: right;
    color: darkgreen;
    cursor: default;
    pointer-events: none;
  }

  .criteria-description-in-tooltip
  {
    color: darkgray;
    margin: 10px 0 0 -15px;
    cursor: default;
    font-size: medium;
  }

  .tooltipster-sidetip.tooltipster-shadow.tooltipster-shadow-customized .tooltipster-content {
    font-family: 'Quicksand', sans-serif;
    letter-spacing: 1px;
    line-height: 1.5em;
  }

  .table>tbody>tr>td, .table>tbody>tr>th, .table>tfoot>tr>td, .table>tfoot>tr>th, .table>thead>tr>td, .table>thead>tr>th
  {
    color: #595959;
  }

  table.collapse.in {
    display: table;
  }

  .tooltip_templates { display: none; }

  .panel-heading a{
    text-decoration: none;
    color: deepskyblue;
  }

  .progress
  {
    margin-bottom: 0;
  }

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

  .form-group {
    margin-bottom: 16px;
    color: #595959;
  }

  .optional-message
  {
    font-size: smaller;
    font-weight: lighter;
    font-style: italic;
  }

  .criteria-options-meaning
  {
    color: black;
    font-style: italic;
  }

  .important-note-about-total-percentage
  {
    margin-bottom: 75px;
  }

  .important-note
  {
    margin-left: 15px;
    font-size: 14px;
    letter-spacing: 1.5px;
  }

  .important-note-title
  {
    font-size: 16px;
    text-decoration: underline;
    text-decoration-color: cornflowerblue;
  }

  .form-horizontal .control-label{
    text-align:left;
  }

  select{
    font-family: 'Quicksand', sans-serif;
    letter-spacing: 2px;
  }

  select option:disabled
  {
    color: lightgrey;
    font-style: italic;
  }

  .floating-form {
    position: fixed;
    transform: rotate(-90deg);
    right: -32px;
    top: 140px;
    padding: 10px 10px 5px 10px;
    letter-spacing: 2px;
    text-shadow: 1px 1px 1px rgba(0, 0, 0, 0.43);
    cursor: pointer;
    border-radius: 5px 5px 0px 0px;
    background: linear-gradient(to bottom,#2D77A2 5%,deepskyblue 100%);
  }

  .contact-opener {
    color: #fff;
  }

  .floating-form a:hover, .floating-form a:focus
  {
    color: #fff;
    text-decoration: none;
    cursor: pointer;
  }

  #footer {
    display: none;
  }

  .git-link
  {
    text-decoration: none;
    color: black;
    font-size: 18px;
  }

  #footer a:hover, #footer a:focus
  {
    text-decoration: none;
    color: deepskyblue;
  }

  @media screen and (max-width: 767px){
    .floating-form {
      display: none;
    }

    .recommend-framework-mobile
    {
      width: 70%;
    }

    #footer {
      display: flex;
      flex-direction: column;
      justify-content: center;
      height: 50px;
      background: ghostwhite;
      width: 100%;
      opacity: .5;
      text-align: center;
    }

  }

</style>
