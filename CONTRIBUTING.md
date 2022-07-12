# Contributing Guidelines

Hi there! We're thrilled that you'd like to contribute to this project, your help is essential for keeping it great. Everyone is welcome to make suggestions on how this project can be improved. You can do this by either submitting an issue to report a bug or discuss a feature, or a pull-request to fix a bug or add a feature.


Contributions to this project are [released](https://help.github.com/articles/github-terms-of-service/#6-contributions-under-repository-license) to the public under the project's open source license.

Please note that this project is released with a Contributor Code of Conduct. By participating in this project you agree to abide by its terms.

### Did you find a bug or other issue?
- Ensure the bug or issue was not already reported by searching on the GitHub repository under issues.
- If your unable to find an issue addressing the problem, open a new one. Be sure to include a title and clear description, plus as much relevant information as possible.
- Use the [xdebug](https://xdebug.org/) extension for PHP if possible an provide the stack trace with the issue.
- For more detailed information about submitting a bug report or creating an issue, view the Reporting Guidelines below.

### Did you write a patch that fixes a bug or other issue?
- Open a new GitHub Pull Request with the patch
- Ensure the Pull Request description clearly describes the problem and the solution you are providing.
- Include the relevant issue number in the description by adding one of either "Fixes \#xx" or "Part of \#xx"
- Before submitting your pull request, please make sure you have followed the Pull Request Guidelines below.

### Do you intend to add a new feature or change an existing one?
- Suggest your change or addition by first creating an issue for discussion which you can then reference to later.
- Add the appropriate label to the issue: New Feature or Enhancement
- Submit a Pull Request containing the change you wish to contribute, ensuring you follow the Pull Request Guidelines below.

## Pull Request Guidelines
- Create a fork of the 'development' branch first, and make sure it's up to date. This helps to prevent conflicts from occuring. 
- Only pull requests to the development branch will be accepted. This ensures that any new code can go through the review process before it reaches the master.
- All commits and pull requests MUST reference a related issue in the comments. If a related issue doesn't exist, please first create a new one.
- Changes that are cosmetic in nature and don't add anything substantial to the stability or functionality of the project will generally not be accepted.
- Acceptance of pull requests is at the descretion of the project leader. All contributions to this repository will be appropriatly credited where possible.

### Code Style
Code should follow common practices and the standards as set out in this document. This includes:
- Indenting of code should consist of 4 spaces per indent, never tabs.
- Each file should contain an empty line at the end, be UTF-8 encoded, and use UNIX based line-endings.
- All new contributed code should be compatible with PHP v5.6 AND newer.
- All PHP files will use complete open tags (no shorthand php `<?=`).
- All functions, classes, variables will be documented in the code using the DocBlock format.
- Assume all user input will be malicious - properly sanitize all form entries and `$_GET`, `$_POST` and `$_COOKIE` variables.
- Avoid the use of ternery operators, espicially nested ones. They become too confusing to read.
- Minimize the use of double quotes. Double quotes force the PHP parser to check the string for variables to evaluate, even if there aren't any variables to evaluate. It is better to use single quotes and concatenate variables
- To make it easier for others to read and understand the code, it is recomended that you space out the code a bit more. An example is provided below:

```php
$concat_string = 'Some plain text and a ' . $variable;

if ( exampleFunction($variable) )
{
    $exploded = explode( $variable );
}
else
{
    $imploded = implode( $variable );
}

// Note the spacing around brackets.
// Curly braces should be on the following line to the 'if' or 'else' statements
```

### Submitting a pull request

0. Fork and clone the repository
0. Create a new branch: `git checkout -b my-branch-name`
0. Make your change, test your changes making sure everything works
0. Push to your fork and submit a pull request
0. Pat your self on the back and wait for your pull request to be reviewed and merged.

Here are a few things you can do that will increase the likelihood of your pull request being accepted:

- Follow standards for style and code quality
- Keep your change as focused as possible. If there are multiple changes you would like to make that are not dependent upon each other, consider submitting them as separate pull requests.
- Write a [good commit message](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html).

## Resources

- [How to Contribute to Open Source](https://opensource.guide/how-to-contribute/)
- [Using Pull Requests](https://help.github.com/articles/about-pull-requests/)
- [GitHub Help](https://help.github.com)
