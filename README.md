Description: 
Build up a simple network visualization prototype, which accepts weighted network graph data as input (formatted in JSON, as attached “test_graph.json”), and show the corresponding network diagram (with nodes and connecting links).

Note:
	This prototype should have at least the following features:
####1	Basic readability:
#####1.1	the nodes should be displayed with their labels so one may identify each of them;
#####1.2	the label (i.e. the weight) of the links among nodes should be included, but not necessarily be displayed UNLESS one clicks on them (or hover);
#####1.3	one should be able to find the difference between two links with unequal weight: for example, in the test_graph, link (4, 1, weight=80) can be more “thick” compared to link (1, 2, weight=10) in the resulting display (or you may set heavier links as color red while lighter links with color blue, but discuss with me first);
#####1.4	one should be able to zoom in/out while visualizing the graph.
What’s more, it will be better if:
####2	One is able to interact with the resulting diagram, like dragging and moving the nodes for better visualization.

Tools and resources you need:
####1	The Python script (“generate_test_graph.py”) provides you a simple tool for generating a weighted network graph. However you do NOT need to take care of the generation of network data. Refer to https://networkx.readthedocs.io/en/stable/reference if you really need to look into the generation of network data.
####2	For building the prototype, there are 2 possible solutions listed as follows:
#####2.1	D3.js: https://d3js.org/ provides the features that you can import the JSON formatted network data and make visualization on it. An example is https://bl.ocks.org/mbostock/4062045 
#####2.2	plotly: https://plot.ly/python/ is another possible solution, but may seem a bit complex. You are suggested to use D3.js but feel free if you would like to turn to plotly (discuss with me first).
####3	The current goal is to build up the effective visualization for the network given in “bpic2012_network.json” as attached.


已实现：
1.	Node 显示label
2.	Link在hover时候能显示数值
3.	Link根据数值不同粗细不同
4.	图能够进行拖拽

待优化
1.	Link和node的颜色等可以修改
2.	能拖拽图的节点，但是效果暂时不是很好


注意： d3文件夹是库文件，source是源文件。直接使用firefox和edge均可打开model.html，但是chrome貌似不支持。
