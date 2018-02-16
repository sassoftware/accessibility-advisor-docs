# Accessibility Advisor Documentation

This project provides user documentation for the Accessibility Advisor Chrome extension.

## Overview

Accessibility Advisor is a Chrome Extension to help developers and testers ensure that their web
pages and applications are accessible to users with disabilities. It does this by leveraging the Axe
Core library to analyze the content of your page and make recommendations about violations. This
tool cannot find all accessibility issues but it does provide a high-quality form of automation to
augment other auditing and testing efforts.

### Prerequisites

The only prerequisite for using Accessibility Advisor is a current version of the Chrome
browser. The extension bundles all of the other technology needed to use it.

### Installation

The extension is available in the Chrome Extension store. It is installed as follows:

1. Open the Chrome web store at https://chrome.google.com/webstore/category/extensions
1. In the Search box enter "Accessibility Advisor"
1. Click on the tile for the Accessibility Advisor extension
1. Use the "Add to Chrome" button to add the extension.
1. For ease of use we recommend pinning the extension to your toolbar. Click the extensions icon in
   the Chrome toolbar (it looks like a puzzle piece), and then click the pin icon next to
   Accessibility Advisor. This will add the icon for the extension to your toolbar.

## Getting Started

### Running

Once you have installed the extension you can run it on most pages displayed in your browser (see
note below). Open the page you want to check and simply click on the Accessibility Advisor
icon. This will start a scan of the current tab, and will open a new tab called "AA Report" (Note:
final label is TBD). This report will provide a listing of the accessibility issues, if any, found
on the page. Full instructions on how to interpret the report are found in the [Using the
Report](ReportDetails.md) file.

Exceptions: because of the way Chrome extension permissions work there are some pages you will not
be able to analyze. Any content displayed in an Incognito window, any URL that starts with
chrome://, or the Developer Tools window cannot be tested.

### Troubleshooting

(Content here is TBD.)

## Contributing

At present this project is not accepting contributions from outside the core development team. When
this policy changes we will provide instructions here.

## License

This project is licensed under the [Apache 2.0 License](LICENSE).

## Additional Resources

More information about accessibility efforts at SAS can be found at [our Accessibility
page](https://support.sas.com/accessibility) or by mailing us at <mailto:accessibility@sas.com>.
