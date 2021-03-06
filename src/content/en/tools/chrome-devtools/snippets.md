project_path: /web/tools/_project.yaml
book_path: /web/tools/_book.yaml
description: Snippets are small scripts that you can author and execute within the Sources panel of Chrome DevTools. You can access and run them from any page. When you run a snippet, it executes from the context of the currently open page.

{# wf_updated_on: 2018-05-03 #}
{# wf_published_on: 2015-10-12 #}
{# wf_blink_components: Platform>DevTools #}

# Run Snippets Of Code From Any Page {: .page-title }

{% include "web/_shared/contributors/kaycebasques.html" %}

Snippets are small scripts that you can author and execute 
within the Sources panel of Chrome DevTools. You can access and run them 
from any page. When you run a snippet, it executes from the context of the 
currently open page.

If you have small utilities or debugging scripts which you find yourself 
using repeatedly on multiple pages, consider saving the scripts as snippets. 
You can also use snippets as an alternative to 
[bookmarklets](https://en.wikipedia.org/wiki/Bookmarklet).


### TL;DR {: .hide-from-toc }
- Snippets are small scripts that you can run from any page (similar to bookmarklets).
- Run portions of snippets in the Console with the "Evaluate in Console" feature.
- Remember that popular features from the Sources panel, like breakpoints, also work with snippets.


## Create snippet

To create a snippet, open the **Sources** panel, click on the **Snippets** tab,
right-click within the Navigator, and then select **New**.

![create snippet](images/create-snippet.png)

Enter your code in the editor. When you have unsaved changes, your script
name has an asterisk next to it, like in the screenshot below. 
Press <kbd>Command</kbd>+<kbd>S</kbd> (Mac) or <kbd>Ctrl</kbd>+<kbd>S</kbd>
(Windows, Linux) to save your changes. 

![unsaved snippet](images/unsaved-snippet.png)

## Run snippet

There are three ways to run your snippet: 

* Right-click on the snippet filename (in the pane on the left that lists
  all your snippets) and select **Run**.
* Click the **Run** button (![run snippet 
  button](images/run.png){:.inline}).
* Press <kbd>Command</kbd>+<kbd>Enter</kbd> (Mac) or 
  <kbd>Ctrl</kbd>+<kbd>Enter</kbd> (Windows, Linux).

To evaluate a portion of your snippet in the Console, highlight the 
portion, right-click anywhere in the editor, and select **Evaluate in 
Console**, or use the keyboard shortcut 
<kbd>Command</kbd>+<kbd>Shift</kbd>+<kbd>E</kbd> (Mac) or
<kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>E</kbd> (Windows, Linux).

![evaluate in console](images/evaluate-in-console.png)

## Set breakpoints

Just like other scripts, you can set breakpoints on snippets. See
[Pause Your Code With
Breakpoints](/web/tools/chrome-devtools/debug/breakpoints/breakpoints)
to learn how to add breakpoints from within the **Sources** panel.

## Feedback {: #feedback }

{% framebox width="auto" height="auto" enable_widgets="true" %}
<script>
var label = '/web/tools/chrome-devtools/snippets';
var title = '[feedback] ' + label;
var url = 'https://github.com/google/webfundamentals/issues/new?title=' + title;
var link = '<a href="' + url + '">open an issue</a>';
var response = 'Thanks for the feedback. Please ' + link + ' and tell us how we can improve.';
var feedback = {
  category: "Helpful",
  question: "Was this page helpful?",
  choices: [
    {
      button: {
        text: "Yes"
      },
      response: response,
      analytics: {
        label: label,
        value: 1
      }
    },
    {
      button: {
        text: "No"
      },
      response: response,
      analytics: {
        label: label,
        value: 0
      }
    }
  ]
};
</script>
{% include "web/_shared/multichoice.html" %}
{% endframebox %}
