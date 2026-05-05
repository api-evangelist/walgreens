---
title: "Changes to Balance Rewards for Healthy Choices API"
url: "https://developer.walgreens.com/blog/changes-balance-rewards-healthy-choices-api"
date: "Tue, 20 Aug 2019 16:27:14 +0000"
author: "aschwein"
feed_url: "https://developer.walgreens.com/blog/rss"
---
<div class="field field-name-body field-type-text-with-summary field-label-hidden"><div class="field-items"><div class="field-item even"><p>Hello all,</p>
<p>We wanted to inform you about some changes we have made to the Balance Rewards for Healthy Choices (BRhc) API program. The API service contract is exactly the same and you still have the same workflow for authentication, tracking, and synchronizing the healthy choices activity data. However, there is one small change in that we have shortened the expiry time of auth_tokens, access token are now only valid for 24 hours, and refresh tokens are now valid for 90 days.</p>
<p>Since the inception of the BRhc API we have be measuring healthy outcomes from the aggregated activity data. We have even been innovating on our own Employee health plan as a result of this measurement to rewarding continuous achievements. Based on some research and the evidence based information we have decided to make a change to the entire BRhc API user rewarding mechanism.</p>
<p>So instead of only rewarding points for the synchronization of healthy activities data the user will have to select a 4-week lifestyle or 4-week physical challenge on the BRhc Dashboard and their data will get synchronized with your integration of the API.As new achievements with the dynamic challenges are completed the Balance Rewards member will continuously be rewarded with points. Once the 4-week challenge is completed the user will be able to spin a wheel for a bonus reward (it's an extremely rewarding moment) and sign up for a new challenge thereby helping further improve the healthy outcomes of the API.</p>
<p>You can see below the new rewards mechanism as we have listed them on our API documentation:</p>
<ul class="list-group"><li class="list-group-item">100 points each week a healthy challenge is completed; maximum of 400 points total per challenge</li>
<li class="list-group-item list-group-item-warning">NOTE: Members can join two challenges (one lifestyle challenge and one healthy activity challenge) simultaneously</li>
<li class="list-group-item list-group-item-success">BONUS: Complete all 4 challenge weeks to earn a prize wheel spin worth up to 2000 points</li>
<li class="list-group-item list-group-item-success">BONUS: 250 points for connecting a compatible health &amp; fitness device/app; up to 2 per month</li>
</ul><p>Thanks,</p>
<p>@WalgreensAPI</p>
</div></div></div>
