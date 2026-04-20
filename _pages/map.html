---
title: "Map"
permalink: /map.html
layout: single
author_profile: false
---

<p>
This map shows conferences, workshops, seminars, and visits.
Blue markers indicate past trips; red markers indicate future ones.
</p>

<div id="travel-map"></div>

<div class="travel-map-legend">
  <span class="travel-map-key">
    <span class="travel-map-dot travel-map-dot--past"></span>
    Past
  </span>
  <span class="travel-map-key">
    <span class="travel-map-dot travel-map-dot--future"></span>
    Future
  </span>
</div>

<script>
document.addEventListener("DOMContentLoaded", function () {
  const locations = [
    {
      city: "Chemnitz, Germany",
      lat: 50.8278,
      lng: 12.9214,
      status: "past",
      items: [
        {
          title: "Workshop and Summer School on Applied Analysis 2023",
          date: "18–22 Sep 2023",
          kind: "summer school"
        }
      ]
    },
    {
      city: "Berlin, Germany",
      lat: 52.5200,
      lng: 13.4050,
      status: "past",
      items: [
        {
          title: "OT-DOM 24",
          date: "2024",
          kind: "posters"
        }
      ]
    },
    {
      city: "Luminy / Marseille, France",
      lat: 43.2315,
      lng: 5.4410,
      status: "past",
      items: [
        {
          title: "Learning and Optimization in Luminy 2024",
          date: "17–21 Jun 2024",
          kind: "poster"
        },
        {
          title: "SIGMA'24",
          date: "28 Oct – 2 Nov 2024",
          kind: "poster"
        }
      ]
    },
    {
      city: "Columbia, South Carolina, USA",
      lat: 34.0007,
      lng: -81.0348,
      status: "past",
      items: [
        {
          title: "Applied and Computational Mathematics / RTG Data Science seminar, University of South Carolina",
          date: "30 Aug 2024",
          kind: "talk"
        },
        {
          title: "USC Mathematics Graduate Colloquium",
          date: "12 Sep 2024",
          kind: "talk"
        }
      ]
    },
    {
      city: "Los Angeles, California, USA",
      lat: 34.0689,
      lng: -118.4452,
      status: "past",
      items: [
        {
          title: "UCLA Level Set Seminar",
          date: "19 Aug 2024",
          kind: "talk"
        },
        {
          title: "Stan Osher's Level Set Seminar",
          date: "2025",
          kind: "talk"
        }
      ]
    },
    {
      city: "Hamburg, Germany",
      lat: 53.5511,
      lng: 9.9937,
      status: "past",
      items: [
        {
          title: "Conference on Mathematics of Machine Learning 2025",
          date: "22–25 Sep 2025",
          kind: "talk"
        }
      ]
    },
    {
      city: "Saint-Malo, France",
      lat: 48.6493,
      lng: -2.0257,
      status: "past",
      items: [
        {
          title: "GSI'25 — Geometric Science of Information",
          date: "29–31 Oct 2025",
          kind: "talk"
        }
      ]
    },
    {
      city: "Oberwolfach, Germany",
      lat: 48.3160,
      lng: 8.2160,
      status: "past",
      items: [
        {
          title: "MFO workshop: Flows on Measure Spaces and Applications in Machine Learning",
          date: "22–27 Mar 2026",
          kind: "workshop"
        }
      ]
    },
    {
      city: "Madrid, Spain",
      lat: 40.4168,
      lng: -3.7038,
      status: "future",
      items: [
        {
          title: "Visit to Joaquín Míguez' group",
          date: "17–21 Nov 2026",
          kind: "research visit"
        }
      ]
    }
  ];

  const map = L.map("travel-map", {
    scrollWheelZoom: false,
    worldCopyJump: true
  });

  L.tileLayer("https://tile.openstreetmap.org/{z}/{x}/{y}.png", {
    maxZoom: 19,
    attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
  }).addTo(map);

  const bounds = [];
  const colors = {
    past: "#2b6cb0",
    future: "#c53030"
  };

  locations.forEach((loc) => {
    const popupList = loc.items.map((item) => {
      return `
        <li>
          <strong>${item.title}</strong><br>
          <span class="travel-map-meta">${item.date} · ${item.kind}</span>
        </li>
      `;
    }).join("");

    const marker = L.circleMarker([loc.lat, loc.lng], {
      radius: 8,
      color: colors[loc.status],
      fillColor: colors[loc.status],
      fillOpacity: 0.85,
      weight: 1.5
    }).addTo(map);

    marker.bindPopup(`
      <div class="travel-map-popup">
        <strong>${loc.city}</strong>
        <ul>${popupList}</ul>
      </div>
    `);

    bounds.push([loc.lat, loc.lng]);
  });

  map.fitBounds(bounds, {
    padding: [35, 35]
  });
});
</script>
