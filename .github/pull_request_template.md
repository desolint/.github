#### [Title of the Jira Ticket](<[https://](https://desolint.atlassian.net/jira/projects)>)

[Description of the PR - Might be simpler/shorter version of Jira description or totally new description] - (Example below)

The shipping service provider is charging extra on order fulfillment based on actual weight. This PR is one part in the implementation of module to allow automatic recovery of the extra charges from the customer. Here this is a CSV file importing module to get the actual charges, and send it to the comparison module in the backend.

<br>


#### commits description

1. Create CSV upload modal [commit code](https://github.com/desolintdev/guidelines/pull/1/commits/edbb9d234d63280f82aa978bd3e53ec111dcfad0)
2. Send CSV data to the server [edbb9d2](https://github.com/desolintdev/guidelines/pull/1/commits/edbb9d234d63280f82aa978bd3e53ec111dcfad0)

<br>

##### Packages Changes (If Applicable)

Name: Installed `react-csv-reader` to read CSV files in the frontend
Effect: +20KB to the bundle size

<br>

##### Developers Checklist

###### Planning And Organizational Tasks
- [ ] I have included a proper description of the changes made in the Jira card
- [ ] I have put the Jira ticket number and title in the PR title
- [ ] I have included the Jira ticket link in the PR description
- [ ] I have included a proper description of the changes made in the PR
- [ ] I have included the commit descriptions and links in the PR description

###### Packages Changes
- [ ] I have included the packages changes in the PR description (if applicable)

###### Testing Tasks
- [ ] I have tested the changes locally
- [ ] I have tested the changes for responsiveness (if applicable)

###### Reviews Tasks
- [ ] I have responded responded to all the comments from all the AI Reviewers
- [ ] I have addressed all the comments of SonarCloud and similar
- [ ] I have addressed all the comments of Socket.dev and similar
- [ ] I have responded responded to all the comments from the reviewers
- [ ] All the comments are resolved

###### Security Tasks
- [ ] I have verified that all API responses contain only necessary fields
- [ ] I have verified all public endpoints for potential data leakage
- [ ] I have tested in browser network tab to confirm no sensitive data exposure
- [ ] I have verified that all the responses data is explicitly filtered/destructured before sending to client
- [ ] I have verified that all error responses do not expose any sensitive information
- [ ] I have reviewed the installed/modified packages profile in Socket.dev

<br>

##### Reviewer Checklist

###### Planning And Organizational Tasks
- [ ] I confirmed that the Jira card has full detailed description of the ticket and how to implement it OR the bug, it's reason and how it's fixed
- [ ] I confirmed that the PR has a proper description (minified version of the Jira card at least)


###### Reviews Tasks
- [ ] I have confirmed that all AI Reviewers comments are addressed


###### Security Tasks
- [ ] I have verified that all API responses contain only necessary fields
- [ ] I have verified all public endpoints for potential data leakage
- [ ] I have verified that all the responses data is explicitly filtered/destructured before sending to client
- [ ] I have verified that all error responses do not expose any sensitive information
- [ ] I have approved the authentication/authorization implementation
- [ ] I have validated security implications of any new endpoints
- [ ] I have confirmed proper data filtering throughout request lifecycle (each item only request and get what it needs, no oversharing)
- [ ] I have confirmed that the Least Privilege Principle is applied on every step ((each item only request and get what it needs, no oversharing)
- [ ] I have done a complete security review
- [ ] I have reviewed the installed/modified packages profile in Socket.dev
