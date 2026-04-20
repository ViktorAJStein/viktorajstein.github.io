---
title: "Publications"
permalink: /publications/
layout: single
author_profile: true
---

<div id="publist">
  <script src="https://bibbase.org/show?bib=https://raw.githubusercontent.com/ViktorAJStein/viktorajstein.github.io/main/files/Publications.bib&jsonp=1&group0=year&sort=-year&hidemenu=true&fullnames=1"></script>
</div>

<script>
(function () {
  function normalizeLabel(text) {
    return text.replace(/\s+/g, "").toLowerCase();
  }

  function classifyBibBaseLinks() {
    const links = document.querySelectorAll(".bibbase_paper_content a");
    links.forEach((a) => {
      const label = normalizeLabel(a.textContent || "");
      const href = (a.getAttribute("href") || "").toLowerCase();

      a.classList.add("pub-badge");

      if (label.includes("doi") || href.includes("doi.org")) {
        a.classList.add("pub-badge--doi");
      } else if (label.includes("preprint") || href.includes("arxiv.org")) {
        a.classList.add("pub-badge--preprint");
      } else if (label.includes("code") || href.includes("github.com")) {
        a.classList.add("pub-badge--code");
      } else if (label.includes("biblatex") || label.includes("bibtex") || href.endsWith(".bib")) {
        a.classList.add("pub-badge--bib");
      } else if (label.includes("slides")) {
        a.classList.add("pub-badge--slides");
      } else if (label.includes("video")) {
        a.classList.add("pub-badge--video");
      } else if (label.includes("pdf")) {
        a.classList.add("pub-badge--pdf");
      } else if (label.includes("paper")) {
        a.classList.add("pub-badge--paper");
      }
    });
  }

  const observer = new MutationObserver(classifyBibBaseLinks);
  observer.observe(document.body, { childList: true, subtree: true });

  window.addEventListener("load", classifyBibBaseLinks);
  setTimeout(classifyBibBaseLinks, 1000);
  setTimeout(classifyBibBaseLinks, 2500);
})();
</script>
