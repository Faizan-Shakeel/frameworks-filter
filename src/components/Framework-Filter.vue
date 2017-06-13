<template>

  <div class="filter-container">

    <div class="tooltip_templates">
      <span id="check-individual-results">
        <p>
          Please note that 'Total Percentage' shows the overall result, which doesn't necessarily mean that the higher the percentage the higher the suitability.
        </p>
        <p>
          Please check individual results for most important criteria for your project.
        </p>
      </span>

      <span id="info-scalability">
        <p>
          Please note that 'Total Percentage' shows the overall result, which doesn't necessarily mean that the higher the percentage the higher the suitability.
        </p>
        <p>
          Please check individual results for most important criteria for your project.
        </p>
      </span>

      <span id="info-modularity">
        <p>
          Please note that 'Total Percentage' shows the overall result, which doesn't necessarily mean that the higher the percentage the higher the suitability.
        </p>
        <p>
          Please check individual results for most important criteria for your project.
        </p>
      </span>

      <span id="info-backwards-compatibility">
        <p>
          Please note that 'Total Percentage' shows the overall result, which doesn't necessarily mean that the higher the percentage the higher the suitability.
        </p>
        <p>
          Please check individual results for most important criteria for your project.
        </p>
      </span>

      <span id="info-testability">
        <p>
          Please note that 'Total Percentage' shows the overall result, which doesn't necessarily mean that the higher the percentage the higher the suitability.
        </p>
        <p>
          Please check individual results for most important criteria for your project.
        </p>
      </span>

      <span id="info-support">
        <p>
          Please note that 'Total Percentage' shows the overall result, which doesn't necessarily mean that the higher the percentage the higher the suitability.
        </p>
        <p>
          Please check individual results for most important criteria for your project.
        </p>
      </span>

      <span id="info-future">
        <p>
          Please note that 'Total Percentage' shows the overall result, which doesn't necessarily mean that the higher the percentage the higher the suitability.
        </p>
        <p>
          Please check individual results for most important criteria for your project.
        </p>
      </span>

      <span id="info-performance">
        <p>
          Please note that 'Total Percentage' shows the overall result, which doesn't necessarily mean that the higher the percentage the higher the suitability.
        </p>
        <p>
          Please check individual results for most important criteria for your project.
        </p>
      </span>

      <span id="info-customizability">
        <p>
          Please note that 'Total Percentage' shows the overall result, which doesn't necessarily mean that the higher the percentage the higher the suitability.
        </p>
        <p>
          Please check individual results for most important criteria for your project.
        </p>
      </span>

      <span id="info-readability">
        <p>
          Please note that 'Total Percentage' shows the overall result, which doesn't necessarily mean that the higher the percentage the higher the suitability.
        </p>
        <p>
          Please check individual results for most important criteria for your project.
        </p>
      </span>

      <span id="info-framework-size">
        <p>
          Please note that 'Total Percentage' shows the overall result, which doesn't necessarily mean that the higher the percentage the higher the suitability.
        </p>
        <p>
          Please check individual results for most important criteria for your project.
        </p>
      </span>

      <span id="info-time-in-hand">
        <p>
          Please note that 'Total Percentage' shows the overall result, which doesn't necessarily mean that the higher the percentage the higher the suitability.
        </p>
        <p>
          Please check individual results for most important criteria for your project.
        </p>
      </span>

      <span id="info-language">
        <p>
          Please note that 'Total Percentage' shows the overall result, which doesn't necessarily mean that the higher the percentage the higher the suitability.
        </p>
        <p>
          Please check individual results for most important criteria for your project.
        </p>
      </span>

      <span id="info-app-size">
        <p>
          Please note that 'Total Percentage' shows the overall result, which doesn't necessarily mean that the higher the percentage the higher the suitability.
        </p>
        <p>
          Please check individual results for most important criteria for your project.
        </p>
      </span>

      <span id="info-learning-curve">
        <p>
          Please note that 'Total Percentage' shows the overall result, which doesn't necessarily mean that the higher the percentage the higher the suitability.
        </p>
        <p>
          Please check individual results for most important criteria for your project.
        </p>
      </span>

      <span id="info-standards-complaint">
        <p>
          Please note that 'Total Percentage' shows the overall result, which doesn't necessarily mean that the higher the percentage the higher the suitability.
        </p>
        <p>
          Please check individual results for most important criteria for your project.
        </p>
      </span>

      <!--<span id="info-architecture">-->
      <!--<p>-->
      <!--Please note that 'Total Percentage' shows the overall result, which doesn't necessarily mean that the higher the percentage the higher the suitability.-->
      <!--</p>-->
      <!--<p>-->
      <!--Please check individual results for most important criteria for your project.-->
      <!--</p>-->
      <!--</span>-->
    </div>

    <nav class="navbar navbar-default navbar-static-top">
      <div class="container-fluid">
        <!-- Brand and toggle get grouped for better mobile display -->
        <div class="navbar-header">
          <a class="navbar-brand" href="#">Framework Filter</a>
        </div>

        <!-- Collect the nav links, forms, and other content for toggling -->
        <div class="" id="bs-example-navbar-collapse-1">
          <ul class="nav navbar-nav navbar-right">
            <li class=""><a href="#" data-toggle="modal" data-target="#myModal">Recommend Framework</a></li>
          </ul>
        </div><!-- /.navbar-collapse -->
      </div>
    </nav>

    <!-- Modal -->
    <div class="modal fade" id="myModal" tabindex="-1" role="dialog" aria-labelledby="myModalLabel" data-backdrop="static" aria-hidden="true">
      <div class="modal-dialog" role="document">
        <div class="modal-content">
          <div class="modal-header">
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
            <h4 class="modal-title text-center" id="myModalLabel">Recommend Framework for Comparison</h4>
          </div>
          <form action="https://formspree.io/faizan.sg@gmail.com" method="post">
            <div class="modal-body">
              <div class="form-group">
                <label for="frameworkName">Framework Name</label>
                <input v-model="recommendedFrameworkByUser" type="text" class="form-control" id="frameworkName" placeholder="Framework Name" name="Framework Name" required>
              </div>
              <div class="form-group">
                <label for="optionalMessage">Message (Optional)</label>
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

    <div class="row whole-page">
      <div class="col-sm-6 col-md-6 col-lg-6">
        <form class="">
          <div class="form-group">
            <label for="scalability">Scalability</label>
            <span class="glyphicon glyphicon-info-sign total-percentage-notification tooltips" data-tooltip-content="#info-scalability"></span>
            <select v-model="scalability" class="form-control" id="scalability" v-on:change="frameworkFilter('scalability', scalability)">
              <option>Not Important</option>
              <option>Moderately Important</option>
              <option>Very Important</option>
            </select>
          </div>
          <div class="form-group">
            <label for="modularity">Modularity</label>
            <span class="glyphicon glyphicon-info-sign total-percentage-notification tooltips" data-tooltip-content="#info-modularity"></span>
            <select v-model="modularity" class="form-control" id="modularity" v-on:change="frameworkFilter('modularity', modularity)">
              <option>Not Important</option>
              <option>Moderately Important</option>
              <option>Very Important</option>
            </select>
          </div>
          <div class="form-group">
            <label for="backwardscompatibility">Backwards Compatibility</label>
            <span class="glyphicon glyphicon-info-sign total-percentage-notification tooltips" data-tooltip-content="#info-backwards-compatibility"></span>
            <select v-model="backwardsCompatibility" class="form-control" id="backwardscompatibility" v-on:change="frameworkFilter('backwardsCompatibility', backwardsCompatibility)">
              <option>Not Important</option>
              <option>Moderately Important</option>
              <option>Very Important</option>
            </select>
          </div>
          <div class="form-group">
            <label for="testability">Testability</label>
            <span class="glyphicon glyphicon-info-sign total-percentage-notification tooltips" data-tooltip-content="#info-testability"></span>
            <select v-model="testability" class="form-control" id="testability" v-on:change="frameworkFilter('testability', testability)">
              <option>Not Important</option>
              <option>Moderately Important</option>
              <option>Very Important</option>
            </select>
          </div>
          <div class="form-group">
            <label for="support">Support</label>
            <span class="glyphicon glyphicon-info-sign total-percentage-notification tooltips" data-tooltip-content="#info-support"></span>
            <select v-model="support" class="form-control" id="support" v-on:change="frameworkFilter('support', support)">
              <option>Not Important</option>
              <option>Moderately Important</option>
              <option>Very Important</option>
            </select>
          </div>
          <div class="form-group">
            <label for="future">Future</label>
            <span class="glyphicon glyphicon-info-sign total-percentage-notification tooltips" data-tooltip-content="#info-future"></span>
            <select v-model="future" class="form-control" id="future" v-on:change="frameworkFilter('future', future)">
              <option>Not Important</option>
              <option>Moderately Important</option>
              <option>Very Important</option>
            </select>
          </div>
          <div class="form-group">
            <label for="performance">Performance</label>
            <span class="glyphicon glyphicon-info-sign total-percentage-notification tooltips" data-tooltip-content="#info-performance"></span>
            <select v-model="performance" class="form-control" id="performance" v-on:change="frameworkFilter('performance', performance)">
              <option>Not Important</option>
              <option>Moderately Important</option>
              <option>Very Important</option>
            </select>
          </div>
          <div class="form-group">
            <label for="customizability">Customizability</label>
            <span class="glyphicon glyphicon-info-sign total-percentage-notification tooltips" data-tooltip-content="#info-customizability"></span>
            <select v-model="customizability" class="form-control" id="customizability" v-on:change="frameworkFilter('customizability', customizability)">
              <option>Not Important</option>
              <option>Moderately Important</option>
              <option>Very Important</option>
            </select>
          </div>
          <div class="form-group">
            <label for="readability">Readability</label>
            <span class="glyphicon glyphicon-info-sign total-percentage-notification tooltips" data-tooltip-content="#info-readability"></span>
            <select v-model="readability" class="form-control" id="readability" v-on:change="frameworkFilter('readability', readability)">
              <option>Not Important</option>
              <option>Moderately Important</option>
              <option>Very Important</option>
            </select>
          </div>
          <div class="form-group">
            <label for="frameworkSize">Framework Size</label>
            <span class="glyphicon glyphicon-info-sign total-percentage-notification tooltips" data-tooltip-content="#info-framework-size"></span>
            <select v-model="frameworkSize" class="form-control" id="frameworkSize" v-on:change="frameworkFilter('frameworkSize', frameworkSize)">
              <option>Not Important</option>
              <option>Moderately Important</option>
              <option>Very Important</option>
            </select>
          </div>
          <div class="form-group">
            <label for="timeInHand">Time in hand</label>
            <span class="glyphicon glyphicon-info-sign total-percentage-notification tooltips" data-tooltip-content="#info-time-in-hand"></span>
            <select v-model="timeInHand" class="form-control" id="timeInHand" v-on:change="frameworkFilter('timeInHand', timeInHand)">
              <option>No Time Constraint</option>
              <option>Routine</option>
              <option>Urgent</option>
            </select>
          </div>
          <div class="form-group">
            <label for="language">Language</label>
            <span class="glyphicon glyphicon-info-sign total-percentage-notification tooltips" data-tooltip-content="#info-language"></span>
            <select v-model="language" class="form-control" id="language" v-on:change="frameworkFilter('language'+language, language)">
              <option>ES6</option>
              <option>TypeScript</option>
            </select>
          </div>
          <div class="form-group">
            <label for="appSize">App Size</label>
            <span class="glyphicon glyphicon-info-sign total-percentage-notification tooltips" data-tooltip-content="#info-app-size"></span>
            <select v-model="appSize" class="form-control" id="appSize" v-on:change="frameworkFilter('appSize', appSize)">
              <option>Small</option>
              <option>Medium</option>
              <option>Big</option>
            </select>
          </div>
          <div class="form-group">
            <label for="learningCurve">Learning Curve</label>
            <span class="glyphicon glyphicon-info-sign total-percentage-notification tooltips" data-tooltip-content="#info-learning-curve"></span>
            <select v-model="learningCurve" class="form-control" id="learningCurve" v-on:change="frameworkFilter('learningCurve', learningCurve)">
              <option>Not Important</option>
              <option>Moderately Important</option>
              <option>Very Important</option>
            </select>
          </div>
          <div class="form-group">
            <label for="standardsComplaint">Standards Complaint</label>
            <span class="glyphicon glyphicon-info-sign total-percentage-notification tooltips" data-tooltip-content="#info-standards-complaint"></span>
            <select v-model="standardsComplaint" class="form-control" id="standardsComplaint" v-on:change="frameworkFilter('standardsComplaint', standardsComplaint)">
              <option>Not Important</option>
              <option>Moderately Important</option>
              <option>Very Important</option>
            </select>
          </div>
          <!--<div class="form-group">-->
          <!--<label for="architecture">Architecture</label>-->
          <!--<span class="glyphicon glyphicon-info-sign total-percentage-notification tooltips" data-tooltip-content="#info-architecture"></span>-->
          <!--<select v-model="architecture" class="form-control" id="architecture" v-on:change="frameworkFilter('architecture', architecture)">-->
          <!--<option>Not Important</option>-->
          <!--<option>Moderately Important</option>-->
          <!--<option>Very Important</option>-->
          <!--</select>-->
          <!--</div>-->
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
                  <!--<span class="glyphicon glyphicon-info-sign total-percentage-notification tooltips" title="Please note that 'Total Percentage' shows the overall result, which doesn't necessarily mean that the higher the percentage the higher the suitability. Please check individual results for most important criteria for your project."></span>-->
                  <span class="glyphicon glyphicon-info-sign total-percentage-notification tooltips" data-tooltip-content="#check-individual-results"></span>
                </a>
              </h4>
            </div>
            <div id="collapseOne" class="panel-collapse collapse in" role="tabpanel" aria-labelledby="headingOne">
              <div class="panel-body">
                <table class="table table-striped table-hover">
                  <tbody>
                  <tr>
                    <th>Scalability</th>
                    <td class="col-xs-1 col-sm-2 col-md-5 col-lg-3">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="angularScalabilityLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="angularScalabilityMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="angularScalabilityHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Modularity</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="angularModularityLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="angularModularityMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="angularModularityHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Backwards Compatibility</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="angularBackwardsCompatibilityLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="angularBackwardsCompatibilityMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="angularBackwardsCompatibilityHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Testability</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="angularTestabilityLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="angularTestabilityMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="angularTestabilityHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Support</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="angularSupportLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="angularSupportMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="angularSupportHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Future</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="angularFutureLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="angularFutureMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="angularFutureHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Performance</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="angularPerformanceLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="angularPerformanceMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="angularPerformanceHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Customizability</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="angularCustomizabilityLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="angularCustomizabilityMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="angularCustomizabilityHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Readability</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="angularReadabilityLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="angularReadabilityMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="angularReadabilityHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Framework Size</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="angularFrameworkSizeLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="angularFrameworkSizeMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="angularFrameworkSizeHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Time in hand</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="angularTimeInHandLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="angularTimeInHandMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="angularTimeInHandHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Language</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="angularLanguageLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="angularLanguageMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="angularLanguageHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>App Size</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="angularAppSizeLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="angularAppSizeMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="angularAppSizeHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Learning Curve</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="angularLearningCurveLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="angularLearningCurveMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="angularLearningCurveHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Standards Complaint</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="angularStandardsComplaintLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="angularStandardsComplaintMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="angularStandardsComplaintHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <!--<tr>-->
                  <!--<th>Architecture</th>-->
                  <!--<td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">-->
                  <!--{{this.angularArchitecturePercentage}}%-->
                  <!--</td>-->
                  <!--</tr>-->
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
                    <td class="col-xs-1 col-sm-2 col-md-5 col-lg-3">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="reactScalabilityLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="reactScalabilityMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="reactScalabilityHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Modularity</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="reactModularityLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="reactModularityMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="reactModularityHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Backwards Compatibility</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="reactBackwardsCompatibilityLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="reactBackwardsCompatibilityMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="reactBackwardsCompatibilityHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Testability</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="reactTestabilityLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="reactTestabilityMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="reactTestabilityHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Support</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="reactSupportLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="reactSupportMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="reactSupportHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Future</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="reactFutureLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="reactFutureMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="reactFutureHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Performance</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="reactPerformanceLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="reactPerformanceMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="reactPerformanceHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Customizability</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="reactCustomizabilityLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="reactCustomizabilityMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="reactCustomizabilityHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Readability</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="reactReadabilityLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="reactReadabilityMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="reactReadabilityHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Framework Size</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="reactFrameworkSizeLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="reactFrameworkSizeMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="reactFrameworkSizeHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Time in hand</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="reactTimeInHandLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="reactTimeInHandMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="reactTimeInHandHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Language</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="reactLanguageLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="reactLanguageMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="reactLanguageHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>App Size</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="reactAppSizeLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="reactAppSizeMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="reactAppSizeHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Learning Curve</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="reactLearningCurveLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="reactLearningCurveMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="reactLearningCurveHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Standards Complaint</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="reactStandardsComplaintLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="reactStandardsComplaintMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="reactStandardsComplaintHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <!--<tr>-->
                  <!--<th>Architecture</th>-->
                  <!--<td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">-->
                  <!--{{this.reactArchitecturePercentage}}%-->
                  <!--</td>-->
                  <!--</tr>-->
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
                    <td class="col-xs-1 col-sm-2 col-md-5 col-lg-3">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="vueScalabilityLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="vueScalabilityMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="vueScalabilityHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Modularity</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="vueModularityLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="vueModularityMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="vueModularityHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Backwards Compatibility</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="vueBackwardsCompatibilityLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="vueBackwardsCompatibilityMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="vueBackwardsCompatibilityHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Testability</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="vueTestabilityLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="vueTestabilityMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="vueTestabilityHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Support</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="vueSupportLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="vueSupportMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="vueSupportHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Future</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="vueFutureLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="vueFutureMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="vueFutureHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Performance</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="vuePerformanceLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="vuePerformanceMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="vuePerformanceHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Customizability</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="vueCustomizabilityLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="vueCustomizabilityMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="vueCustomizabilityHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Readability</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="vueReadabilityLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="vueReadabilityMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="vueReadabilityHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Framework Size</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="vueFrameworkSizeLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="vueFrameworkSizeMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="vueFrameworkSizeHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Time in hand</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="vueTimeInHandLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="vueTimeInHandMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="vueTimeInHandHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Language</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="vueLanguageLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="vueLanguageMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="vueLanguageHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>App Size</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="vueAppSizeLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="vueAppSizeMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="vueAppSizeHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Learning Curve</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="vueLearningCurveLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="vueLearningCurveMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="vueLearningCurveHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Standards Complaint</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100" :style="vueStandardsComplaintLow">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" :style="vueStandardsComplaintMid">
                        </div>
                      </div>
                      <div class="progress progress-bar-vertical">
                        <div class="progress-bar progress-bar-success progress-bar-striped active" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100" :style="vueStandardsComplaintHigh">
                        </div>
                      </div>
                    </td>
                  </tr>
                  <!--<tr>-->
                  <!--<th>Architecture</th>-->
                  <!--<td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">-->
                  <!--{{this.reactArchitecturePercentage}}%-->
                  <!--</td>-->
                  <!--</tr>-->
                  </tbody>
                </table>

              </div>
            </div>
          </div>
        </div>
      </div>

      <!--Accordion End-->

    </div>
  </div>

</template>

<script>
  export default {
    beforeMount(){

      $(function () {
        $('.tooltips').tooltipster({
//          theme: 'tooltipster-shadow',
          theme: ['tooltipster-shadow', 'tooltipster-shadow-customized'],
          delay: 0,
          maxWidth: 500,
          side: "left"
        });
      })
    },

    name: 'hello',
    data () {
      return {
        recommendedFrameworkByUser: this.recommendedFrameworkByUser,
        emailFormOptionalMessage: this.emailFormOptionalMessage,
        scalability: this.scalability,
        modularity: this.modularity,
        backwardsCompatibility: this.backwardsCompatibility,
        testability: this.testability,
        support: this.support,
        future: this.future,
        performance: this.performance,
        customizability: this.customizability,
        readability: this.readability,
        frameworkSize: this.frameworkSize,
        timeInHand: this.timeInHand,
        language: this.language,
        appSize: this.appSize,
        learningCurve: this.learningCurve,
        standardsComplaint: this.standardsComplaint,
//        architecture: this.architecture,

        totalCriteria: 16,
        totalPercentageAngular: 0,
        totalPercentageReact: 0,
        totalPercentageVue: 0,

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
//        angularArchitecturePercentage: 0,

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
//        reactArchitecturePercentage: 0,


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
//        vueArchitecturePercentage: 0,

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
        angularSupportMid: this.angularSupportLow,
        angularSupportHigh: this.angularSupportLow,
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
        reactSupportMid: this.reactSupportLow,
        reactSupportHigh: this.reactSupportLow,
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
        vueSupportMid: this.vueSupportLow,
        vueSupportHigh: this.vueSupportLow,
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
        this.clearConsole();
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

                  fdSubChild["goalMet"] = this.calculateGoalMet(framework, selectedCriteria, userSelection, fdSubChild);
                  fdSubChild["score"] = fdSubChild["goalMet"] * weightPerCriteria;
                  fdSubChild["percentage"] = Math.round(fdSubChild["score"] / (maxCriteriaScore) * 100);
                  this.setIndividualPercentage(framework, selectedCriteria, fdSubChild["percentage"]);
                }
              }
            }
          }
        }

        this.setMeanTotalScore(maxCriteriaScore, this.language);
      },

      setIndividualPercentage: function (currentFramework, currentCriteria, currentCriteriaPercentage) {

        if (currentFramework === "Angular")
        {
          if (currentCriteria === "scalability")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularScalabilityLow = 'height: 33%;';
              this.angularScalabilityMid = 'height: 0%;';
              this.angularScalabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularScalabilityLow = 'height: 33%;';
              this.angularScalabilityMid = 'height: 66%;';
              this.angularScalabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularScalabilityLow = 'height: 33%;';
              this.angularScalabilityMid = 'height: 66%;';
              this.angularScalabilityHigh = 'height: 100%;';
            }

          }
          else if (currentCriteria === "modularity")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularModularityLow = 'height: 33%;';
              this.angularModularityMid = 'height: 0%;';
              this.angularModularityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularModularityLow = 'height: 33%;';
              this.angularModularityMid = 'height: 66%;';
              this.angularModularityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularModularityLow = 'height: 33%;';
              this.angularModularityMid = 'height: 66%;';
              this.angularModularityHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "backwardsCompatibility")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularBackwardsCompatibilityLow = 'height: 33%;';
              this.angularBackwardsCompatibilityMid = 'height: 0%;';
              this.angularBackwardsCompatibilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularBackwardsCompatibilityLow = 'height: 33%;';
              this.angularBackwardsCompatibilityMid = 'height: 66%;';
              this.angularBackwardsCompatibilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularBackwardsCompatibilityLow = 'height: 33%;';
              this.angularBackwardsCompatibilityMid = 'height: 66%;';
              this.angularBackwardsCompatibilityHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "testability")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularTestabilityLow = 'height: 33%;';
              this.angularTestabilityMid = 'height: 0%;';
              this.angularTestabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularTestabilityLow = 'height: 33%;';
              this.angularTestabilityMid = 'height: 66%;';
              this.angularTestabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularTestabilityLow = 'height: 33%;';
              this.angularTestabilityMid = 'height: 66%;';
              this.angularTestabilityHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "support")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularSupportLow = 'height: 33%;';
              this.angularSupportMid = 'height: 0%;';
              this.angularSupportHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularSupportLow = 'height: 33%;';
              this.angularSupportMid = 'height: 66%;';
              this.angularSupportHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularSupportLow = 'height: 33%;';
              this.angularSupportMid = 'height: 66%;';
              this.angularSupportHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "future")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularFutureLow = 'height: 33%;';
              this.angularFutureMid = 'height: 0%;';
              this.angularFutureHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularFutureLow = 'height: 33%;';
              this.angularFutureMid = 'height: 66%;';
              this.angularFutureHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularFutureLow = 'height: 33%;';
              this.angularFutureMid = 'height: 66%;';
              this.angularFutureHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "performance")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularPerformanceLow = 'height: 33%;';
              this.angularPerformanceMid = 'height: 0%;';
              this.angularPerformanceHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularPerformanceLow = 'height: 33%;';
              this.angularPerformanceMid = 'height: 66%;';
              this.angularPerformanceHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularPerformanceLow = 'height: 33%;';
              this.angularPerformanceMid = 'height: 66%;';
              this.angularPerformanceHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "customizability")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularCustomizabilityLow = 'height: 33%;';
              this.angularCustomizabilityMid = 'height: 0%;';
              this.angularCustomizabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularCustomizabilityLow = 'height: 33%;';
              this.angularCustomizabilityMid = 'height: 66%;';
              this.angularCustomizabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularCustomizabilityLow = 'height: 33%;';
              this.angularCustomizabilityMid = 'height: 66%;';
              this.angularCustomizabilityHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "readability")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularReadabilityLow = 'height: 33%;';
              this.angularReadabilityMid = 'height: 0%;';
              this.angularReadabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularReadabilityLow = 'height: 33%;';
              this.angularReadabilityMid = 'height: 66%;';
              this.angularReadabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularReadabilityLow = 'height: 33%;';
              this.angularReadabilityMid = 'height: 66%;';
              this.angularReadabilityHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "frameworkSize")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularFrameworkSizeLow = 'height: 33%;';
              this.angularFrameworkSizeMid = 'height: 0%;';
              this.angularFrameworkSizeHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularFrameworkSizeLow = 'height: 33%;';
              this.angularFrameworkSizeMid = 'height: 66%;';
              this.angularFrameworkSizeHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularFrameworkSizeLow = 'height: 33%;';
              this.angularFrameworkSizeMid = 'height: 66%;';
              this.angularFrameworkSizeHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "timeInHand")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularTimeInHandLow = 'height: 33%;';
              this.angularTimeInHandMid = 'height: 0%;';
              this.angularTimeInHandHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularTimeInHandLow = 'height: 33%;';
              this.angularTimeInHandMid = 'height: 66%;';
              this.angularTimeInHandHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularTimeInHandLow = 'height: 33%;';
              this.angularTimeInHandMid = 'height: 66%;';
              this.angularTimeInHandHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "languageES6")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularLanguageLow = 'height: 33%;';
              this.angularLanguageMid = 'height: 0%;';
              this.angularLanguageHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularLanguageLow = 'height: 33%;';
              this.angularLanguageMid = 'height: 66%;';
              this.angularLanguageHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularLanguageLow = 'height: 33%;';
              this.angularLanguageMid = 'height: 66%;';
              this.angularLanguageHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "languageTypeScript")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularLanguageLow = 'height: 33%;';
              this.angularLanguageMid = 'height: 0%;';
              this.angularLanguageHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularLanguageLow = 'height: 33%;';
              this.angularLanguageMid = 'height: 66%;';
              this.angularLanguageHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularLanguageLow = 'height: 33%;';
              this.angularLanguageMid = 'height: 66%;';
              this.angularLanguageHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "appSize")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularAppSizeLow = 'height: 33%;';
              this.angularAppSizeMid = 'height: 0%;';
              this.angularAppSizeHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularAppSizeLow = 'height: 33%;';
              this.angularAppSizeMid = 'height: 66%;';
              this.angularAppSizeHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularAppSizeLow = 'height: 33%;';
              this.angularAppSizeMid = 'height: 66%;';
              this.angularAppSizeHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "learningCurve")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularLearningCurveLow = 'height: 33%;';
              this.angularLearningCurveMid = 'height: 0%;';
              this.angularLearningCurveHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularLearningCurveLow = 'height: 33%;';
              this.angularLearningCurveMid = 'height: 66%;';
              this.angularLearningCurveHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularLearningCurveLow = 'height: 33%;';
              this.angularLearningCurveMid = 'height: 66%;';
              this.angularLearningCurveHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "standardsComplaint")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.angularStandardsComplaintLow = 'height: 33%;';
              this.angularStandardsComplaintMid = 'height: 0%;';
              this.angularStandardsComplaintHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.angularStandardsComplaintLow = 'height: 33%;';
              this.angularStandardsComplaintMid = 'height: 66%;';
              this.angularStandardsComplaintHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.angularStandardsComplaintLow = 'height: 33%;';
              this.angularStandardsComplaintMid = 'height: 66%;';
              this.angularStandardsComplaintHigh = 'height: 100%;';
            }
          }
        }
        else if (currentFramework === "React")
        {
          if (currentCriteria === "scalability")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactScalabilityLow = 'height: 33%;';
              this.reactScalabilityMid = 'height: 0%;';
              this.reactScalabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactScalabilityLow = 'height: 33%;';
              this.reactScalabilityMid = 'height: 66%;';
              this.reactScalabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactScalabilityLow = 'height: 33%;';
              this.reactScalabilityMid = 'height: 66%;';
              this.reactScalabilityHigh = 'height: 100%;';
            }

          }
          else if (currentCriteria === "modularity")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactModularityLow = 'height: 33%;';
              this.reactModularityMid = 'height: 0%;';
              this.reactModularityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactModularityLow = 'height: 33%;';
              this.reactModularityMid = 'height: 66%;';
              this.reactModularityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactModularityLow = 'height: 33%;';
              this.reactModularityMid = 'height: 66%;';
              this.reactModularityHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "backwardsCompatibility")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactBackwardsCompatibilityLow = 'height: 33%;';
              this.reactBackwardsCompatibilityMid = 'height: 0%;';
              this.reactBackwardsCompatibilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactBackwardsCompatibilityLow = 'height: 33%;';
              this.reactBackwardsCompatibilityMid = 'height: 66%;';
              this.reactBackwardsCompatibilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactBackwardsCompatibilityLow = 'height: 33%;';
              this.reactBackwardsCompatibilityMid = 'height: 66%;';
              this.reactBackwardsCompatibilityHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "testability")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactTestabilityLow = 'height: 33%;';
              this.reactTestabilityMid = 'height: 0%;';
              this.reactTestabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactTestabilityLow = 'height: 33%;';
              this.reactTestabilityMid = 'height: 66%;';
              this.reactTestabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactTestabilityLow = 'height: 33%;';
              this.reactTestabilityMid = 'height: 66%;';
              this.reactTestabilityHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "support")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactSupportLow = 'height: 33%;';
              this.reactSupportMid = 'height: 0%;';
              this.reactSupportHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactSupportLow = 'height: 33%;';
              this.reactSupportMid = 'height: 66%;';
              this.reactSupportHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactSupportLow = 'height: 33%;';
              this.reactSupportMid = 'height: 66%;';
              this.reactSupportHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "future")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactFutureLow = 'height: 33%;';
              this.reactFutureMid = 'height: 0%;';
              this.reactFutureHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactFutureLow = 'height: 33%;';
              this.reactFutureMid = 'height: 66%;';
              this.reactFutureHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactFutureLow = 'height: 33%;';
              this.reactFutureMid = 'height: 66%;';
              this.reactFutureHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "performance")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactPerformanceLow = 'height: 33%;';
              this.reactPerformanceMid = 'height: 0%;';
              this.reactPerformanceHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactPerformanceLow = 'height: 33%;';
              this.reactPerformanceMid = 'height: 66%;';
              this.reactPerformanceHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactPerformanceLow = 'height: 33%;';
              this.reactPerformanceMid = 'height: 66%;';
              this.reactPerformanceHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "customizability")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactCustomizabilityLow = 'height: 33%;';
              this.reactCustomizabilityMid = 'height: 0%;';
              this.reactCustomizabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactCustomizabilityLow = 'height: 33%;';
              this.reactCustomizabilityMid = 'height: 66%;';
              this.reactCustomizabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactCustomizabilityLow = 'height: 33%;';
              this.reactCustomizabilityMid = 'height: 66%;';
              this.reactCustomizabilityHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "readability")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactReadabilityLow = 'height: 33%;';
              this.reactReadabilityMid = 'height: 0%;';
              this.reactReadabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactReadabilityLow = 'height: 33%;';
              this.reactReadabilityMid = 'height: 66%;';
              this.reactReadabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactReadabilityLow = 'height: 33%;';
              this.reactReadabilityMid = 'height: 66%;';
              this.reactReadabilityHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "frameworkSize")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactFrameworkSizeLow = 'height: 33%;';
              this.reactFrameworkSizeMid = 'height: 0%;';
              this.reactFrameworkSizeHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactFrameworkSizeLow = 'height: 33%;';
              this.reactFrameworkSizeMid = 'height: 66%;';
              this.reactFrameworkSizeHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactFrameworkSizeLow = 'height: 33%;';
              this.reactFrameworkSizeMid = 'height: 66%;';
              this.reactFrameworkSizeHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "timeInHand")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactTimeInHandLow = 'height: 33%;';
              this.reactTimeInHandMid = 'height: 0%;';
              this.reactTimeInHandHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactTimeInHandLow = 'height: 33%;';
              this.reactTimeInHandMid = 'height: 66%;';
              this.reactTimeInHandHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactTimeInHandLow = 'height: 33%;';
              this.reactTimeInHandMid = 'height: 66%;';
              this.reactTimeInHandHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "languageES6")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactLanguageLow = 'height: 33%;';
              this.reactLanguageMid = 'height: 0%;';
              this.reactLanguageHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactLanguageLow = 'height: 33%;';
              this.reactLanguageMid = 'height: 66%;';
              this.reactLanguageHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactLanguageLow = 'height: 33%;';
              this.reactLanguageMid = 'height: 66%;';
              this.reactLanguageHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "languageTypeScript")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactLanguageLow = 'height: 33%;';
              this.reactLanguageMid = 'height: 0%;';
              this.reactLanguageHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactLanguageLow = 'height: 33%;';
              this.reactLanguageMid = 'height: 66%;';
              this.reactLanguageHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactLanguageLow = 'height: 33%;';
              this.reactLanguageMid = 'height: 66%;';
              this.reactLanguageHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "appSize")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactAppSizeLow = 'height: 33%;';
              this.reactAppSizeMid = 'height: 0%;';
              this.reactAppSizeHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactAppSizeLow = 'height: 33%;';
              this.reactAppSizeMid = 'height: 66%;';
              this.reactAppSizeHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactAppSizeLow = 'height: 33%;';
              this.reactAppSizeMid = 'height: 66%;';
              this.reactAppSizeHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "learningCurve")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactLearningCurveLow = 'height: 33%;';
              this.reactLearningCurveMid = 'height: 0%;';
              this.reactLearningCurveHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactLearningCurveLow = 'height: 33%;';
              this.reactLearningCurveMid = 'height: 66%;';
              this.reactLearningCurveHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactLearningCurveLow = 'height: 33%;';
              this.reactLearningCurveMid = 'height: 66%;';
              this.reactLearningCurveHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "standardsComplaint")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.reactStandardsComplaintLow = 'height: 33%;';
              this.reactStandardsComplaintMid = 'height: 0%;';
              this.reactStandardsComplaintHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.reactStandardsComplaintLow = 'height: 33%;';
              this.reactStandardsComplaintMid = 'height: 66%;';
              this.reactStandardsComplaintHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.reactStandardsComplaintLow = 'height: 33%;';
              this.reactStandardsComplaintMid = 'height: 66%;';
              this.reactStandardsComplaintHigh = 'height: 100%;';
            }
          }
        }
        else if (currentFramework === "Vue")
        {
          if (currentCriteria === "scalability")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueScalabilityLow = 'height: 33%;';
              this.vueScalabilityMid = 'height: 0%;';
              this.vueScalabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueScalabilityLow = 'height: 33%;';
              this.vueScalabilityMid = 'height: 66%;';
              this.vueScalabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueScalabilityLow = 'height: 33%;';
              this.vueScalabilityMid = 'height: 66%;';
              this.vueScalabilityHigh = 'height: 100%;';
            }

          }
          else if (currentCriteria === "modularity")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueModularityLow = 'height: 33%;';
              this.vueModularityMid = 'height: 0%;';
              this.vueModularityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueModularityLow = 'height: 33%;';
              this.vueModularityMid = 'height: 66%;';
              this.vueModularityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueModularityLow = 'height: 33%;';
              this.vueModularityMid = 'height: 66%;';
              this.vueModularityHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "backwardsCompatibility")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueBackwardsCompatibilityLow = 'height: 33%;';
              this.vueBackwardsCompatibilityMid = 'height: 0%;';
              this.vueBackwardsCompatibilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueBackwardsCompatibilityLow = 'height: 33%;';
              this.vueBackwardsCompatibilityMid = 'height: 66%;';
              this.vueBackwardsCompatibilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueBackwardsCompatibilityLow = 'height: 33%;';
              this.vueBackwardsCompatibilityMid = 'height: 66%;';
              this.vueBackwardsCompatibilityHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "testability")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueTestabilityLow = 'height: 33%;';
              this.vueTestabilityMid = 'height: 0%;';
              this.vueTestabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueTestabilityLow = 'height: 33%;';
              this.vueTestabilityMid = 'height: 66%;';
              this.vueTestabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueTestabilityLow = 'height: 33%;';
              this.vueTestabilityMid = 'height: 66%;';
              this.vueTestabilityHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "support")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueSupportLow = 'height: 33%;';
              this.vueSupportMid = 'height: 0%;';
              this.vueSupportHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueSupportLow = 'height: 33%;';
              this.vueSupportMid = 'height: 66%;';
              this.vueSupportHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueSupportLow = 'height: 33%;';
              this.vueSupportMid = 'height: 66%;';
              this.vueSupportHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "future")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueFutureLow = 'height: 33%;';
              this.vueFutureMid = 'height: 0%;';
              this.vueFutureHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueFutureLow = 'height: 33%;';
              this.vueFutureMid = 'height: 66%;';
              this.vueFutureHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueFutureLow = 'height: 33%;';
              this.vueFutureMid = 'height: 66%;';
              this.vueFutureHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "performance")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vuePerformanceLow = 'height: 33%;';
              this.vuePerformanceMid = 'height: 0%;';
              this.vuePerformanceHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vuePerformanceLow = 'height: 33%;';
              this.vuePerformanceMid = 'height: 66%;';
              this.vuePerformanceHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vuePerformanceLow = 'height: 33%;';
              this.vuePerformanceMid = 'height: 66%;';
              this.vuePerformanceHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "customizability")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueCustomizabilityLow = 'height: 33%;';
              this.vueCustomizabilityMid = 'height: 0%;';
              this.vueCustomizabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueCustomizabilityLow = 'height: 33%;';
              this.vueCustomizabilityMid = 'height: 66%;';
              this.vueCustomizabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueCustomizabilityLow = 'height: 33%;';
              this.vueCustomizabilityMid = 'height: 66%;';
              this.vueCustomizabilityHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "readability")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueReadabilityLow = 'height: 33%;';
              this.vueReadabilityMid = 'height: 0%;';
              this.vueReadabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueReadabilityLow = 'height: 33%;';
              this.vueReadabilityMid = 'height: 66%;';
              this.vueReadabilityHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueReadabilityLow = 'height: 33%;';
              this.vueReadabilityMid = 'height: 66%;';
              this.vueReadabilityHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "frameworkSize")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueFrameworkSizeLow = 'height: 33%;';
              this.vueFrameworkSizeMid = 'height: 0%;';
              this.vueFrameworkSizeHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueFrameworkSizeLow = 'height: 33%;';
              this.vueFrameworkSizeMid = 'height: 66%;';
              this.vueFrameworkSizeHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueFrameworkSizeLow = 'height: 33%;';
              this.vueFrameworkSizeMid = 'height: 66%;';
              this.vueFrameworkSizeHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "timeInHand")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueTimeInHandLow = 'height: 33%;';
              this.vueTimeInHandMid = 'height: 0%;';
              this.vueTimeInHandHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueTimeInHandLow = 'height: 33%;';
              this.vueTimeInHandMid = 'height: 66%;';
              this.vueTimeInHandHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueTimeInHandLow = 'height: 33%;';
              this.vueTimeInHandMid = 'height: 66%;';
              this.vueTimeInHandHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "languageES6")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueLanguageLow = 'height: 33%;';
              this.vueLanguageMid = 'height: 0%;';
              this.vueLanguageHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueLanguageLow = 'height: 33%;';
              this.vueLanguageMid = 'height: 66%;';
              this.vueLanguageHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueLanguageLow = 'height: 33%;';
              this.vueLanguageMid = 'height: 66%;';
              this.vueLanguageHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "languageTypeScript")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueLanguageLow = 'height: 33%;';
              this.vueLanguageMid = 'height: 0%;';
              this.vueLanguageHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueLanguageLow = 'height: 33%;';
              this.vueLanguageMid = 'height: 66%;';
              this.vueLanguageHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueLanguageLow = 'height: 33%;';
              this.vueLanguageMid = 'height: 66%;';
              this.vueLanguageHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "appSize")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueAppSizeLow = 'height: 33%;';
              this.vueAppSizeMid = 'height: 0%;';
              this.vueAppSizeHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueAppSizeLow = 'height: 33%;';
              this.vueAppSizeMid = 'height: 66%;';
              this.vueAppSizeHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueAppSizeLow = 'height: 33%;';
              this.vueAppSizeMid = 'height: 66%;';
              this.vueAppSizeHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "learningCurve")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueLearningCurveLow = 'height: 33%;';
              this.vueLearningCurveMid = 'height: 0%;';
              this.vueLearningCurveHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueLearningCurveLow = 'height: 33%;';
              this.vueLearningCurveMid = 'height: 66%;';
              this.vueLearningCurveHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueLearningCurveLow = 'height: 33%;';
              this.vueLearningCurveMid = 'height: 66%;';
              this.vueLearningCurveHigh = 'height: 100%;';
            }
          }
          else if (currentCriteria === "standardsComplaint")
          {
            if (currentCriteriaPercentage < 40)
            {
              this.vueStandardsComplaintLow = 'height: 33%;';
              this.vueStandardsComplaintMid = 'height: 0%;';
              this.vueStandardsComplaintHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage < 70)
            {
              this.vueStandardsComplaintLow = 'height: 33%;';
              this.vueStandardsComplaintMid = 'height: 66%;';
              this.vueStandardsComplaintHigh = 'height: 0%;';
            }
            else if (currentCriteriaPercentage > 80)
            {
              this.vueStandardsComplaintLow = 'height: 33%;';
              this.vueStandardsComplaintMid = 'height: 66%;';
              this.vueStandardsComplaintHigh = 'height: 100%;';
            }
          }
        }

      },

      setMeanTotalScore: function (maxCriteriaScore, selectedLanguage) {

        let fdParent = this.frameworksData;
        let localScoreSum;
        let counter;
        let str;

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

      calculateGoalMet: function (framework, selectedCriteria, userSelection, selectedCriteriaData) {
        let criteriaStrength = selectedCriteriaData['strength'];
        let criteriaGoalMet = selectedCriteriaData['goalMet'];

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

      sendMail: function (recommendedFrameworkByUser, optionalMessage) {
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

          $("#myModal").modal('hide');
          toastr.success('Thank you for the recommendation.', 'Email Sent', {timeOut: 5000});
        }
        else
        {
          toastr.warning('Please provide a framework name.', 'Required', {timeOut: 5000});
        }

        this.clearFormFields();

      },

      clearFormFields: function () {
        this.recommendedFrameworkByUser = '';
        this.emailFormOptionalMessage = '';
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>

  /*.filter-container*/
  /*{*/
  /*width: 95%;*/
  /*margin: 0 auto;*/
  /*}*/


  .whole-page
  {
    width: 95%;
    margin: 0 auto;
  }

  .total-percentage
  {
    float: right;
    color: darkgreen;
    cursor: default;
  }

  .total-percentage-notification
  {
    float: right;
    color: darkgray;
    margin-right: 10px;
    cursor: default;
    font-size: medium;
  }

  .tooltipster-sidetip.tooltipster-shadow.tooltipster-shadow-customized .tooltipster-content {
    font-size: 16px;
    /*letter-spacing: 1.5px;*/
    line-height: 2em;
  }

  table.collapse.in {
    display: table;
  }

  .tooltip_templates { display: none; }

  .panel-heading a{
    text-decoration: none;
    color: deepskyblue;
  }

  .progress-bar-vertical {
    width: 25px;
    min-height: 44px;
    display: flex;
    align-items: flex-end;
    margin: 0 5px 0 0;
    float: left;
  }

  .progress-bar-vertical .progress-bar {
    width: 100%;
    height: 0;
    -webkit-transition: height 0.6s ease;
    -o-transition: height 0.6s ease;
    transition: height 0.6s ease;
  }

  .table>tbody>tr>td, .table>tbody>tr>th, .table>tfoot>tr>td, .table>tfoot>tr>th, .table>thead>tr>td, .table>thead>tr>th
  {
     vertical-align: middle !important;
  }

</style>
