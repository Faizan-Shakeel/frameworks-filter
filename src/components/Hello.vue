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
        <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
          <ul class="nav navbar-nav navbar-right">
            <li><a href="#" data-toggle="modal" data-target="#myModal">Recommend Framework</a></li>
          </ul>
        </div><!-- /.navbar-collapse -->
      </div>
    </nav>

    <!-- Modal -->
    <div class="modal fade" id="myModal" tabindex="-1" role="dialog" aria-labelledby="myModalLabel" data-backdrop="static">
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
                  <input v-model="recommendedFrameworkByUser" type="text" class="form-control" id="frameworkName" placeholder="Framework Name" name="Framework Name">
                </div>
                <div class="form-group">
                  <label for="optionalMessage">Message (Optional)</label>
                  <textarea v-model="emailFormOptionalMessage" class="form-control" rows="3" id="optionalMessage" placeholder="Message" name="Message"></textarea>
                </div>
              <input type="hidden" name="_subject" :value="recommendedFrameworkByUser" />
            </div>
            <div class="modal-footer">
              <button type="button" class="btn btn-default" data-dismiss="modal">Close</button>
              <button type="button" class="btn btn-success" data-dismiss="modal" v-on:click="sendMail(recommendedFrameworkByUser, emailFormOptionalMessage)">Submit Recommendation</button>
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
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      {{this.angularScalabilityPercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Modularity</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      {{this.angularModularityPercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Backwards Compatibility</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      {{this.angularBackwardsCompatibilityPercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Testability</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      {{this.angularTestabilityPercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Support</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      {{this.angularSupportPercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Future</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      {{this.angularFuturePercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Performance</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      {{this.angularPerformancePercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Customizability</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      {{this.angularCustomizabilityPercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Readability</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      {{this.angularReadabilityPercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Framework Size</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      {{this.angularFrameworkSizePercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Time in hand</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      {{this.angularTimeInHandPercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Language</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      {{this.angularLanguagePercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>App Size</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      {{this.angularAppSizePercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Learning Curve</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      {{this.angularLearningCurvePercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Standards Complaint</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      {{this.angularStandardsComplaintPercentage}}%
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
                    <td>
                      {{this.reactScalabilityPercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Modularity</th>
                    <td>
                      {{this.reactModularityPercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Backwards Compatibility</th>
                    <td>
                      {{this.reactBackwardsCompatibilityPercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Testability</th>
                    <td>
                      {{this.reactTestabilityPercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Support</th>
                    <td>
                      {{this.reactSupportPercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Future</th>
                    <td>
                      {{this.reactFuturePercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Performance</th>
                    <td>
                      {{this.reactPerformancePercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Customizability</th>
                    <td>
                      {{this.reactCustomizabilityPercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Readability</th>
                    <td>
                      {{this.reactReadabilityPercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Framework Size</th>
                    <td>
                      {{this.reactFrameworkSizePercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Time in hand</th>
                    <td>
                      {{this.reactTimeInHandPercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Language</th>
                    <td>
                      {{this.reactLanguagePercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>App Size</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      {{this.reactAppSizePercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Learning Curve</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      {{this.reactLearningCurvePercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Standards Complaint</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      {{this.reactStandardsComplaintPercentage}}%
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
                    <td>
                      {{this.vueScalabilityPercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Modularity</th>
                    <td>
                      {{this.vueModularityPercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Backwards Compatibility</th>
                    <td>
                      {{this.vueBackwardsCompatibilityPercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Testability</th>
                    <td>
                      {{this.vueTestabilityPercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Support</th>
                    <td>
                      {{this.vueSupportPercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Future</th>
                    <td>
                      {{this.vueFuturePercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Performance</th>
                    <td>
                      {{this.vuePerformancePercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Customizability</th>
                    <td>
                      {{this.vueCustomizabilityPercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Readability</th>
                    <td>
                      {{this.vueReadabilityPercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Framework Size</th>
                    <td>
                      {{this.vueFrameworkSizePercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Time in hand</th>
                    <td>
                      {{this.vueTimeInHandPercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Language</th>
                    <td>
                      {{this.vueLanguagePercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>App Size</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      {{this.vueAppSizePercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Learning Curve</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      {{this.vueLearningCurvePercentage}}%
                    </td>
                  </tr>
                  <tr>
                    <th>Standards Complaint</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      {{this.vueStandardsComplaintPercentage}}%
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

//      $('#myModal').modal({
//        backdrop: 'static'
//      });


//      $(function () {
//        $('#myModal').on('hidden.bs.modal', function (e) {
//          toastr.success('Thank you for the recommendation.', 'Email Sent', {timeOut: 5000})
//        });
//      });


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

//                  console.log(framework + ", " + keyChild + ", goalMet : " + fdSubChild["goalMet"]);
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
            this.angularScalabilityPercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "modularity")
          {
            this.angularModularityPercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "backwardsCompatibility")
          {
            this.angularBackwardsCompatibilityPercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "testability")
          {
            this.angularTestabilityPercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "support")
          {
            this.angularSupportPercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "future")
          {
            this.angularFuturePercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "performance")
          {
            this.angularPerformancePercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "customizability")
          {
            this.angularCustomizabilityPercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "readability")
          {
            this.angularReadabilityPercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "frameworkSize")
          {
            this.angularFrameworkSizePercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "timeInHand")
          {
            this.angularTimeInHandPercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "languageES6")
          {
            this.angularLanguagePercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "languageTypeScript")
          {
            this.angularLanguagePercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "appSize")
          {
            this.angularAppSizePercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "learningCurve")
          {
            this.angularLearningCurvePercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "standardsComplaint")
          {
            this.angularStandardsComplaintPercentage = currentCriteriaPercentage;
          }
        }
        else if (currentFramework === "React")
        {
          if (currentCriteria === "scalability")
          {
            this.reactScalabilityPercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "modularity")
          {
            this.reactModularityPercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "backwardsCompatibility")
          {
            this.reactBackwardsCompatibilityPercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "testability")
          {
            this.reactTestabilityPercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "support")
          {
            this.reactSupportPercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "future")
          {
            this.reactFuturePercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "performance")
          {
            this.reactPerformancePercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "customizability")
          {
            this.reactCustomizabilityPercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "readability")
          {
            this.reactReadabilityPercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "frameworkSize")
          {
            this.reactFrameworkSizePercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "timeInHand")
          {
            this.reactTimeInHandPercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "languageES6")
          {
            this.reactLanguagePercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "languageTypeScript")
          {
            this.reactLanguagePercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "appSize")
          {
            this.reactAppSizePercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "learningCurve")
          {
            this.reactLearningCurvePercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "standardsComplaint")
          {
            this.reactStandardsComplaintPercentage = currentCriteriaPercentage;
          }
        }
        else if (currentFramework === "Vue")
        {
          if (currentCriteria === "scalability")
          {
            this.vueScalabilityPercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "modularity")
          {
            this.vueModularityPercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "backwardsCompatibility")
          {
            this.vueBackwardsCompatibilityPercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "testability")
          {
            this.vueTestabilityPercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "support")
          {
            this.vueSupportPercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "future")
          {
            this.vueFuturePercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "performance")
          {
            this.vuePerformancePercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "customizability")
          {
            this.vueCustomizabilityPercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "readability")
          {
            this.vueReadabilityPercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "frameworkSize")
          {
            this.vueFrameworkSizePercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "timeInHand")
          {
            this.vueTimeInHandPercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "languageES6")
          {
            this.vueLanguagePercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "languageTypeScript")
          {
            this.vueLanguagePercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "appSize")
          {
            this.vueAppSizePercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "learningCurve")
          {
            this.vueLearningCurvePercentage = currentCriteriaPercentage;
          }
          else if (currentCriteria === "standardsComplaint")
          {
            this.vueStandardsComplaintPercentage = currentCriteriaPercentage;
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
        $.ajax({
          url: "https://formspree.io/faizan.sg@gmail.com",
          method: "POST",
          data:
            {
              'Recommended Framework': recommendedFrameworkByUser,
              'Message': optionalMessage,
          },
          dataType: "json"
        });

        $('#myModal').on('hidden.bs.modal', function (e) {
          toastr.success('Thank you for the recommendation.', 'Email Sent', {timeOut: 10000})
        });
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

</style>
