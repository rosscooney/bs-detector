# B.S. 💩 Detector

**B.S. Detector** is a rejoinder to Mark Zuckerberg's dubious claims that Facebook is unable to substantively address the proliferation of fake news on its platform. A browser extension for both Chrome and Mozilla-based browsers, B.S. Detector searches all links on a given webpage for references to unreliable sources, checking against a manually compiled list of domains. It then provides visual warnings about the presence of questionable links or the browsing of questionable websites:

![bs-detector-alert](http://bsdetector.tech/images/alert.png)

The list of domains powering the B.S. Detector was somewhat indiscriminately compiled from various sources around the web. We are actively reviewing this dataset, categorizing entries, and removing misidentified domains. We thus cannot guarantee complete accuracy of our data at the moment. You can view the complete list [here](https://github.com/selfagency/bs-detector/blob/master/chrome/data/data.json).

Domain classifications include:

-   **Fake News:** Sources that fabricate stories out of whole cloth with the intent of pranking the public.
-   **Satire:** Sources that provide humorous commentary on current events in the form of fake news.
-   **Extreme Bias:** Sources that traffic in political propaganda and gross distortions of fact.
-   **Conspiracy Theory:** Sources that are well-known promoters of kooky conspiracy theories.
-   **Rumor Mill:** Sources that traffic in rumors, innuendo, and unverified claims.
-   **State News:** Sources in repressive states operating under government sanction.
-   **Junk Science:** Sources that promote pseudoscience, metaphysics, naturalistic fallacies, and other scientifically dubious claims.
-   **Hate Group:** Sources that actively promote racism, misogyny, homophobia, and other forms of discrimination.
-   **Clickbait:** Sources that are aimed at generating online advertising revenue and rely on sensationalist headlines or eye-catching pictures.
    **Proceed With Caution:** Sources that may be reliable but whose contents require further verification.

If there are any sites you recommend adding or removing, or if you object to your site being listed, you can file a report [here](https://github.com/selfagency/bs-detector/issues/53).

---

## Installation

<a name="chrome"></a>

### Chrome and Chrome-based browsers
[Click here](https://chrome.google.com/webstore/detail/dlcgkekjiopopabcifhebmphmfmdbjod/) to go to the Chrome Web Store and click 'Install.' The plugin is compatible with all Chromium browsers, including Opera (with the [Chrome Extension extension](https://addons.opera.com/en/extensions/details/download-chrome-extension-9/)).

<a name="firefox"></a>

### Firefox and Mozilla-based browsers
Installation via the Firefox Add-ons directory coming soon. For now, download a .zip [here](https://github.com/selfagency/bs-detector/releases) and follow [these instructions](https://developer.mozilla.org/en-US/Add-ons/WebExtensions/Temporary_Installation_in_Firefox) to load the add-on.

<a name="other"></a>

### Other browsers
Install [Tampermonkey](https://tampermonkey.net) for [Safari](https://tampermonkey.net/?ext=dhdg&browser=safari), [Edge](https://tampermonkey.net/?ext=dhdg&browser=edge), or any other available browser, then install the Greasemonkey script [here](https://github.com/selfagency/bs-detector/raw/master/greasemonkey/bs-detector.user.js).

---

## Contributing

We welcome pull requests and community collaboration. Before contributing, please review our [Code of Conduct](https://github.com/selfagency/bs-detector/blob/master/CODE_OF_CONDUCT.md). You can chat with other community members in realtime on Gitter [here](https://gitter.im/bs-detector/).

If you are planning to contribute, please work off and submit pull requests to the `dev` branch, which is the most current build. `master` is intended for public releases only and is several commits behind  `dev`. Edit browser specific resources in their corresponding folders, common resources in `_shared`, and use `gulp build` to compile. Check out our [roadmap](https://github.com/selfagency/bs-detector/wiki/Product-Roadmap) to see what we intend to integrate in future releases and to decide whether you'd like to help with one of those tasks, as they might be duplicative of new functionality you wish to propose. We don't want to squander your time or enthusiasm, so we recommend proposing new functionality in an issue or on Gitter before building something out we might not end up using. It will also provide you with an opportunity to hear from other community members who might help flesh out your ideas.
