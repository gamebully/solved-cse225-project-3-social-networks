Download Link: https://assignmentchef.com/product/solved-cse225-project-3-social-networks
<br>
This project is a programming assignment in C which aims to find influencer peaople in a social graph. Your program will read a data file containing a list of people names and the friendness they have. You will build a graph from the given data file. The vertices of the graph will be the people and there will be an edge between each person who have a friendness relationship.

You will process the graph and make the necessary calculations. The output of your program will be

<ol>

 <li>a representation of the graph you generated (can be viewed like adjacency matrix) and</li>

 <li>the centrality degrees .</li>

</ol>




The input will be in the following format:




Cem; Ayşe, Ferit, Dundar

Ayşe; Cem, Ferit, Dundar, Belma

Belma; Ayşe, Dundar, Edip

Edip; Belma, Dundar, Gamze

Dundar; Ayse, Belma, Cem, Ferit, Gamze, Edip

Gamze; Dundar, Edip, Ferit, Halit Ferit; Ayşe, Cem, Dundar, Gamze, Halit

Halit; Ferit, Gamze, Ilke

Ilke; Halit, Jale

Jale; Ilke

<ol>

 <li>a)  The output of your program must be in the following form:</li>

</ol>

As the output, the resulting graph can be displayed using either of the following formats:

As an adjacency matrix:

The first 2 rows have been done for you:

<table width="948">

 <tbody>

  <tr>

   <td width="102"> </td>

   <td width="74">Cem</td>

   <td width="79">Ayşe</td>

   <td width="86">Belma</td>

   <td width="77">Edip</td>

   <td width="91">Dundar</td>

   <td width="89">Gamze</td>

   <td width="77">Ferit</td>

   <td width="79">Halit</td>

   <td width="121">Ilke</td>

   <td width="73">Jale</td>

  </tr>

  <tr>

   <td width="102">Cem</td>

   <td width="74">0</td>

   <td width="79">1</td>

   <td width="86">0</td>

   <td width="77">0</td>

   <td width="91">1</td>

   <td width="89">0</td>

   <td width="77">1</td>

   <td width="79">0</td>

   <td width="121">0</td>

   <td width="73">0</td>

  </tr>

  <tr>

   <td width="102">Ayşe</td>

   <td width="74">1</td>

   <td width="79">0</td>

   <td width="86">1</td>

   <td width="77">0</td>

   <td width="91">1</td>

   <td width="89">0</td>

   <td width="77">1</td>

   <td width="79">0</td>

   <td width="121">0</td>

   <td width="73">0</td>

  </tr>

  <tr>

   <td width="102">Belma</td>

   <td width="74"> </td>

   <td width="79"> </td>

   <td width="86"> </td>

   <td width="77"> </td>

   <td width="91"> </td>

   <td width="89"> </td>

   <td width="77"> </td>

   <td width="79"> </td>

   <td width="121"> </td>

   <td width="73"> </td>

  </tr>

  <tr>

   <td width="102">Edip</td>

   <td width="74"> </td>

   <td width="79"> </td>

   <td width="86"> </td>

   <td width="77"> </td>

   <td width="91"> </td>

   <td width="89"> </td>

   <td width="77"> </td>

   <td width="79"> </td>

   <td width="121"> </td>

   <td width="73"> </td>

  </tr>

  <tr>

   <td width="102">Dundar</td>

   <td width="74"> </td>

   <td width="79"> </td>

   <td width="86"> </td>

   <td width="77"> </td>

   <td width="91"> </td>

   <td width="89"> </td>

   <td width="77"> </td>

   <td width="79"> </td>

   <td width="121"> </td>

   <td width="73"> </td>

  </tr>

  <tr>

   <td width="102">Gamze</td>

   <td width="74"> </td>

   <td width="79"> </td>

   <td width="86"> </td>

   <td width="77"> </td>

   <td width="91"> </td>

   <td width="89"> </td>

   <td width="77"> </td>

   <td width="79"> </td>

   <td width="121"> </td>

   <td width="73"> </td>

  </tr>

  <tr>

   <td width="102">Ferit</td>

   <td width="74"> </td>

   <td width="79"> </td>

   <td width="86"> </td>

   <td width="77"> </td>

   <td width="91"> </td>

   <td width="89"> </td>

   <td width="77"> </td>

   <td width="79"> </td>

   <td width="121"> </td>

   <td width="73"> </td>

  </tr>

  <tr>

   <td width="102">Halit</td>

   <td width="74"> </td>

   <td width="79"> </td>

   <td width="86"> </td>

   <td width="77"> </td>

   <td width="91"> </td>

   <td width="89"> </td>

   <td width="77"> </td>

   <td width="79"> </td>

   <td width="121"> </td>

   <td width="73"> </td>

  </tr>

  <tr>

   <td width="102">Ilke</td>

   <td width="74"> </td>

   <td width="79"> </td>

   <td width="86"> </td>

   <td width="77"> </td>

   <td width="91"> </td>

   <td width="89"> </td>

   <td width="77"> </td>

   <td width="79"> </td>

   <td width="121"> </td>

   <td width="73"> </td>

  </tr>

  <tr>

   <td width="102">Jale</td>

   <td width="74"> </td>

   <td width="79"> </td>

   <td width="86"> </td>

   <td width="77"> </td>

   <td width="91"> </td>

   <td width="89"> </td>

   <td width="77"> </td>

   <td width="79"> </td>

   <td width="121"> </td>

   <td width="73"> </td>

  </tr>

 </tbody>

</table>




b)Build your graph and calculate the following values, Degree centrality(20 points), Closeness centrality, Betweenness centrality(20 points).

<strong>Example: </strong>

<strong>Degree centrality:</strong> Degree centrality of a node refers to the number of edges attached to the node.  In order to know the standardized score, you need to divide each score by n-1 (n = the number of nodes).  Since the graph has 7 nodes, 6 (7-1) is the denominator for this question.

<table width="243">

 <tbody>

  <tr>

   <td width="48">Node</td>

   <td width="90">Score</td>

   <td width="105">StandardizedScore</td>

  </tr>

  <tr>

   <td width="48">1</td>

   <td width="90"> 1</td>

   <td width="105"> 1/6</td>

  </tr>

  <tr>

   <td width="48">2</td>

   <td width="90"> 1</td>

   <td width="105"> 1/6</td>

  </tr>

  <tr>

   <td width="48">3</td>

   <td width="90"> 3</td>

   <td width="105"> 3/6 = 1/2</td>

  </tr>

  <tr>

   <td width="48">4</td>

   <td width="90"> 2</td>

   <td width="105">2/6 = 1/3</td>

  </tr>

  <tr>

   <td width="48">5</td>

   <td width="90"> 3</td>

   <td width="105"> 3/6 = 1/2</td>

  </tr>

  <tr>

   <td width="48">6</td>

   <td width="90"> 2</td>

   <td width="105"> 2/6  = 1/3</td>

  </tr>

  <tr>

   <td width="48">7</td>

   <td width="90"> 2</td>

   <td width="105"> 2/6 = 1/3</td>

  </tr>

 </tbody>

</table>




<strong>Closeness centrality:</strong> You need to calculate the inverted score after you count the total number of steps to a node.  In order to know the standardized score, you need to divide a score by (n-1), then take inverse.  Note that the most central node is node 4 while the most central node for degree centrality is node 3 and 5.

<table width="243">

 <tbody>

  <tr>

   <td width="42">Node</td>

   <td width="112">Score</td>

   <td width="88">StandardizedScore</td>

  </tr>

  <tr>

   <td width="42">1</td>

   <td width="112"> 1/16</td>

   <td width="88"> 6/16 = 3/8</td>

  </tr>

  <tr>

   <td width="42">2</td>

   <td width="112"> 1/16</td>

   <td width="88"> 6/16 = 3/8</td>

  </tr>

  <tr>

   <td width="42">3</td>

   <td width="112"> 1/11</td>

   <td width="88">6/11</td>

  </tr>

  <tr>

   <td width="42">4</td>

   <td width="112"> 1/10</td>

   <td width="88"> 6/10 = 3/5</td>

  </tr>

  <tr>

   <td width="42">5</td>

   <td width="112"> 1/11</td>

   <td width="88">6/11</td>

  </tr>

  <tr>

   <td width="42">6</td>

   <td width="112"> 1/15</td>

   <td width="88"> 6/15 = 2/5</td>

  </tr>

  <tr>

   <td width="42">7</td>

   <td width="112"> 1/15</td>

   <td width="88"> 6/15 = 2/5</td>

  </tr>

 </tbody>

</table>




<strong>Betweenness centrality:</strong> To calculate betweenness centrality, you take every pair of the network and count how many times a node can interrupt the shortest paths (geodesic distance) between the two nodes of the pair. For standardization, I note that the denominator is (n-1)(n-2)/2. For this network, (7-1)(7-2)/2 = 15.  Note that node 5 has a little smaller centrality score that node 3 and 4 because the connection between node 6 and 7 reduces the controllability of node 5.

<strong>Betwennes Centrality: </strong>

Where,         is the betwenness centarlity of node V,   is the number of shortest paths between all source and target pairs,  is the number of shortests paths between all source and target pairs those pass through from node V.

<table width="299">

 <tbody>

  <tr>

   <td width="55">Source</td>

   <td width="53">Target</td>

   <td width="122">Intermedia Nodes</td>

   <td width="70">Path</td>

  </tr>

  <tr>

   <td width="55">1</td>

   <td width="53">2</td>

   <td width="122">3</td>

   <td width="70">1-3-2</td>

  </tr>

  <tr>

   <td width="55">1</td>

   <td width="53">3</td>

   <td width="122">–</td>

   <td width="70">1-3</td>

  </tr>

  <tr>

   <td width="55">1</td>

   <td width="53">4</td>

   <td width="122">3</td>

   <td width="70">1-3-4</td>

  </tr>

  <tr>

   <td width="55">1</td>

   <td width="53">5</td>

   <td width="122">3,4</td>

   <td width="70">1-3-4-5</td>

  </tr>

  <tr>

   <td width="55">1</td>

   <td width="53">6</td>

   <td width="122">3,4,5</td>

   <td width="70">1-3-4-5-6</td>

  </tr>

  <tr>

   <td width="55">1</td>

   <td width="53">7</td>

   <td width="122">3,4,5</td>

   <td width="70">1-3-4-5-7</td>

  </tr>

  <tr>

   <td width="55">2</td>

   <td width="53">3</td>

   <td width="122">–</td>

   <td width="70">2-3</td>

  </tr>

  <tr>

   <td width="55">2</td>

   <td width="53">4</td>

   <td width="122">3</td>

   <td width="70">2-3-4</td>

  </tr>

  <tr>

   <td width="55">2</td>

   <td width="53">5</td>

   <td width="122">3,4</td>

   <td width="70">2-3-4-5</td>

  </tr>

  <tr>

   <td width="55">2</td>

   <td width="53">6</td>

   <td width="122">3,4,5</td>

   <td width="70">2-3-4-5-6</td>

  </tr>

  <tr>

   <td width="55">2</td>

   <td width="53">7</td>

   <td width="122">3,4,5</td>

   <td width="70">2-3-4-5-7</td>

  </tr>

  <tr>

   <td width="55">3</td>

   <td width="53">4</td>

   <td width="122">–</td>

   <td width="70">3-4</td>

  </tr>

  <tr>

   <td width="55">3</td>

   <td width="53">5</td>

   <td width="122">4</td>

   <td width="70">3-4-5</td>

  </tr>

  <tr>

   <td width="55">3</td>

   <td width="53">6</td>

   <td width="122">4,5</td>

   <td width="70">3-4-5-6</td>

  </tr>

  <tr>

   <td width="55">3</td>

   <td width="53">7</td>

   <td width="122">4,5</td>

   <td width="70">3-4-5-7</td>

  </tr>

  <tr>

   <td width="55">4</td>

   <td width="53">5</td>

   <td width="122">–</td>

   <td width="70">4-5</td>

  </tr>

  <tr>

   <td width="55">4</td>

   <td width="53">6</td>

   <td width="122">5</td>

   <td width="70">4-5-6</td>

  </tr>

  <tr>

   <td width="55">4</td>

   <td width="53">7</td>

   <td width="122">5</td>

   <td width="70">5-6-7</td>

  </tr>

  <tr>

   <td width="55">5</td>

   <td width="53">6</td>

   <td width="122">–</td>

   <td width="70">5-6</td>

  </tr>

  <tr>

   <td width="55">5</td>

   <td width="53">7</td>

   <td width="122">–</td>

   <td width="70">5-7</td>

  </tr>

  <tr>

   <td width="55">6</td>

   <td width="53">7</td>

   <td width="122">–</td>

   <td width="70">5-7</td>

  </tr>

 </tbody>

</table>










After making standardization (n-1)(n-2)/2=15







c)(15 points) What do you think about the information flow on this graph? What do you think the most powerful/critical node of this graph?,nk that this is a centralized graph? Why, why not?Do you think that