# Setup folder:
keep api.js, utility.js in same folder
Keep sw.js file in root folder of project directory.

# For HTML:
1. add "utility.js" file
2. add "api.js"
3. in "sw.js" file update "utility.js" url path at utilityUrl variable. Ex: const utilityUrl = '/src/js/utility.js'
4. in "sw.js" at STATIC_FILES variable add your static file url like: index.php, boostrap, js, images.
5. For sync form submission for offline. have to use submitPostData().
Ex:
const url_to_submit = "http://localhost/create_post";
const post_data_as_object = { name: "AM", title: "Software developer" };
submitPostData(url_to_submit, post_data_as_object)
N.B.: Don't need to import sw.js in html

Every time change static file update sw.js VERSION variable
