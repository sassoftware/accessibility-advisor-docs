# Accessibility Advisor Documentation

This project provides user documentation for the Accessibility Advisor Chrome extension.

## Overview

Accessibility Advisor is a Chrome Extension that enables users to scan a web page for
accessibility violations with one click. Users can download a report of the violations and share
it with others.

### Installation

The extension is available in the Chrome Web Store. It is installed as follows:

1. View the extension in the [Chrome Web Store](https://chrome.google.com/webstore/detail/sas-accessibility-advisor/oajhmnajfdmljdknoeohidpjjdokokpl)
1. Use the "Add to Chrome" button to add the extension.
1. Optionally, for ease of use pin the extension to your Chrome toolbar.
   1. Click the Extensions icon in the Chrome toolbar (it looks like a puzzle piece)
   1. Click the pin icon next to Accessibility Advisor. This will add the icon for the extension
   to your toolbar.

## Getting Started

### Running

1. Browse to the Web page you want to analyze.
1. Click the Accessibility Advisor icon from the pinned location or from the Extensions menu.
1. View the report in the new tab titled "Accessibility Advisor". The report details are explained
in the following section, "Report Details".
1. Optionally, save the report by clicking the "Save Report" button at the end of the report.
1. To evaluate a new page, repeat all of the previous steps. The current report will update to
show the accessibility analysis of the new page.

Note, some pages may take a longer time to analyze. While the analysis is running, the message
"Analyzing Page..." will be displayed in the report.


### Report Details

Accessibility Advisor reports accessibility violations found on Web pages. Each report contains
the following.

* The date and time of the analysis.
* The Application Conformance Level.
  * This value should be ignored as it will be removed soon.
* The URL of the page evaluated.
* A screenshot of the page evaluated.
* The detected accessibility violations, categorized by type
* A Save Report button, which saves the report as a single file.

Each set of categorized accessibility violations indicates the type of violation and the number of
violations. The individual instances of violations are listed within each set of categories. Each
category can be expanded and collapsed. The individual instances contain the following information.

* A screenshot of the element, if the element is in the current viewport.
  * If the element with the violation is not in the current viewport, the screenshot will be blank
  or say "Screenshot not available".
* Problem: A high level description of the problem that was detected.
* Solution: Suggested solutions for solving the problem.
* HTML: The HTML snippet where the problem was detected.
* CSS Selector: The CSS Selector where the problem was detected.
  * Note, violations found in iframes will be in the form of a comma separated list, listing the CSS
  Selector for each iframe, and ending with the CSS Selector of the element itself. For instance,
  "#frameContent, h1" indicates an h1 element found in an iframe with the ID of "frameContent".
* Help: A link to help documentation, explaining the violation.
* Impact: A measure of the impact this violation has in users.
  * This value should be ignored as it will be
removed soon.
* WCAG Criteria: The WCAG criteria violated.
* WCAG Conformance Level: The WCAG conformance level violated.
* Timestamp: The timestamp when the analysis was performed.

To share the findings with others, the entire report can be sent, or individual violations can be
copied and pasted into emails, word processing documents, or bug tracking software.


### Troubleshooting

* To evaluate a page in Incognito mode, you must first enable the permission for Accessibility
Advisor to run in Incognito pages.
* If a page cannot be analyzed, an error message will be displayed in the report explaining why the
page cannot be analyzed.

## Contributing

At present this project is not accepting contributions from outside the core development team. When
this policy changes we will provide instructions here.

## License

This project is licensed under the [SAS® Accessibility Advisor Software End User License Agreement](https://support.sas.com/accessibility/doc/AccessibilityAdvisorForChromeEULA.pdf).

## Additional Resources

More information about accessibility efforts at SAS can be found at [our Accessibility
page](https://support.sas.com/accessibility) or by mailing us at <mailto:accessibility@sas.com>.
