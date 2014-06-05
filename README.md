jquery.connectingLine
=====================

This jQuery Plugin helps to connect two elements with a line. 
Any two elements on the page can be connected with a line using this plugin. We just have to give Element ID or class which should be connected.

SVG images are created to show connected line. On Resize of the Screen or Repositioning the element will regenrate the line between elements.

Here is an example step by step :

Step - 1 :
Required files- 
required/script/jquery-1.11.0.min.js
required/script/jquery.svg.min.js
required/script/jquery.connectingLine.js
<script type="text/javascript" src="required/script/jquery-1.11.0.min.js"></script>
<script type="text/javascript" src="required/script/jquery.svg.min.js"></script>
<script type="text/javascript" src="required/script/jquery.connectingLine.js"></script>


Step - 2 :
Create a SVG Connecting Line object.
<script type="text/javascript">
var mySVG = $('body').connectSVG();
</script>

Step - 3 :
Give the left_node and second_node as First node and Second Node respectively. These are mandatory fields.
There are few other parameters you can pass to customize your connecting line.

//Options
left_node - Left Element by ID - Mandatory
right_node - Right Element ID - Mandatory
status - accepted, rejected, modified, (none) - Optional
style - (dashed), solid, dotted - Optional	
horizantal_gap - (0), Horizantal Gap from original point
error - show, (hide) - To show error or not

<script type="text/javascript">
		mySVG.drawLine({
			left_node:'.node1',
			right_node:'.node2',
		});
</script>
