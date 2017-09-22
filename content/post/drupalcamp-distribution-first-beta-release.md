---
title: "Drupal Camp Distribution: First Beta Release"
date: 2016-11-14
tags: ["drupal", "planet", "open source"]
---

<p><a href="http://www.drupal.org/project/drupalcamp">DrupalCamp</a>&nbsp;is the distribution, for spinning up camp sites. &nbsp;Lately, as always :), I was part of the site building team at a local camp in India and after working with the team, found that all the sites were/are having similar content architecture e.g. content types, listing pages etc., except their themes and designs.</p>

<p>While sprinting at DrupalCamp Pune, we decided to build a site for DrupalCamp Delhi. While sprinting we realised we need &nbsp;a common code/feature base for camp sites. And there we started building distribution in D8. The time we started making this distribution profile Drupal 8 was in beta 16 and we are hoping to make first release candidate soon.</p>

<p>Drupalcamp comes up with the 2 contributed modules fb_likebox, twitter_block for the facebook and twitter share blocks in sidebar.</p>

<p>Configurations that this installation profile provides&nbsp;are:</p>

<ol><li dir="ltr">
	<p>Content types</p>

	<ol><li dir="ltr">
		<p>Basic Page&nbsp;: &nbsp;For creating basic pages like about us,etc. on the site.</p>
		</li>
		<li dir="ltr">
		<p>Session&nbsp;: This is used for creating/submitting sessions.</p>
		</li>
		<li dir="ltr">
		<p>Sponsor&nbsp;: This is used to keep information about the sponsors.</p>
		</li>
	</ol></li>
	<li dir="ltr">
	<p>Listings (Views):</p>

	<ol><li dir="ltr">
		<p>Accepted Sessions</p>
		</li>
		<li dir="ltr">
		<p>Proposed Sessions</p>
		</li>
		<li dir="ltr">
		<p>Sponsors</p>
		</li>
		<li dir="ltr">
		<p>Students.</p>
		</li>
	</ol></li>
	<li dir="ltr">
	<p>Social sharing buttons:</p>

	<ol><li dir="ltr">
		<p>facebook</p>
		</li>
		<li dir="ltr">
		<p>twitter</p>
		</li>
	</ol></li>
	<li dir="ltr">
	<p>Blocks:</p>

	<ol><li dir="ltr">
		<p>facebook</p>
		</li>
		<li dir="ltr">
		<p>twitter</p>
		</li>
	</ol></li>
</ol><p>We need to just use the drupalcamp profile and theme the site.</p>

<p>Challenges that came up while building this profile&nbsp;:</p>

<ol><li dir="ltr">
	<p>Contributed modules : The contributed modules stable release was not out so ported the fb_likebox, twitter_block module to drupal 8 and created the stable release of&nbsp;<a href="http://www.drupal.org/project/fb_likebox">fb_likebox</a>. Special thanks to the maintainer&nbsp;<a href="https://www.drupal.org/u/baekelandt">baekelandt</a>&nbsp;for quick promptness.</p>
	</li>
	<li dir="ltr">
	<p>There was no tool available which will provide the boilerplate code, so we started with forking the standard profile and used the config-export to export the configurations.&nbsp;Now with the drupalconsole 0.9.9 we have&nbsp;<a href="https://github.com/hechoendrupal/DrupalConsole/releases/tag/0.9.9">generate profile</a>&nbsp;command available to &nbsp;generate the boilerplate code. Used the phing to automate the testing as sam specified in its&nbsp;<a href="https://codedrop.com.au/blog/test-driving-drupal-8-writing-install-profile">blog</a>.</p>
	</li>
</ol><p>Thanks to the entire Drupalcamp Distribution Team!</p>

<p>What's Next ?</p>

<p>Please join hands to release the stable version for&nbsp;<a href="https://www.drupal.org/project/twitter_block">twitter_block</a>&nbsp;and include this stable release in the drupalcamp distribution.</p>