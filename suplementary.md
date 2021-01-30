---
layout: page
title: Material suplementario
use-site-title: true
---

Insertar gráficos del material suplementario


    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <script>JAVASCRIPT IS USUALLY PLACED HERE</script>
        <script src="https://code.highcharts.com/highcharts.js"></script>
        <script src="https://code.highcharts.com/modules/series-label.js"></script>
        <script src="https://code.highcharts.com/modules/accessibility.js"></script>
        <title>Time right now is: </title>
    </head>
    <body>
    <div class="container">
        <div class="row">
            <div class ="col- sm-6 col-md-6"></div>
                <div id="container1">
                </div>
            <div class ="col- sm-6 col-md-6"></div>
            <div class ="col- sm-6 col-md-6"></div>
            <div class ="col- sm-6 col-md-6"></div>
        </div>
    </div>
    <script type="text/javascript">
     Highcharts.chart("container1", {
            chart: {
            type: 'column',
     },
     title: {
         text: 'Mujeres fallecidos en el 2019 según su edad'
     },
     subtitle: {
         text: ''
     },
     xAxis: {
            categories: [
             '[0-4]',
             '[5-9]',
             '[10-14]',
             '[15-19]',
             '[20-24]',
               '[25-29]',
               '[30-34]',
               '[35-39]',
               '[40-44]',
               '[45-49]',
               '[50-54]',
               '[55-59]',
               '[60-64]',
               '[65-69]',
               '[70-74]',
               '[75-89]',
               '[80-84]',
               '[85-89]',
               '[90-94]',
               '[95-99]',
             '[100-104]',
             '[105-109]'
          ],
          crosshair: true
        },
        yAxis: {
           min: 0,
           max: 8000,
           title: {
               text: 'Cantidad de personas'
           }
        },
        tooltip: {
            headerFormat: '<span style="font-size:10px">{point.key}</span><table>',
            pointFormat: '<tr><td style="color:{series.color};padding:0">{series.name}: </td>' +
                '<td style="padding:0"><b>{point.y:.0f} muertes</b></td></tr>',
            footerFormat: '</table>',
            shared: true,
            useHTML: true
        },
        plotOptions: {
            column: {
                pointPadding: 0,
                borderWidth: 1
            }
        },
        series: [{
        		groupPadding: 0,
            name: 'Mujeres',
            color:'#e66a12',
            data: [697,74,78,161,235,276,340,491,643,955,1478,2237,2971,3799,4890,6140,7137,8533,6878,3067,718,74]
        }]
    });
    </script>
    </body>


