This is the documentation for the 3D force directed graph visualization project.



The project is written in pure javascript, HTML and CSS , with the aid of this library:
https://github.com/vasturiano/3d-force-graph

which is built on top of Three.js



these libraries are included in the HTML file simply like that:

    <script src="//unpkg.com/three"></script>

    <script src="//unpkg.com/three-spritetext"></script>

    <script src="//unpkg.com/3d-force-graph"></script>



==========================================================================================================================



To host the project right away go to hosting_files folder, there's 2 files: graph.html and data.json


These are the 2 files you need to host, you must also provide the url of the data.json file in the DATA_URL variable in the HTML file.

(line number 102 in graph.html file, set the variable DATA_URL to the url of your json file in your hosting).



==========================================================================================================================



In case you want to provide new data, put the CSV file in the python_script folder and make sure to name it data.csv, and run the script from the command line like the following:

python script.py



and it will output a json file called data.json in the same folder.


make sure you're using python 3 not python 2, and that you have numpy and pandas libraries installed.



==========================================================================================================================



Simple example of data.json:

to understand how the graph is drawn using the file data.json lets give this example json file:

nodes = [

	{id : a},

	{id: b},

	{id: c}

	]



links = [{source: a, target: b},

	 {source: c, target: b}]



this will draw a graph of 3 nodes and 2 links.


you can also include other fields in the nodes or links array, and access them inside the HTML file.



===========================================================================================================================



For any questions, you can contact me at: gmelkabany@gmail.com


Mostafa.