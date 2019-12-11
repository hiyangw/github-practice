# Automation

You can use query parameters to share URLs with customized information.

Query parameters are optional parts of a URL you can customize to share a specific web page view, such as search filter results or an issue template on GitHub. To create your own query parameters, you must match the key and value pair.

## Query Parameters

You must have the proper permissions for any action to use the equivalent query parameter. For example, you must have permission to add a label to an issue to use the `labels` query parameter.

If you create an invalid URL using query parameters, or if you don’t have the proper permissions, the URL will return a `404` error page.

### Supported query parameters

| Query parameter | Example |
|:---------------:|:-------:|
| body | https://github.com/octo-org/octo-repo/compare/master...pull-request-test?quick_pull=1&body=Fixes+the+problem. creates a pull request, comparing the branches master and pull-request-test, with the comment "Fixes the problem" in the pull request body. |
| title | https://github.com/octo-org/octo-repo/issues/new?labels=bug&title=New+bug+report creates an issue with the label "bug" and title "New bug report." |
| labels | https://github.com/octo-org/octo-repo/compare/master...pull-request-test?quick_pull=1&labels=bug creates a pull request, comparing the branches master and pull-request-test, with the label "bug." |
| template | https://github.com/octo-org/octo-repo/issues/new?template=issue_template.md creates an issue with a template in the issue body. |
| milestone | https://github.com/octo-org/octo-repo/issues/new?milestone=testing+milestones creates an issue with the milestone "testing milestones."
| assignee | https://github.com/octo-org/octo-repo/issues/new?assignee=octocat |creates an issue and assigns it to @octocat. |
| projects | https://github.com/octo-org/octo-repo/issues/new?title=Bug+fix&projects=octo-org/1 creates an issue with the title "Bug fix" and adds it to the organization's project board 1. |
