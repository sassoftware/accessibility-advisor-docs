# SAS Accessibility Advisor Documentation

This project provides user documentation for the SAS Accessibility Advisor Chrome extension.

## Overview

SAS Accessibility Advisor is a Chrome Extension that enables users to scan a web page for
accessibility violations with one click. Users can download a report of the violations and share
it with others.

### Installation

The extension is available in the Chrome Web Store. It is installed as follows:

1. View the extension in the [Chrome Web Store](https://chrome.google.com/webstore/detail/sas-accessibility-advisor/oajhmnajfdmljdknoeohidpjjdokokpl)
1. Click the **Add to Chrome** button to add the extension.
1. For easier access, you can use the following steps to pin the extension to your Chrome toolbar:
    1. Click the Extensions icon in the Chrome toolbar (it looks like a puzzle piece).
    1. Click the pin icon next to **SAS Accessibility Advisor** to add the icon for the extension
    to your toolbar.

## Getting Started

### Analyzing

1. Browse to the web page that you want to analyze.
1. Click the SAS Accessibility Advisor icon from the pinned location or from the Extensions menu.
1. View the report in the new tab titled **SAS Accessibility Advisor**. The report details are
explained in the following "Report Details" section.
1.  You can save the report by clicking the **Save Report** button at the beginning of the
report.
1. To evaluate a new page, repeat all of the previous steps. The current report will update to show
the accessibility analysis of the new page.

**Note:** Some pages might take a long time to analyze. While the analysis is running, the message
"Analyzing Page..." is displayed in the report and the title of the tab is updated to indicate that
it is analyzing.

### Report Details

SAS Accessibility Advisor finds and reports accessibility violations on web pages. Each report
contains the following information:

* The version of axe-core used in the analysis.
* The total number of accessibility violations found.
* A screenshot of the web page.
* The date and time of the analysis.
* The URL of the web page.
* Expandable sections that provide details about the accessibility violations found, grouped by the
type of violation.

Each type of accessibility violation is an expandable section. The description for the violation
includes the applicable WCAG criteria and the count of violations of this type. When expanded, the
individual instances are listed and they contain the following information:

* A **Copy Information** button, which copies the details of the violation to the
clipboard.
* A screenshot of the element with the violation, if the element is in the current viewport.
Otherwise, there is a message stating "No screen shot available".
* Problem: A high level description of the problem that was detected.
* Solution: Suggested solutions for solving the problem.
* HTML: The HTML snippet where the problem was detected.
* CSS Selector: The CSS Selector where the problem was detected, presented as a comma-delimited
list that defines the selector for each parent iframe where the violation occurs. For example,
"#frameContent, h1" indicates an h1 element found in an iframe with the ID of "frameContent".
* Help: A link to Help documentation, explaining the violation.

To share the findings with others, the entire report can be sent, or individual violations can be
copied and pasted into emails, word processing documents, or bug tracking software.

### Troubleshooting

* To evaluate a page in Incognito mode, you must first enable the permission for Accessibility
Advisor to run in Incognito pages.
* If a page cannot be analyzed, an error message is displayed in the report explaining the reason
the page cannot be analyzed.

#### Dragon Users

Dragon users cannot use native Dragon commands when viewing the report directly from the extension
(when the URL begins with chrome-extension://). This is due to limitations that Chrome imposes on
extensions, where the Dragon Web Extension cannot operate directly on other extensions such as SAS
Accessibility Advisor. To fully interact with the report:
1. Save the report by clicking the **Save Report** button at the beginning of the report.
1. Open the report as a local file in Chrome.
1. Make sure that you have granted SAS Accessibility Advisor access to local files.

## Support

Found a bug? Want to suggest a new feature? Got a question? Send email to [accessibility@sas.com](mailto:accessibility@sas.com).

## Contributing

At present this project is not accepting contributions from outside the core development team. When
this policy changes we will provide instructions here.

## License

This project is licensed under the [SAS® Accessibility Advisor Software End User License Agreement](https://support.sas.com/accessibility/doc/AccessibilityAdvisorForChromeEULA.pdf).

## User Data Policy

The use of information received from Google APIs will adhere to the
[Chrome Web Store User Data Policy](https://developer.chrome.com/docs/webstore/program_policies/#userdata),
including the [Limited Use](https://developer.chrome.com/docs/webstore/program_policies/#limited_use)
requirements.

## Additional Resources

More information about accessibility efforts at SAS can be found at [our Accessibility
page](https://support.sas.com/accessibility) or by mailing us at [accessibility@sas.com](mailto:accessibility@sas.com).

