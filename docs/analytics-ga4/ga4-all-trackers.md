# Trackers

For tracking different kinds of data on GOV.UK we have built several different trackers. Each type of tracking is handled by a separate script, but some code is shared between them as they often do similar things.

Most of the trackers work by adding a `data-module` attribute to an element along with additional data attributes to provide specific tracking information. Some components have this already built into their code, which is usually activated using a `ga4_tracking: true` option.

## Link tracking

There are several types of link tracking. To distinguish them and simplify the code, we define them as follows.

- the [link tracker](https://github.com/alphagov/govuk_publishing_components/blob/main/docs/analytics-ga4/ga4-link-tracker.md) handles link clicks with data attributes added to specific links, or to parent elements of groups of links
- the [specialist link tracker](https://github.com/alphagov/govuk_publishing_components/blob/main/docs/analytics-ga4/ga4-specialist-link-tracker.md)automatically tracks clicks on 'special' links, such as external links, download links and mailto links

## Event tracking

The [event tracker](https://github.com/alphagov/govuk_publishing_components/blob/main/docs/analytics-ga4/ga4-event-tracker.md) handles tracking on buttons or other interactive elements, such as tabs and details elements.

## Auto tracking

The [auto tracker](https://github.com/alphagov/govuk_publishing_components/blob/main/docs/analytics-ga4/ga4-auto-tracker.md) is used to cause an event to occur as soon as a page has finished loading (but after a page view). This is used to track significant moments in journeys, such as the successful completion of a smart answer, or an error.

## Ecommerce tracker

The [ecommerce tracker](https://github.com/alphagov/govuk_publishing_components/blob/main/docs/analytics-ga4/ga4-ecommerce-tracker.md) is used to track things like search results within a finder.

## Form tracker

The [form tracker](https://github.com/alphagov/govuk_publishing_components/blob/main/docs/analytics-ga4/ga4-form-tracker.md) is designed to capture data about a form when it has been submitted.

## Smart answer results tracker

The [smart answer results tracker](https://github.com/alphagov/govuk_publishing_components/blob/main/docs/analytics-ga4/ga4-smart-answer-results-tracker.md) has been built specifically to track the Cost of Living smart answer.