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
                  <span class="glyphicon glyphicon-info-sign total-percentage-notification tooltips" data-tooltip-content="#check-individual-results"></span>
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
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularModularityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularModularityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularModularityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Backwards Compatibility</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularBackwardsCompatibilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularBackwardsCompatibilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularBackwardsCompatibilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Testability</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularTestabilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularTestabilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularTestabilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Support</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularSupportLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularSupportMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularSupportHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Future</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularFutureLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularFutureMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularFutureHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Performance</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularPerformanceLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularPerformanceMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularPerformanceHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Customizability</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularCustomizabilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularCustomizabilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularCustomizabilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Readability</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularReadabilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularReadabilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularReadabilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Framework Size</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularFrameworkSizeLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularFrameworkSizeMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularFrameworkSizeHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Time in hand</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularTimeInHandLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularTimeInHandMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularTimeInHandHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Language</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularLanguageLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularLanguageMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularLanguageHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>App Size</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularAppSizeLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularAppSizeMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularAppSizeHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Learning Curve</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularLearningCurveLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularLearningCurveMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularLearningCurveHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Standards Complaint</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="angularStandardsComplaintLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="angularStandardsComplaintMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="angularStandardsComplaintHigh"></div>
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
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactModularityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactModularityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactModularityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Backwards Compatibility</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactBackwardsCompatibilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactBackwardsCompatibilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactBackwardsCompatibilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Testability</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactTestabilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactTestabilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactTestabilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Support</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactSupportLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactSupportMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactSupportHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Future</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactFutureLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactFutureMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactFutureHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Performance</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactPerformanceLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactPerformanceMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactPerformanceHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Customizability</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactCustomizabilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactCustomizabilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactCustomizabilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Readability</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactReadabilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactReadabilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactReadabilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Framework Size</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactFrameworkSizeLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactFrameworkSizeMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactFrameworkSizeHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Time in hand</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactTimeInHandLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactTimeInHandMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactTimeInHandHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Language</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactLanguageLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactLanguageMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactLanguageHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>App Size</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactAppSizeLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactAppSizeMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactAppSizeHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Learning Curve</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactLearningCurveLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactLearningCurveMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactLearningCurveHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Standards Complaint</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="reactStandardsComplaintLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="reactStandardsComplaintMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="reactStandardsComplaintHigh"></div>
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
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueModularityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueModularityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueModularityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Backwards Compatibility</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueBackwardsCompatibilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueBackwardsCompatibilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueBackwardsCompatibilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Testability</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueTestabilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueTestabilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueTestabilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Support</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueSupportLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueSupportMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueSupportHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Future</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueFutureLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueFutureMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueFutureHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Performance</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vuePerformanceLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vuePerformanceMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vuePerformanceHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Customizability</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueCustomizabilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueCustomizabilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueCustomizabilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Readability</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueReadabilityLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueReadabilityMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueReadabilityHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Framework Size</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueFrameworkSizeLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueFrameworkSizeMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueFrameworkSizeHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Time in hand</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueTimeInHandLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueTimeInHandMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueTimeInHandHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Language</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueLanguageLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueLanguageMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueLanguageHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>App Size</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueAppSizeLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueAppSizeMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueAppSizeHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Learning Curve</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueLearningCurveLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueLearningCurveMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueLearningCurveHigh"></div>
                      </div>
                    </td>
                  </tr>
                  <tr>
                    <th>Standards Complaint</th>
                    <td class="col-xs-1 col-sm-2 col-md-1 col-lg-1">
                      <div class="progress">
                        <div class="progress-bar progress-bar-danger progress-bar-striped" :style="vueStandardsComplaintLow"></div>
                        <div class="progress-bar progress-bar-success progress-bar-striped" :style="vueStandardsComplaintMid"></div>
                        <div class="progress-bar progress-bar-info progress-bar-striped active" :style="vueStandardsComplaintHigh"></div>
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

  /*.progress-bar-vertical {*/
    /*width: 25px;*/
    /*min-height: 44px;*/
    /*display: flex;*/
    /*align-items: flex-end;*/
    /*margin: 0 5px 0 0;*/
    /*float: left;*/
  /*}*/

  /*.progress-bar-vertical .progress-bar {*/
    /*width: 100%;*/
    /*height: 0;*/
    /*-webkit-transition: height 0.6s ease;*/
    /*-o-transition: height 0.6s ease;*/
    /*transition: height 0.6s ease;*/
  /*}*/

  .progress
  {
    margin-bottom: 0;
  }

  /*.table>tbody>tr>td, .table>tbody>tr>th, .table>tfoot>tr>td, .table>tfoot>tr>th, .table>thead>tr>td, .table>thead>tr>th*/
  /*{*/
     /*vertical-align: middle !important;*/
  /*}*/

</style>
