## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/chirag-vithlani/family-tree/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Organization Chart Plugin</title>
  <link rel="icon" href="https://dabeng.github.io/OrgChart/img/logo.png">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/orgchart/2.1.9/css/jquery.orgchart.min.css">
  <link rel="stylesheet" href="https://dabeng.github.io/OrgChart/css/style.css">
</head>
<body>
  <div id="chart-container"></div>

<script type="text/javascript" src="https://code.jquery.com/jquery-3.5.1.min.js"></script>
  <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/orgchart/2.1.9/js/jquery.orgchart.min.js"></script>
  <script type="text/javascript">
    $(function() {

    var datasource = {
      'name': 'Kalidas',
      'children': [
        { 'name': 'Odhvaji' },
        { 'name': 'Hemraj', 'title': 'department manager',
          'children': [
            { 'name': 'Tie Hua', 'title': 'senior engineer' },
            { 'name': 'Hei Hei', 'title': 'senior engineer',
              'children': [
                { 'name': 'Dan Dan', 'title': 'engineer' }
              ]
            },
            { 'name': 'Pang Pang', 'title': 'senior engineer' }
          ]
        },
        { 'name': 'Hong Miao', 'title': 'department manager' }
      ]
    };

    $('#chart-container').orgchart({
      'data' : datasource,
      'nodeContent': 'title'
    });

  });
  </script>
  </body>
</html>

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/chirag-vithlani/family-tree/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
