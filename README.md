# flask-demo
This demonstration shows how to integrate Flask with your HTML and JavaScript code for Project 2 in Data Analytics &amp; Visualization. 


Please clone this repository to your desktop and then do the following:

1. Navigate to the folder that contains ``app.py`` and launch a GitBash (Windows) or Terminal (Mac). 
2. Type ``source activate PythonData`` and then hit ENTER.
3. Type ``export FLASK_APP=app.py`` and then hit ENTER.
4. Type ``flask run`` and then hit ENTER.
5. Observe that the Flask server starts and tells you which port it's running on. Don't close this window.
6. With the Flask server running, enter this address in your Chrome browser: http://127.0.0.1:5000/. You'll see that it loads the index page. 
7. Click the link that says "Click here for the other page!" You'll notice that Chrome loads a new page containing a list of available routes. Be sure to view the link in the HTML to see how you specify this other page. It's different from what you might think!
8. If you navigate to the following address, you'll see that it returns a JSON: http://127.0.0.1:5000/dictionary. This is an example of an API endpoint you'd use to get data into your JavaScript file for graphing and analysis. 
9. If you navigate to the following address, you'll see that it returns another JSON, this time from a database query: http://127.0.0.1:5000/fighteraircraft This is another example of an API endpoint. Please read the code in ``app.py`` to see how this all works. 

Additional notes: 
* Please peruse my files and my directory structure to see how this all comes together.
* Note the use of the ``templates`` and ``static`` folders. 
* *NEW:* I've added some database queries. For these to work, you'll have to have the GlobalFirePower database we created in Week 9, Night 1, Activity 08-Stu_CRUD. If you don't have this database, you'll get unpredictable results.
* *IMPORTANT:* You'll have to update the PostgreSQL username and password (``app.py``) so that they match your own values. You likely have the same username, but your password will (probably) be different.
* You're using a Flask server, not LiveServer. **LiveServer doesn't play a role in this project**, and won't work properly with the Flask server. (Yes, you can use LiveServer for quick changes to your HTML, CSS, and page layout. But it won't properly serve your data to you, because it doesn't know how.)
* There's a wrinkle when trying to ``jsonify()`` the results of a MongoDB query. I'll eventually try to provide an example here, but please ask for help in the meantime.  
* *REMEMBER*: In the real world, your server would be running on a completely separate  machine, and the only way you could query its database is using these API endpoints. 

