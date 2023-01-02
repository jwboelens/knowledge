Frontpage with different pieces of content. For instance, the latest blog posts and the latest photos.

```
<?php foreach (page('notes')->children()->listed()->sortBy('date', 'desc')->limit('3') as $note): ?>
	<a href="<?= $note->url() ?>"><date><?= $note->date()->toDate('Y-m-d') ?></date></a>
	<?= $note->text()->kt() ?>
<?php endforeach ?>
```

```
<?php foreach (page('photos')->children()->listed()->sortBy('date', 'desc')->limit('3') as $photo): ?>
	<?php if($image = $photo->image()): ?>
        <a href="<?= $photo->url() ?>">
   		<img src="<?= $image->crop(400,300)->url() ?>" alt="">
        </a>
    <?php endif ?>
<?php endforeach ?>
```
