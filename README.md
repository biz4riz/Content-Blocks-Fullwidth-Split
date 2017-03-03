# Content Blocks Fullwidth Split
Split content contained with fullwidth background color/image. 

<a href="http://biz4riz.com/development/github-projects/content-blocks-fullwidth-split/">View Demo</a>

<h3>Styles</h3>
```html

.row_flex {
  display: -ms-flexbox;
  display: -webkit-flex;
  display: flex;
  -ms-flex-wrap: wrap;
  -webkit-flex-wrap: wrap;
  flex-wrap: wrap;
}

.split_content.full .block {
  padding: 8rem 0 4rem;
  width: 100%;
}
@media (min-width: 570px) {
  .split_content.full .block {
    width: 50%;
  }
}
.split_content.full .block.bg_img {
  background-image: url("https://www.placecage.com/g/740/600");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
@media (min-width: 570px) {
  .split_content.full .block .wrap {
    margin: 0;
    max-width: 55rem;
  }
}
@media (min-width: 570px) {
  .split_content.full .block .wrap.left {
    float: left;
  }
}
@media (min-width: 570px) {
  .split_content.full .block .wrap.right {
    float: right;
  }
}
@media (min-width: 570px) {
  .split_content.full .block .wrap > div {
    padding: 0;
  }
}
```

<h3>Classes</h3>
Inset classes add padding, dictated by the number of columns set within the class, on either side of the element. 
inset_[breakpoint]_[columns]

Pull classes add margins, dictated by the number of columns set within the class, on the left side of the element. 
push_[breakpoint]_[columns]

Push classes add margins, dictated by the number of columns set within the class, on the left side of the element. 
push_[breakpoint]_[columns]

<h3>HTML</h3>
```html

// Adding .full to split content in case there are other content block sections that are not fullwidth

<section class="split_content full">	

	// Using Flexbox to split the columns and to display the content blocks at equal heights	
	
	<div class="row_flex">
		<div class="block bg_blue">
		
			// The class .right floats the content within the block to the right when the content block splits
		
			<div class="wrap right">
				<div class="inset_md_1 pull_md_1 pull_lg_2">
					<h3>Inceptos Condimentum Commodo</h3>
					<p>Nullam quis risus eget urna mollis ornare vel eu leo. Donec sed odio dui.</p>
					<p><img src="http://placehold.it/550x200" alt="[ALT TEXT HERE]" /></p>
					<p>Etiam porta sem malesuada magna mollis euismod. Vestibulum id ligula porta felis euismod semper.</p>
				</div>
			</div>
		</div>
		<div class="block bg_img">
		
			// The class .left floats the content within the block to the left when the content block splits
			
			<div class="wrap left">
				<div class="inset_md_1 push_md_1 push_lg_2">
					<h3>Donec id elit non mi porta gravida at eget metus.</h3>
					<p>Donec ullamcorper nulla non metus auctor fringilla. Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
					<p>Fill out and submit this form, and we’ll give you a downloadable bidding template and helpful information about being financially ready to take on multiple projects.</p>
				</div>
			</div>
		</div>
	</div>
</section>
```
