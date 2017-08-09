# githubprofilething
Click 'Show more activity' on your github profile until there is no more!
**Why?** it's nice to see everything in one place

## I'm sorry github, is this abuse?
Open up your public github profile, fire up Chrome dev tools or similar, open the console and inject away:

## Inject me
```
window.setInterval(function(){var elements = document.getElementsByClassName('contribution-activity-show-more'); if (elements.length) { elements[0].click(); }}, 1800);
```

## Output expected
Your browser will click the 'Show more activity' button every 1800ms until the button is no longer in the DOM, at which point you'll have your entire github history as one page which you can download as a PDF or print or search using `cmd + f` or `ctrl + f` in most browsers to find a commit, pull, or whatever.

