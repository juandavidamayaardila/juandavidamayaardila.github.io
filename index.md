HOLAA Mundo Juan Amaya

Mi nombre es Juan David Amaya, soy ingeniero de sistemas de la universidad del Quindío

### Mis hobbies son

Mis pasatiempos son:


1. Football
2. Musica
3. Percusion 
4. Natacion



### Contacto

Tel: 3113559485
Juandavidamayaardila@gmail.com
Armenia Quindío



<html>
  <head>
    <!--Load the AJAX API-->
    <script type="text/javascript" src="https://www.gstatic.com/charts/loader.js"></script>
    <script type="text/javascript">

      // Load the Visualization API and the corechart package.
      google.charts.load('current', {'packages':['corechart']});

      // Set a callback to run when the Google Visualization API is loaded.
      google.charts.setOnLoadCallback(drawChart);

      // Callback that creates and populates a data table,
      // instantiates the pie chart, passes in the data and
      // draws it.
      function drawChart() {

        // Create the data table.
        var data = new google.visualization.DataTable();
        data.addColumn('string', 'Topping');
        data.addColumn('number', 'Slices');
        data.addRows([
          ['IE6', 15],
          ['IE7', 20],
          ['IE8', 65],
       
        ]);

        // Set chart options
        var options = {'title':'How Much Pizza I Ate Last Night',
                       'width':400,
                       'height':300};

        // Instantiate and draw our chart, passing in some options.
        var chart = new google.visualization.PieChart(document.getElementById('chart_div'));
        chart.draw(data, options);
      }
      
      
      //cambio de datos
      function cambioValores() {

        // Create the data table.
        var data = new google.visualization.DataTable();
        data.addColumn('string', 'Topping');
        data.addColumn('number', 'Slices');
        data.addRows([
          ['IE6', 30],
          ['IE7', 25],
          ['IE8', 45],
       
        ]);

        // Set chart options
        var options = {'title':'How Much Pizza I Ate Last Night',
                       'width':400,
                       'height':300};

        // Instantiate and draw our chart, passing in some options.
        var chart = new google.visualization.PieChart(document.getElementById('chart_div'));
        chart.draw(data, options);
      }
      
    </script>
  </head>

  <body>
    <!--Div that will hold the pie chart-->
    <div id="chart_div"></div>
  <input type="button" value="Inicializar" onclick="drawChart()"/>
  <input type="button" value="Cambio Valores" onclick="cambioValores()"/>
  </body>
</html>


