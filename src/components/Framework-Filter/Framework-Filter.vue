<template>

  <div class="filter-container">

    <Tooltips-Template></Tooltips-Template>
    <Navigation-Bar v-bind:check-form-status=checkFormStatus v-bind:clear-form=clearForm></Navigation-Bar>

    <div class="row whole-page">

      <a class="feedback" href="https://goo.gl/forms/6sakUAormUq3IkU43" target="_blank">Feedback</a>

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

      <Accordion v-bind:total-percentage-angular=totalPercentageAngular
                 v-bind:total-percentage-react=totalPercentageReact
                 v-bind:total-percentage-vue=totalPercentageVue
                 v-bind:angular-scalability-low=angularScalabilityLow
                 v-bind:angular-scalability-mid=angularScalabilityMid
                 v-bind:angular-scalability-high=angularScalabilityHigh
                 v-bind:angular-modularity-low=angularModularityLow
                 v-bind:angular-modularity-mid=angularModularityMid
                 v-bind:angular-modularity-high=angularModularityHigh
                 v-bind:angular-backwards-compatibility-low=angularBackwardsCompatibilityLow
                 v-bind:angular-backwards-compatibility-mid=angularBackwardsCompatibilityMid
                 v-bind:angular-backwards-compatibility-high=angularBackwardsCompatibilityHigh
                 v-bind:angular-testability-low=angularTestabilityLow
                 v-bind:angular-testability-mid=angularTestabilityMid
                 v-bind:angular-testability-high=angularTestabilityHigh
                 v-bind:angular-support-low=angularSupportLow
                 v-bind:angular-support-mid=angularSupportMid
                 v-bind:angular-support-high=angularSupportHigh
                 v-bind:angular-future-low=angularFutureLow
                 v-bind:angular-future-mid=angularFutureMid
                 v-bind:angular-future-high=angularFutureHigh
                 v-bind:angular-performance-low=angularPerformanceLow
                 v-bind:angular-performance-mid=angularPerformanceMid
                 v-bind:angular-performance-high=angularPerformanceHigh
                 v-bind:angular-customizability-low=angularCustomizabilityLow
                 v-bind:angular-customizability-mid=angularCustomizabilityMid
                 v-bind:angular-customizability-high=angularCustomizabilityHigh
                 v-bind:angular-readability-low=angularReadabilityLow
                 v-bind:angular-readability-mid=angularReadabilityMid
                 v-bind:angular-readability-high=angularReadabilityHigh
                 v-bind:angular-framework-size-low=angularFrameworkSizeLow
                 v-bind:angular-framework-size-mid=angularFrameworkSizeMid
                 v-bind:angular-framework-size-high=angularFrameworkSizeHigh
                 v-bind:angular-time-in-hand-low=angularTimeInHandLow
                 v-bind:angular-time-in-hand-mid=angularTimeInHandMid
                 v-bind:angular-time-in-hand-high=angularTimeInHandHigh
                 v-bind:angular-language-low=angularLanguageLow
                 v-bind:angular-language-mid=angularLanguageMid
                 v-bind:angular-language-high=angularLanguageHigh
                 v-bind:angular-app-size-low=angularAppSizeLow
                 v-bind:angular-app-size-mid=angularAppSizeMid
                 v-bind:angular-app-size-high=angularAppSizeHigh
                 v-bind:angular-learning-curve-low=angularLearningCurveLow
                 v-bind:angular-learning-curve-mid=angularLearningCurveMid
                 v-bind:angular-learning-curve-high=angularLearningCurveHigh
                 v-bind:angular-standards-complaint-low=angularStandardsComplaintLow
                 v-bind:angular-standards-complaint-mid=angularStandardsComplaintMid
                 v-bind:angular-standards-complaint-high=angularStandardsComplaintHigh
                 v-bind:react-scalability-low=reactScalabilityLow
                 v-bind:react-scalability-mid=reactScalabilityMid
                 v-bind:react-scalability-high=reactScalabilityHigh
                 v-bind:react-modularity-low=reactModularityLow
                 v-bind:react-modularity-mid=reactModularityMid
                 v-bind:react-modularity-high=reactModularityHigh
                 v-bind:react-backwards-compatibility-low=reactBackwardsCompatibilityLow
                 v-bind:react-backwards-compatibility-mid=reactBackwardsCompatibilityMid
                 v-bind:react-backwards-compatibility-high=reactBackwardsCompatibilityHigh
                 v-bind:react-testability-low=reactTestabilityLow
                 v-bind:react-testability-mid=reactTestabilityMid
                 v-bind:react-testability-high=reactTestabilityHigh
                 v-bind:react-support-low=reactSupportLow
                 v-bind:react-support-mid=reactSupportMid
                 v-bind:react-support-high=reactSupportHigh
                 v-bind:react-future-low=reactFutureLow
                 v-bind:react-future-mid=reactFutureMid
                 v-bind:react-future-high=reactFutureHigh
                 v-bind:react-performance-low=reactPerformanceLow
                 v-bind:react-performance-mid=reactPerformanceMid
                 v-bind:react-performance-high=reactPerformanceHigh
                 v-bind:react-customizability-low=reactCustomizabilityLow
                 v-bind:react-customizability-mid=reactCustomizabilityMid
                 v-bind:react-customizability-high=reactCustomizabilityHigh
                 v-bind:react-readability-low=reactReadabilityLow
                 v-bind:react-readability-mid=reactReadabilityMid
                 v-bind:react-readability-high=reactReadabilityHigh
                 v-bind:react-framework-size-low=reactFrameworkSizeLow
                 v-bind:react-framework-size-mid=reactFrameworkSizeMid
                 v-bind:react-framework-size-high=reactFrameworkSizeHigh
                 v-bind:react-time-in-hand-low=reactTimeInHandLow
                 v-bind:react-time-in-hand-mid=reactTimeInHandMid
                 v-bind:react-time-in-hand-high=reactTimeInHandHigh
                 v-bind:react-language-low=reactLanguageLow
                 v-bind:react-language-mid=reactLanguageMid
                 v-bind:react-language-high=reactLanguageHigh
                 v-bind:react-app-size-low=reactAppSizeLow
                 v-bind:react-app-size-mid=reactAppSizeMid
                 v-bind:react-app-size-high=reactAppSizeHigh
                 v-bind:react-learning-curve-low=reactLearningCurveLow
                 v-bind:react-learning-curve-mid=reactLearningCurveMid
                 v-bind:react-learning-curve-high=reactLearningCurveMid
                 v-bind:react-standards-complaint-low=reactStandardsComplaintLow
                 v-bind:react-standards-complaint-mid=reactStandardsComplaintMid
                 v-bind:react-standards-complaint-high=reactStandardsComplaintHigh
                 v-bind:vue-scalability-low=vueScalabilityLow
                 v-bind:vue-scalability-mid=vueScalabilityMid
                 v-bind:vue-scalability-high=vueScalabilityHigh
                 v-bind:vue-modularity-low=vueModularityLow
                 v-bind:vue-modularity-mid=vueModularityMid
                 v-bind:vue-modularity-high=vueModularityHigh
                 v-bind:vue-backwards-compatibility-low=vueBackwardsCompatibilityLow
                 v-bind:vue-backwards-compatibility-mid=vueBackwardsCompatibilityMid
                 v-bind:vue-backwards-compatibility-high=vueBackwardsCompatibilityHigh
                 v-bind:vue-testability-low=vueTestabilityLow
                 v-bind:vue-testability-mid=vueTestabilityMid
                 v-bind:vue-testability-high=vueTestabilityHigh
                 v-bind:vue-support-low=vueSupportLow
                 v-bind:vue-support-mid=vueSupportMid
                 v-bind:vue-support-high=vueSupportHigh
                 v-bind:vue-future-low=vueFutureLow
                 v-bind:vue-future-mid=vueFutureMid
                 v-bind:vue-future-high=vueFutureHigh
                 v-bind:vue-performance-low=vuePerformanceLow
                 v-bind:vue-performance-mid=vuePerformanceMid
                 v-bind:vue-performance-high=vuePerformanceHigh
                 v-bind:vue-customizability-low=vueCustomizabilityLow
                 v-bind:vue-customizability-mid=vueCustomizabilityMid
                 v-bind:vue-customizability-high=vueCustomizabilityHigh
                 v-bind:vue-readability-low=vueReadabilityLow
                 v-bind:vue-readability-mid=vueReadabilityMid
                 v-bind:vue-readability-high=vueReadabilityHigh
                 v-bind:vue-framework-size-low=vueFrameworkSizeLow
                 v-bind:vue-framework-size-mid=vueFrameworkSizeMid
                 v-bind:vue-framework-size-high=vueFrameworkSizeHigh
                 v-bind:vue-time-in-hand-low=vueTimeInHandLow
                 v-bind:vue-time-in-hand-mid=vueTimeInHandMid
                 v-bind:vue-time-in-hand-high=vueTimeInHandHigh
                 v-bind:vue-language-low=vueLanguageLow
                 v-bind:vue-language-mid=vueLanguageMid
                 v-bind:vue-language-high=vueLanguageHigh
                 v-bind:vue-app-size-low=vueAppSizeLow
                 v-bind:vue-app-size-mid=vueAppSizeMid
                 v-bind:vue-app-size-high=vueAppSizeHigh
                 v-bind:vue-learning-curve-low=vueLearningCurveLow
                 v-bind:vue-learning-curve-mid=vueLearningCurveMid
                 v-bind:vue-learning-curve-high=vueLearningCurveMid
                 v-bind:vue-standards-complaint-low=vueStandardsComplaintLow
                 v-bind:vue-standards-complaint-mid=vueStandardsComplaintMid
                 v-bind:vue-standards-complaint-high=vueStandardsComplaintHigh>
      </Accordion>

    </div>

    <div id="footer">
      <a href="https://goo.gl/forms/6sakUAormUq3IkU43" target="_blank">Feedback</a>
    </div>

  </div>

</template>

<script>

  import Accordion from './Accordion'
  import TooltipsTemplate from './Tooltips-Templates'
  import NavigationBar from './Nav-Bar/Navigation-Bar'

  export default {

    name: 'Framework-Filter',

    components: {
      Accordion,
      TooltipsTemplate,
      NavigationBar,
    },

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

    },

    data () {
      return {
        recommendedFrameworkByUser: '',
        emailFormOptionalMessage: '',
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

//      clearConsole: function () {
//        if (typeof console._commandLineAPI !== 'undefined') {
//          console.API = console._commandLineAPI; //chrome
//        } else if (typeof console._inspectorCommandLineAPI !== 'undefined') {
//          console.API = console._inspectorCommandLineAPI; //Safari
//        } else if (typeof console.clear !== 'undefined') {
//          console.API = console;
//        }
//        console.API.clear();
//      },

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
          }, 500);
        }

        $('.clear-data').addClass('clear-button-disabled');
        $('.clear-data-mobile').addClass('clear-button-disabled');
        this.formEdited = false;
        $("#clearFormConfirmationModal").modal('hide');
      }

    }
  }
</script>

<style>

  .whole-page
  {
    width: 95%;
    margin: 0 auto;
    font-family: 'Quicksand', sans-serif;
    letter-spacing: 2px;
  }

  .criteria-description-in-tooltip
  {
    width: 3%;
    color: darkgray;
    margin: 10px 0 0 -15px;
    cursor: default;
    font-size: medium;
  }

  .criteria-description-in-tooltip:hover
  {
    color: #595959;
    margin: 5px 0 0 -19px;
    font-size: x-large;
  }

  .form-group {
    margin-bottom: 16px;
    color: #595959;
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

  .feedback {
    position: fixed;
    transform: rotate(-90deg);
    right: -32px;
    top: 140px;
    padding: 10px 10px 5px 10px;
    letter-spacing: 2px;
    text-shadow: 1px 1px 1px rgba(0, 0, 0, 0.43);
    border-radius: 5px 5px 0px 0px;
    background: linear-gradient(to bottom,#2D77A2 5%,deepskyblue 100%);
    color: #fff;
    z-index: 1;
  }

  .feedback:hover, .feedback:focus
  {
    color: #fff;
    text-decoration: none;
    cursor: pointer;
  }

  #footer {
    display: none;
  }

  #footer a
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
    .feedback {
      display: none;
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
