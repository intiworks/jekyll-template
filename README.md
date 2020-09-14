# jekyll-template
Template for jekyll + netlify cms

Template made by Inti Rodriguez (intiworks.com) for Jekyll projects with Netlify CMS.
HOW TO USE:

-Clone repo to your pc. Install jekyll and ruby.

-To edit the main page, edit the files under the _includes folder and add/remove the links from _layouts/front.html

-To add/remove post categories, add a new folder "categoryname" and inside of it a new one called "_posts" -> 
   |
   |--index.html
   |--categoryfolder (example: "updates", "sections")
      |
      |--_posts
         |
         --.md files
  Then edit admin/config.yml and add new entries taking "sections" as example.
  Then, add a file named "categoryname.html" inside "_layouts". Take "section.html" as an example of how to write it.
  Finally, create "categorynameplural.html" inside "_includes". Take "sections.html" as an example of how to write it.
  Add a link to categorynameplural.html inside the includes of _layouts/front.html
  
-To simply add a new page in the domain.com/pagename fashion, edit the admin/config.yml file taking "about" as an example, and link to your html file here

-To add/remove posts (or sections), go to domain.com/admin and log in with github
   For this step, go to your cloned Github repo and enable Github Pages. 
   Then, go to netlify -> https://app.netlify.com/sites/your-site-name/settings/access -> OAuth -> Install provider
   In your Github account, go to https://github.com/settings/developers and go to OAuth - > New OAuth app
   Field Authorization Callback URL must be https://api.netlify.com/auth/done
   Copy client secret and ID, paste to Netlify Oauth Install provider thing
   Add your URL in _config.yml, take the one already there as example
   
-To add custom css styles, go to _includes/head.html and link them there. For example I created css/custom.css and linked it in that HTML file

Resources:

https://cnly.github.io/2018/04/14/just-3-steps-adding-netlify-cms-to-existing-github-pages-site-within-10-minutes.html
https://github.com/netlify/netlify-cms/blob/master/dev-test/config.yml
https://gist.github.com/maciejmatu/987563ede550e7b9f1644cd01882e6f5
https://github.com/adamwatters/jekyll-tutorial-with-netlify-cms/blob/master/about.md
https://www.netlifycms.org/docs/jekyll/
https://stackoverflow.com/questions/30205465/jekyll-including-a-post-inside-another-post
https://ben.balter.com/2015/02/20/jekyll-collections/
      
