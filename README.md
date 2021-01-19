
 <h1>  Introduction </h1>
 
  this is a WordPress plugin for user writes the movies review. In this plugin, user needs to put release year, director, IMDb link, photo and rating.
 it is can let the user manage the post with the content. 
 
 <h1> Requirements</h1>
 user need to have to download a plugin called Meta Box. it will show when the user installed this movies reviews plugin.
 Meta Box proves a better user interface for custom options. therefore I added in this movies reviews plugin.
 
<h1> Recommended modules</h1>
 This module requires no modules.
 
<h1>  Installation</h1>
 Install as you would normally install a WordPress plugin. 
 put the zip file into plugin
 
<h1>  Configuration</h1>
 The module has no menu or modifiable settings. There is no configuration. When
enabled, the module will prevent the links from appearing. To get the links
back, disable the module and clear caches.

 <h1>  Troubleshooting</h1>
 If the post information does not display, check the following:
 
 check the themes what you use 
 
 check the content.php of the themes 
 
 add 

     `the_meta();`
  
 into `<div class="entry-content">` 
 
 sample: 
 ```
 	<div class="entry-content">
		<?php
		the_content();
		the_meta();
		wp_link_pages(
			array(
				'before'   => '<nav class="page-links" aria-label="' . esc_attr__( 'Page', 'twentytwentyone' ) . '">',
				'after'    => '</nav>',
				/* translators: %: page number. */
				'pagelink' => esc_html__( 'Page %', 'twentytwentyone' ),
			)
		);
		?>
	</div><!-- .entry-content -->
 ```
 
 <h1>  FAQ</h1>
<h1>  Maintainers</h1>
Code Reference: https://developer.wordpress.org/reference/functions/register_post_type/ <br />
Developer Resources: https://developer.wordpress.org/resource/dashicons/#html  <br />
Code Reference : https://developer.wordpress.org/reference/functions/flush_rewrite_rules/ <br />

