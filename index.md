---
layout: default
landing: true
title: Home
order: -1
---

<section class="content medium">
	<div class="container">

		{% include /partials/major-heading headline="Aims & Actions" strapline="We have set specific goals for the society and this is how we aim to achieve them." %}
		<!--FB js-->
		<div id="fb-root"></div>
		<script>(function(d, s, id) {
		  var js, fjs = d.getElementsByTagName(s)[0];
		  if (d.getElementById(id)) return;
		  js = d.createElement(s); js.id = id;
		  js.src = "//connect.facebook.net/en_GB/sdk.js#xfbml=1&version=v2.8";
		  fjs.parentNode.insertBefore(js, fjs);
		}(document, 'script', 'facebook-jssdk'));</script>
		
		<div class="boxes">
			<section class="box">
				<h3>Demystify engineering</h3>
				<p>By having talks, discussions and group meet-ups to discuss various types of engineering.</p>
			</section>
			<section class="box">
				<h3>Remain inclusive</h3>
				<p>You do not have to identify as a women to attend our events, we welcome all 
				like-minded engineers.</p>
			</section>
			<section class="box">
				<h3>Break down stereotypes</h3>
				<p>By increasing exposure overall to the benefits of studying and working in engineering.</p>
			</section>
			<section class="box">
				<h3>Provide opportunities</h3>
				<p>By putting on regular events with industrial partners in order to forge connections and provide information.</p>
			</section>
		</div>

	</div>

</section>

<section class="content">
	<div class="container" style="text-align: center">
		<p>Find out more by visiting our committee page!</p>
		<ul class="actions">
			<li>
				<a href="{{ "/committee/" | prepend: site.base_url }}" class="button big">See the Committee</a>
			</li>
		</ul>
		<p>Or see what we have on at our events page!</p>
		<ul class="actions">
			<li>
				<a href="{{ "/events/" | prepend: site.base_url }}" class="button big">See the Events</a>
			</li>
		</ul>
		<br>
		<div class="fb-like" data-href="https://www.facebook.com/womeninengbristol/?ref=aymt_homepage_panel" data-width="165" data-layout="standard" data-action="like" data-size="small" data-show-faces="true" data-share="true"></div>

		<a href="https://twitter.com/WiE_Bristol" class="twitter-follow-button" data-size="large" data-show-count="false">Follow @WiE_Bristol</a><script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>
	</div>
</section>
