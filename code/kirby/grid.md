Create a photo / project grid:

```
.projects {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  list-style: none;
  grid-column-gap: 1.5rem;
  grid-row-gap: 2rem;
}
.projects img {
  width: 100%;
  margin-bottom: 0;
}
```

```
<ul class="projects">
    <?php foreach ($page->children()->listed()->sortBy('date', 'desc') as $photo): ?>
        <li>
        <?php if($image = $photo->image()): ?>
 
        	<a href="<?= $photo->url() ?>">
   					<img src="<?= $image->crop(400,300)->url() ?>" alt="">
            <figcaption><?= $photo->title() ?></figcaption>
        	</a>
        
        <?php endif ?>
      </li>
   <?php endforeach ?>    
</ul>
```
