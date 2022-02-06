---
title: Flagrant Garden
description: A Garden of Play, Flagrantly Cultivated
type: docs
---

Welcome to the Flagrant Garden, a nursery for narrative play.

We're very much under early construction;
in the menu on the left you can find our growing catalogue of playkits as well as our [call to cultivate them](/cultivation), our [blog](/posts), and a list of [flagrantly cultivated works found elsewhere](/cultivars).

You can find free web editions of our games here, namely [Flagrant Factions](/games/factions) and [Flagrant66](/games/66).

Finally, you might want to [check us out on OpenCollective](https://opencollective.com/flagrantgarden), where you can contribute to our work, back projects, and see what we're up to more broadly.

<!--
  This is the HTML block you need to insert wherever you want
  your webring to show up. By default, it is displayed exactly
  as it is styled on the host.

  The entries in the allow attribute(s) are security defaults.
  You're welcome to override them if you want, but it's best
  to leave them in place unless something is broken. For more
  info on them, see:
      https://www.w3schools.com/tags/tag_iframe.asp
  The only setting that *has* to remain in place is in the
  sandbox attribute; 'allow-top-navigation-by-user-activation'
  is what enables the iframe to send users to a member site or
  the list of members. The 'allow-same-origin' is required for
  the included script to work and set the styling correctly.
  The 'allow-scripts' attribute is only required if you are
  using the random member link.
-->
<iframe id="toroidal-iframe-gardeners-circle-first-member"
        class="toroidal"
        frameBorder="0"
        allow="layout-animations 'none';
        unoptimized-images 'none';
        oversized-images 'none';
        sync-script 'none';
        sync-xhr 'none';
        unsized-media 'none';"
        allowfullscreen="false"
        allowpaymentrequest="false"
        sandbox="allow-top-navigation allow-same-origin allow-scripts"
        src="https://deploy-preview-29--flagrant-garden.netlify.app/toroidal/first-member/" >
</iframe>

<!--
  You can put this script block wherever makes sense for your
  site; you might want it in your footer or pulled into a JS
  file, but if you want the iframe to configure correctly,
  you will need it *somewhere*.
-->
<script>
  // This function configures the iframe display so that it
  // looks okay after loading; this default implementation
  // will display the iframe to its actual size wherever
  // you put it in your site, themed exactly as it is on
  // the host.
  function configureToroidalIframe() {
    let iframeID = 'toroidal-iframe-gardeners-circle-first-member'
    let navID    = 'toroidal-nav-gardeners-circle'
    let webringIframe = document.getElementById(iframeID);
    if (webringIframe != null) {
      let webringDoc = webringIframe.contentDocument;
      let webringNav = webringDoc.getElementById(navID);
      webringDoc.body.style.overflow = 'hidden';
      webringIframe.style.height = (webringNav.scrollHeight + 30) + 'px';
    } else {
      setTimeout(configureToroidalIframe, 100);
    }
  }

  // When the window loads, the iframe configuration is called;
  // the implementation will retry until it is able to connect.
  window.onload = function() {
    configureToroidalIframe();
  }
</script>
