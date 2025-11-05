---
layout: essay
type: essay
title: "Final Project Idea"
date: 2025-11-04
labels:
  - Software Engineering
  - Nextjs
---

<figure style="float: right; margin-left: 20px; margin-bottom: 10px; text-align: center;">
  <img src="../img/lostandfound.png"
       width="400"
       alt="UH Manoa Lost and Found Page"
       style="border: 1px solid #ccc; border-radius: 10px; padding: 4px;">
  <figcaption><em>(UH Manoa's Current Lost and Found Page)</em></figcaption>
</figure>

## Manoa Lost & Found
Proposers: Jermaine Bruno, Michael Lau, Brandon Nguyen, Edward Uzueta

## Overview
The Problem:<br>Throughout the semester, students at UH Manoa may lose countless items such as IDs, water bottles, textbooks, or even valuables such as their AirPods or other electronic devices. UH Manoa does have a Lost & Found system, but the current process consists of manually emailing departments, visiting physical locations like Campus Center, and making phone calls to said offices. It can be very inconsistent and students have no way of knowing when or if their items have been found without repeating this process numerous times.
<br>
<br>
The Solution:<br>**Manoa Lost & Found** would be a **digital platform for posting, searching, and aiding in the recovery of lost items** on the UH campus. Users will be able to create posts for their lost items, adding images, tagging potential lost-at-locations, as well as leaving their contact information. For users that have found lost items, they will also be able to create posts for items that they have found, including images, and will be prompted to return the item to official UH offices such as Campus Center. It connects finders and owners directly by UH authentication, organized item listings, improving lost-item recovery efficiency.
<br>
## Approach
For this app, we will create a campus-wide, unified way to **report, browse, and recover** lost items at UH Manoa. There are three roles: **Users** (students/staff) who can log in to report items they have lost and search/browse through found items; **Finders** (any logged-in user who posts a found item) who can create "found" listings and are guided to turn items in to official UH collection points; and **Admins** (Campus Center/Library or designated staff) who can verify items, manage flags/duplicates, and mark items as **recovered**.

The Manoa Lost and Found app will provide an easy-to-use directory of lost and found items reported across campus. In addition to organizing listings by **status** (Lost vs. Found) and **category** (Electronics, IDs, Books, Clothing, Misc), you can also organize and filter data by **location** (last seen/turned in), **date**, and **keywords** to speed matching.

Users should be able to:
- Create **Lost Item** reports with photo, category, description, last-seen time/place, and optional distinguishing details
- Set **alerts/preferences** (e.g., keywords like "Hydroflask," categories, or buildings) so they can be shown a feed of suggested matching **Found** posts when they appear
- View a personalized dashboard with "My Lost Items," "My Found Items," and **Matches and Alerts**

Finders should be able to:
- Create **Found Item** posts with photo, where/when it was found, and where it was **turned in**
- See a **"How to turn in items"** page with instructions for official UH offices (e.g., Campus Center, Library)
- If they spot a matching **Lost** post, they can send a notification to the owner **without arranging private handoffs** (owner retrieves the item from the official office)

Admins should be able to:
- **Verify** items turned in at official locations and update the status of items (e.g., _Received at Campus Center, Ready for Pickup, Recovered_)
- **Flag** duplicate posts, moderate content, and manage role assignments
- Configure campus **drop-off** locations with hours and contact info

To encourage safe recovery and deter theft, **all physical returns should flow through official UH offices**. Messaging exists only to confirm a likely match and inform the owner **where** the item was turned in.

## Mockup page ideas
- Landing page
- Feed (tabs for Lost and Found, quick filters by category/location/date
- Dashboard (My Lost Items, My Found Items, Matches & Alerts)
- Post Lost Item (photo upload, category, description, last-seen location/time)
- Post Found Item (photo upload, category, description, turned-in location)
- Item Details page (photo, description, location information, status, "Notify Owner" or "Message via UH email")
- Recovery Instructions page
- Admin home page
- Locations & Offices page
- Search & Advanced Filters

## Use case ideas
- New user (student) visits the landing page and clicks "Log in with UH." After authentication, they are brought to their personal dashboard with tabs for "Lost" and "Found."
- User reports a lost item, filling in the required details for a post such as: _Category - Bottle, Description - Blue Hydroflask with straw and dog stickers, Last seen: POST Room 318, uploaded photo_.
- The listing appears in the **Lost Items** feed and on their personal **My Lost Items** page.
- They receive notifications whenever similar "Found" posts are added
- Another user finds the item, logs in, and notifies the owner that the item was found and returned to Campus Center

## Beyond the Basics
<div style="overflow: auto;">
  <figure style="float: right; margin-left: 10px; margin-bottom: 10px; text-align: center;">
    <img src="../img/map.jpg"
         width="150"
         height="150"
         alt="UH Manoa Campus Map"
         style="border: 1px solid #ccc; border-radius: 10px; padding: 4px;">
    <figcaption><em>(UH Mānoa's Campus Map)</em></figcaption>
  </figure>
  
After implementing the basic functionality, here are ideas for more advanced features:

  <ul>
    <li>Implement a fuzzy-match search (perhaps using AI to match similar keywords such as “AirPods” to “Apple Earbuds” or “Wireless Headphones”).</li>
    <li>QR Poster Generator (allows users to print posters for campus bulletin boards with scannable links to their listings).</li>
    <li>Map integration (visual markers showing last-seen and found-item locations on campus).</li>
    <li>Automated clean-up (posts older than a set time period will be auto-archived unless renewed).</li>
    <li>Recovery metrics (display stats such as “123 items reunited this semester” to highlight community impact).</li>
  </ul>
</div>
<div style="clear: both; margin-bottom: 20px;"></div>
