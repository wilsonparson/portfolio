# Oldcastle Materials Customer Portal

## Summary
I redesigned and developed the front end of the Oldcastle Materials Customer Portal.

## Problem/Objective
The Oldcastle Materials Customer Portal is used by 45 of [Oldcastle Materials'](http://www.oldcastlematerials.com/) subsidiaries to allow their customers to make payments on materials and construction invoices. Oldcastle had outsourced the development of the front end of the portal, and it two major issues:

1. It was non-responsive (even though [Twitter Bootstrap](http://getbootstrap.com) was apparently being used)
2. It had very high CSS specificity (over 200 !important rules in a single CSS file)

Both of these issues were important to Oldcastle Materials, because (1) users had expressed frustration in not being able to make payments with mobile devices, and (2) each Oldcastle Materials subsidiary has its own version of the portal. Since each subsidiary has its own version, creating custom themes for each version becomes extremely time-consuming when the main CSS file has such high specificity.

`image of css specificity`

## Process

### 1. Heuristic Evaluation
I conducted a full-scale heuristic evaluation on the entire app, using [Nielsen's 10 heuristics for user interface design](https://www.nngroup.com/articles/ten-usability-heuristics/).

### 2. Information Architecture
I evaluated the information architecture of the app, and discovered that it could be simplified and consolidated.

`image of presentation`

### 3. Sketches & Mockups
I sketched new designs of each page and major component of the app, with at least two different iterations for every page/component.

 `images of sketches`

### 4. Development
I scrapped the CSS file, and rewrote the HTML, CSS, and Javascript (AngularJS & Kendo UI).

## Results
The portal now has a completely different overall structure and look, is responsive, and much more flexible for customization (so flexible, in fact, that only 3 CSS variables need to be declared for different portal themes).

`image of side by side comparison`
