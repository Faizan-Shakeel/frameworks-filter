<template>

  <!--Accordion Start-->

  <div class="col-sm-6 col-md-6 col-lg-6">
    <div class="panel-group" id="accordion" role="tablist" aria-multiselectable="true">
      <div class="panel panel-default">
        <div class="panel-heading" role="tab" id="headingOne">
          <h4 class="panel-title">
            <a role="button" data-toggle="collapse" data-parent="#accordion" href="#collapseOne" aria-expanded="true" aria-controls="collapseOne" class="test-accordion-style">
              Angular 2
              <span class="total-percentage">
                                        {{totalPercentageAngular}}%
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
                    {{totalPercentageReact}}%
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
                    {{totalPercentageVue}}%
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

</template>

<script>

  export default {

    name: 'Accordion',

    data () {
      return {
      }
    },

    props: ['totalPercentageAngular',
      'totalPercentageReact',
      'totalPercentageVue',
      'angularScalabilityLow',
      'angularScalabilityMid',
      'angularScalabilityHigh',
      'angularModularityLow',
      'angularModularityMid',
      'angularModularityHigh',
      'angularBackwardsCompatibilityLow',
      'angularBackwardsCompatibilityMid',
      'angularBackwardsCompatibilityHigh',
      'angularTestabilityLow',
      'angularTestabilityMid',
      'angularTestabilityHigh',
      'angularSupportLow',
      'angularSupportMid',
      'angularSupportHigh',
      'angularFutureLow',
      'angularFutureMid',
      'angularFutureHigh',
      'angularPerformanceLow',
      'angularPerformanceMid',
      'angularPerformanceHigh',
      'angularCustomizabilityLow',
      'angularCustomizabilityMid',
      'angularCustomizabilityHigh',
      'angularReadabilityLow',
      'angularReadabilityMid',
      'angularReadabilityHigh',
      'angularFrameworkSizeLow',
      'angularFrameworkSizeMid',
      'angularFrameworkSizeHigh',
      'angularTimeInHandLow',
      'angularTimeInHandMid',
      'angularTimeInHandHigh',
      'angularLanguageLow',
      'angularLanguageMid',
      'angularLanguageHigh',
      'angularAppSizeLow',
      'angularAppSizeMid',
      'angularAppSizeHigh',
      'angularLearningCurveLow',
      'angularLearningCurveMid',
      'angularLearningCurveHigh',
      'angularStandardsComplaintLow',
      'angularStandardsComplaintMid',
      'angularStandardsComplaintHigh',
      'reactScalabilityLow',
      'reactScalabilityMid',
      'reactScalabilityHigh',
      'reactModularityLow',
      'reactModularityMid',
      'reactModularityHigh',
      'reactBackwardsCompatibilityLow',
      'reactBackwardsCompatibilityMid',
      'reactBackwardsCompatibilityHigh',
      'reactTestabilityLow',
      'reactTestabilityMid',
      'reactTestabilityHigh',
      'reactSupportLow',
      'reactSupportMid',
      'reactSupportHigh',
      'reactFutureLow',
      'reactFutureMid',
      'reactFutureHigh',
      'reactPerformanceLow',
      'reactPerformanceMid',
      'reactPerformanceHigh',
      'reactCustomizabilityLow',
      'reactCustomizabilityMid',
      'reactCustomizabilityHigh',
      'reactReadabilityLow',
      'reactReadabilityMid',
      'reactReadabilityHigh',
      'reactFrameworkSizeLow',
      'reactFrameworkSizeMid',
      'reactFrameworkSizeHigh',
      'reactTimeInHandLow',
      'reactTimeInHandMid',
      'reactTimeInHandHigh',
      'reactLanguageLow',
      'reactLanguageMid',
      'reactLanguageHigh',
      'reactAppSizeLow',
      'reactAppSizeMid',
      'reactAppSizeHigh',
      'reactLearningCurveLow',
      'reactLearningCurveMid',
      'reactLearningCurveHigh',
      'reactStandardsComplaintLow',
      'reactStandardsComplaintMid',
      'reactStandardsComplaintHigh',
      'vueScalabilityLow',
      'vueScalabilityMid',
      'vueScalabilityHigh',
      'vueModularityLow',
      'vueModularityMid',
      'vueModularityHigh',
      'vueBackwardsCompatibilityLow',
      'vueBackwardsCompatibilityMid',
      'vueBackwardsCompatibilityHigh',
      'vueTestabilityLow',
      'vueTestabilityMid',
      'vueTestabilityHigh',
      'vueSupportLow',
      'vueSupportMid',
      'vueSupportHigh',
      'vueFutureLow',
      'vueFutureMid',
      'vueFutureHigh',
      'vuePerformanceLow',
      'vuePerformanceMid',
      'vuePerformanceHigh',
      'vueCustomizabilityLow',
      'vueCustomizabilityMid',
      'vueCustomizabilityHigh',
      'vueReadabilityLow',
      'vueReadabilityMid',
      'vueReadabilityHigh',
      'vueFrameworkSizeLow',
      'vueFrameworkSizeMid',
      'vueFrameworkSizeHigh',
      'vueTimeInHandLow',
      'vueTimeInHandMid',
      'vueTimeInHandHigh',
      'vueLanguageLow',
      'vueLanguageMid',
      'vueLanguageHigh',
      'vueAppSizeLow',
      'vueAppSizeMid',
      'vueAppSizeHigh',
      'vueLearningCurveLow',
      'vueLearningCurveMid',
      'vueLearningCurveHigh',
      'vueStandardsComplaintLow',
      'vueStandardsComplaintMid',
      'vueStandardsComplaintHigh'
    ]
  }

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>

  .total-percentage
  {
    float: right;
    color: darkgreen;
    cursor: default;
    pointer-events: none;
  }

  .table>tbody>tr>td, .table>tbody>tr>th, .table>tfoot>tr>td, .table>tfoot>tr>th, .table>thead>tr>td, .table>thead>tr>th
  {
    color: #595959;
  }

  table.collapse.in {
    display: table;
  }

  .panel-heading a{
    text-decoration: none;
    color: deepskyblue;
  }

  .progress
  {
    margin-bottom: 0;
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

</style>
