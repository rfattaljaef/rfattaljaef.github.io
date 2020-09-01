---
#permalink: /
#title: "academicpages is a ready-to-fork GitHub Pages template for academic personal websites"
#excerpt: "About me"
#author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

This is the front page of a website that is powered by the [academicpages template](https://github.com/academicpages/academicpages.github.io) and hosted on GitHub pages. [GitHub pages](https://pages.github.com) is a free service in which websites are built and hosted from code and data stored in a GitHub repository, automatically updating when a new commit is made to the respository. This template was forked from the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/) created by Michael Rose, and then extended to support the kinds of content that academics have: publications, talks, teaching, a portfolio, blog posts, and a dynamically-generated CV. You can fork [this repository](https://github.com/academicpages/academicpages.github.io) right now, modify the configuration and markdown files, add your own PDFs and other content, and have your own site for free, with no ads! An older version of this template powers my own personal website at [stuartgeiger.com](http://stuartgeiger.com), which uses [this Github repository](https://github.com/staeiou/staeiou.github.io).

A data-driven personal website
======
Like many other Jekyll-based GitHub Pages templates, academicpages makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over -- just be sure to save the markdown files! Finally, you can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the academicpages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring academicpages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
ROBERTO N. FATTAL JAEF is an economist in the Macroeconomics and Growth team of the World Bank’s Research Department. His research interest cover various areas of macroeconomics, with a special emphasis on economic growth. Current and recent research topics include: 1) understanding the role of market distortions for firm level behavior, entrepreneurship, and long run macroeconomic outcomes; 2) investigating the micro and macro patterns of transition growth paths, 3) studying the role of credit for business cycle. Prior to joining the Bank, he worked at the International Monetary Fund’s Research department (2011-2013). He holds a Ph.D. in Economics from UCLA.

 **Research Interests**  Macroeconomics, International Macroeconomics, Economic Development.
 
 _Disclaimer_: the views expressed in this site are those of the author and do not necessarily represent those of the World Bank or World Bank policy.

# Publications

1. Size-Dependent Tax Enforcement and Compliance: Global Evidence and Aggregate Implications, with Pierre Bachas and Anders Jensen,  _Journal of Development Economics , vol. 140, September 2019_ 
[pdf](https://www.sciencedirect.com/science/article/abs/pii/S0304387818308447?via%3Dihub)

2. Taxing the Good? Distortions, Productivity, and Misallocation in Sub-Saharan Africa, with Xavier Cirera and Hibret Maemir, _World Bank Economic Review, August 2019_
[pdf](https://academic.oup.com/wber/article-abstract/34/1/75/5543189)

3. Entry and Exit, Multi-Product Firms, and Allocative Distortions  _AEJ: Macroeconomics Vol 10 No. 2, April 2018_ 
[pdf](https://www.dropbox.com/s/n4jidqig6iugkjx/AEJ_published_version.pdf?dl=0)

4. The Anatomy of a Credit Crunch: from Capital to Labor Markets, with Francisco Buera and Yongseok Shin, Review of Economic Dynamics, January 2015
[pdf](https://pages.wustl.edu/files/pages/imce/yshin/bfs.pdf)

5. Entry, Trade Costs and International Business Cycles with Jose Ignacio Lopez,  Journal of International Economics 94 (2014), 224-238
[pdf](https://www.dropbox.com/s/7avntiqo8igs2ph/JIE_final.pdf?dl=0)

# Under Review

1. The Dynamics of Development: Innovation and Reallocation, with Francisco Buera, Revise and Resubmit AEJ: Macroeconomics
[pdf](https://www.dropbox.com/s/50g7e2ilco1sf98/draft_January_2020.pdf?dl=0)

2. Entry Barriers, Idiosyncratic Distortions, and the Firm-Size Distribution, June 2020 (updated!), reject-resubmit at AEJ:Macroeconomics 
[pdf](https://www.dropbox.com/s/m9bl786d4gwtocx/draft_july_2020.pdf?dl=0)

# Working Papers

* The Economic Ripple Effects of Covid-19, with Francisco Buera, Hugo Hopenhayn, Andy Neumeyer, and Yongseok Shin, June 2020
 [pdf](https://www.dropbox.com/s/mx0qifbgiwi6650/Ripples.pdf?dl=0)

* The Missing Middle in a Broad Cross-Section of Indian Establishments, with Francisco Buera, Reiki Laski, and Nicholas Tracther, in progress

* Constrained-Efficiency and the Welfare Effects of Misallocation with Hugo Hopenhayn, November 2019
 [pdf](https://www.dropbox.com/s/6yrutojvg68x26z/Constrained_Efficiency_Nov2019.pdf?dl=0)

* The Elusive Missing Middle: The Size Distribution of Firms in Sub-Saharan Africa, Xavier Cirera, Hibret Maemir, and Nicolas Gonne, in progress


