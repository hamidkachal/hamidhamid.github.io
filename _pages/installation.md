# lj-folio

## A [Jekyll](https://jekyllrb.com/) theme for academic sites. 

[![license](https://img.shields.io/github/license/mashape/apistatus.svg?maxAge=2592000)](https://github.com/LuckyJimJD/CourseSiteTheme/blob/master/LICENSE)

This theme is based on [alshedivat/al-folio](https://github.com/alshedivat/al-folio). It is designed for use as a simple personal or course website. 

### Demos 

#### Personal site with pages for publications and courses taught

[![demo 1](https://img.shields.io/badge/theme-demo-brightgreen.svg)](https://LuckyJimJD.github.io/lj-folio/)

#### Course site with pages for syllabus, course materials, and links to external resources

[![demo 2](https://img.shields.io/badge/theme-demo-brightgreen.svg)](https://LuckyJimJD.github.io/lj-teaching-template/)

## Installation 

1. Fork theme from `https://github.com/LuckyJimJD/CourseSiteTheme`to `github.com:<your-username>/<your-repo-name>`. 

2. Clone to local system. 

3. Edit _config.yml: 

You must include at least the 'url', 'baseurl', 'title' & 'name' variables: 
    ```
    url: http://username.github.io # change 'username' to your github username; if your github.io site directs to a custom URL, use that instead. 
    baseurl:  /repository/ # change 'repository' to your github repository name; be sure to keep the leading and trailing '/'. 
	title: 'Site Title' # change 'Site Title' to the title of your site as you want it to appear on the 'About' page and in the header of other pages . 
	name: 'Author Name' # change 'Author Name' to your name as you want it to appear on 'About' page and elsewhere. 
    ```
The remaining variables ('position', 'affiliation', etc.) are optional but should be included if you want this information to appear on the 'About' page or elsewhere in your site. Replace contents with your information. 

4. Edit _layouts/default.html & _layouts/about.html 

Delete Statcounter code 

- If you use Statcounter or other site tracker, insert code for your site as directed. 


5. Edit other content:

The '_data' folder has YAML files with information to populate the 'About', 'Scholarship' & 'Teaching' pages. You can modify these and add other pages for the content you want to include in your site. 

To create a gallery page (like the 'teaching' page here):

- Add images to 'assets/img'
	- File names should follow the pattern 'RepoName.png' (or 'RepoName.jpg'), replacing 'RepoName' with the name of the repository for the site you want to link to and using the appropriate extension for the image format. 
	- You can organize images in subfolders as desired. 
- Create a YAML file in the '_data' folder, following the example of '_data/classes.yml' in this repository. 
- Create a new page (in the '_pages' folder), following the example of '_pages/teaching.md', substituting the fields in your YAML data file. 
	- If your gallery images are in subfolders under 'assets/img', be sure to include the subfolder in the 'src' path. 

To create an index page (like the 'scholarship' page here): 

- Create a YAML file in the '_data' folder, following the example of '_data/scholarship.yml' in this repository. 
- Create a new page (in the '_pages' folder), following the example of '_pages/scholarship.md', substituting the fields in your YAML data file. 

To include navigation links to pages in the site header, edit the '_data/pages.yml' file. That file is used to auto-populate the navigation links in the site header ('_includes/header.html').

6. Commit changes in git and then push to [GitHub Pages]((https://pages.github.com/).

### Modifying Theme Style 

Fonts, font sizes, spacing, colors, etc. are set using variables (`$variable_name`) in the `_sass/variables.scss` file. 

To use Google webfonts, replace the code in `_includes/head.html` with the appropriate code for your fonts and then edit the font variables in '_sass/variables.scss' to use your preferred font names. 

## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
