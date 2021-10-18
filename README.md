# Linkvertise-Bypass by. R0z3y44#3331

- Als erstes installiert ihr die Browser Erweiterung: ,,Tampermonkey"
- Dann geht kopiert ihr diesen Script:
 
// ==UserScript==
// @name         Linkvertise Bypass
// @namespace    http://tampermonkey.net/
// @version      1.0
// @description  Bypasses Linkvertise links with foreign api
// @author       HussNuss
// @match        *://*.linkvertise.com/*
// @match        *://*.linkvertise.net/*
// @match        *://*.link-to.net/*
// @exclude      *://publisher.linkvertise.com/*
// @exclude      *://linkvertise.com
// @exclude      *://linkvertise.com/search*
// @exclude      *://blog.linkvertise.com
// @exclude      *://blog.linkvertise.com/*
// @exclude      https://linkvertise.com/assets/vendor/thinksuggest.html
// @exclude      https://linkvertise.com/
// @grant        GM.xmlHttpRequest
// @icon         https://www.google.com/s2/favicons?domain=linkvertise.com
// @grant        none
// ==/UserScript==

(async function () {
    'use strict';
      var url = "https://bypass.bot.nu/bypass2?url=" + location.href;
      var oReq = new XMLHttpRequest();
      oReq.addEventListener("load", function() {
          location = JSON.parse(this.responseText).destination;
      });
      oReq.open("GET", url);
      oReq.send();
})();

- Dann geht ihr auf Tampermonkey und klickt auf: ,,Neuen Userscript erstellen".
- Als letztes löscht ihr den Script der da ist und Copy-Pastet ihr denn Script denn ihr kopiert habt.
- Damit ihr den Script saved klickt ihr oben rechts auf datei dann auf Speichern und dann seid ihr fertig und habt einen Bypass für Linkvertise!

Leak by R0z3y44 😈🔥
