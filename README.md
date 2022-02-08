# Peer Feedback for statistics projects

## Adding peer feedback templates to project GitHub repos

### Making the template 

- Start by making issue templates that will go in the `project` repos. You can do this directly in GitHub or in your local `project` repo. You can find the issue templates I've used in the `issue-templates` folder. 

- If you've already created the repos, you can add them to the student repos using the `repo_add_file` function in the [**ghclass**](https://rundel.github.io/ghclass/articles/ghclass.html) R package. Example code is below: 

```r
repo_add_file(repo = repos,
              branch = "main",
              repo_folder = ".github/ISSUE_TEMPLATE",
              message = "Adding peer review template",
              file = "[FILE PATH]/01-peer-review-introduction.md", 
              overwrite = FALSE)
```

In this code 

- `repos` is a vector of the project repos
- `[FILE PATH]` is the location of the issue templates on your local computer. 

I haven't figured out a way to post all four templates simultaneously, so I just change the file name and run this code separately for each template.


## Opening a new issue

When students click to open a new issue in that GitHub repo, you should now see the option to use one of the templates.  It will look similar to this: 

![](img/issue-template.png)


## Instructions for students

[Click here](https://sta210-fa21.netlify.app/project/peer-review) for instructions from STA 210: Regression Analysis. It includes the peer review assignment and how to create the new issues.
