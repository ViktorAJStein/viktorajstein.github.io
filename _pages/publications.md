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
    return (text || "").replace(/\s+/g, "").toLowerCase();
  }

  function setBadgeType(a, type, label) {
    a.classList.add("pub-badge", "pub-badge--" + type);

    const currentText = (a.textContent || "").trim();
    if (!currentText) {
      a.textContent = label;
    }

    if (!a.getAttribute("title")) {
      a.setAttribute("title", label);
    }

    a.setAttribute("aria-label", label);
  }

  function classifyBibBaseLinks() {
    const links = document.querySelectorAll(".bibbase_paper_content a");

    links.forEach((a) => {
      const rawText = (a.textContent || "").trim();
      const label = normalizeLabel(rawText);
      const href = (a.getAttribute("href") || "").toLowerCase();

      // Avoid reprocessing
      if (a.classList.contains("pub-badge")) return;

      if (label.includes("doi") || href.includes("doi.org")) {
        setBadgeType(a, "doi", "DOI");
      } else if (label.includes("preprint") || href.includes("arxiv.org")) {
        setBadgeType(a, "preprint", "Preprint");
      } else if (label.includes("code") || href.includes("github.com") || href.includes("gitlab.com")) {
        setBadgeType(a, "code", "Code");
      } else if (label.includes("slides") || href.includes("speakerdeck.com")) {
        setBadgeType(a, "slides", "Slides");
      } else if (label.includes("video") || href.includes("youtube.com") || href.includes("youtu.be")) {
        setBadgeType(a, "video", "Video");
      } else if (label.includes("biblatex") || label.includes("bibtex") || href.endsWith(".bib")) {
        setBadgeType(a, "bib", "BibLaTeX");
      } else if (label.includes("pdf")) {
        setBadgeType(a, "pdf", "PDF");
      } else if (label.includes("paper")) {
        setBadgeType(a, "paper", "Paper");
      } else {
        a.classList.add("pub-badge");
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
