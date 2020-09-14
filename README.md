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
      
