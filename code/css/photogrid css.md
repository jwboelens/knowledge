<ul class="photos">
  {{ range .Pages }}
    <li>
      <a href="{{ .Permalink }}"><img src="https://cdn.jwboelens.org{{ .Params.photo }}?width=400&aspect_ratio=3:2&quality=50"></a>
    </li>
  {{ end }}
</ul>

/* Photos */
.photos {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    list-style: none;
    grid-column-gap: 10px;
    grid-row-gap: 4px;
    padding: 0;
}
.photos img {
    width: 100%;
    margin-bottom: 0;
}
}
