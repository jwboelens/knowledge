This css code transforms the 13px increments to actual stars. So 13px is one star, 26px is 2 stars, etc.

.star {
    width: 13px;
    height: 12px;
    display: inline-block;
    background: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTMiIGhlaWdodD0iMTIiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PHBhdGggZD0iTTYuMzA5IDkuMjJMMi40MDkgMTJsMS40NC00LjU2N0wwIDQuNTgzbDQuNzg4LS4wNDJMNi4zMDggMCA3LjgzIDQuNTRsNC43ODkuMDQ0LTMuODUgMi44NDlMMTAuMjA5IDEyeiIgZmlsbC1ydWxlPSJldmVub2RkIi8+PC9zdmc+);
}

U can use this code to generate the stars in your html.

<div class="star" style="width:13px"></div> : 1 star
<div class="star" style="width:26px"></div> : 2 stars
<div class="star" style="width:39px"></div> : 3 stars
<div class="star" style="width:52px"></div> : 4 stars
<div class="star" style="width:65px"></div> : 5 stars
