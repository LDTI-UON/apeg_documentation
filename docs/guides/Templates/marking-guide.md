# Marking Guide Example Template

``` html
<head>
<!-- imported from LMS -->
	{css_link_tags}
<style>
.contentPane {
	margin: 0 14px 0 14px;
}
.liItem {
	padding: 25px;
}
textarea {
	width: 22em;
	height: 5em;
}
table {
	min-width: 90% !important;
}
.datalist th {
  height: 20px !important;
  /*background-color: gray;*/
  color: white;
  padding: 8px;
}
.datalist td {
  height: 20px;
  padding: 8px;
}
.datalist tr:nth-child(odd) {
  background-color: rgb(196, 225, 234);
}
/* verification form styles*/
.p_ver {
	padding: 1.1em;
}
.p_ver > input {
  margin-left: 2em;
}
.not_matched {
	background-color: rgb(200, 155, 180);
}
p {
	margin-top: 0.5em;
	margin-bottom: 0.5em;
	font-size: 14pt;
}
</style>
    <title>Marking Impact</title>
</head>
<body class='lesson-plan-page'>

{if logged_in}
<div class='contentPane'>
<div class='contentBox' style='padding: 1em'>
		<h2>Marking impact:</h2>
<p>The grading will be from 1 - 5 with 5 being the highest. Marks will be averaged out to an overall peer assessment grade out of 5. Part marks will
be rounded up or down .1 - .4 rounded down and .5 - .9 rounded up.</p><p>
Therefore is you scored 34/40 your overall score would be 4.25 which would mean you would be awarded a score of 4. This means that you
would receive 3 additional marks on top of your group score for your communication audit. EG. Group score 21/25 – you would have a final
mark of 24/30.</p>
<p>
If you were scored 14/40 your overall score would be 1.75 which would mean you would be awarded a score of 2. This means that you would
have 3 marks deducted from your group score for your communication audit. EG. Group score 21/25 – you would have a final mark of 18/30.</p>
<p style='margin-left:3em'>
5 = Outstanding contribution, can't be faulted (awarded 5 marks on top of group mark)<br>
4 = Very good overall (awarded 3 marks on top of group mark)<br>
3 = Generally good (awarded the group project mark as assessed by the tutor)<br>
2 = Barely adequate overall (awarded the group mark minus 3 marks)<br>
1 = Generally inadequate overall (awarded the group mark minus 5 marks)<br>
</p>
<p>
This means that if the group mark is allocated by the tutor as 22/25, a group member judged by group peers as making an outstanding
contribution will receive 27/30 as the final assessment mark (group mark plus 5 marks). A group member judged by group peers to have made
a generally inadequate overall contribution would receive 17/30 for the same group assignment (group mark minus 5 marks).</p>

<a href='javascript: {window.history.back()}'>&larr; Back</a>
{if:else}

<p>You are not logged in.</p>
{/if}

</div>
</div>
```
