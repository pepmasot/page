<html> 
<head>
      <title></title>
</head>
<body>
<h1><strong>Descarga de Datos Bicing</strong></h1>

<p>Los datos sobre el servicio de sharing de bicicletas, bicing, est&aacute;n disponibles en la web del Ajuntament de Barcelona,&nbsp;<a href="https://opendata-ajuntament.barcelona.cat/resources/bcn/BicingBCN">https://opendata-ajuntament.barcelona.cat/resources/bcn/BicingBCN</a>&nbsp;.&nbsp;Los datos estan agrupados por meses y comprimidos con el formato <span style="color:#3498db">{year}_{month:02d}_{month_name}_BicingNou_ESTACIONS.7z</span>&nbsp; y se recopilan desde marzo de 2019. Para este proyecto, descargamos todos los datos del periodo marzo 2019 . diciembre 2022, que seran los datos que usaremos para el entrenamiento, los guardamos en formato csv, tambi&eacute;n por meses para su posterior procesamiento.</p>

<p>Cada uno de los ficheros contiene la siguiente informaci&oacute;n y tipo de dato:</p>

<table border="0" cellpadding="1" cellspacing="1" style="width:786px">
      <thead>
            <tr>
                  <th scope="col" style="width:239px"><strong>Variable</strong></th>
                  <th scope="col" style="width:61px"><strong>Tipo</strong></th>
                  <th scope="col" style="width:355px"><strong>Descripci&oacute;n</strong></th>
                  <th scope="col" style="width:59px"><strong>Min</strong></th>
                  <th scope="col" style="width:74px"><strong>Max</strong></th>
            </tr>
      </thead>
      <tbody>
            <tr>
                  <td style="width:239px"><strong>station_id</strong></td>
                  <td style="width:61px">int64</td>
                  <td style="width:355px">Identificador de la estaci&oacute;n</td>
                  <td style="width:59px">1</td>
                  <td style="width:74px">532</td>
            </tr>
            <tr>
                  <td style="width:239px"><strong>num_bikes_available</strong></td>
                  <td style="width:61px">int64</td>
                  <td style="width:355px">autoexplicativa</td>
                  <td style="width:59px">0</td>
                  <td style="width:74px">54</td>
            </tr>
            <tr>
                  <td style="width:239px"><strong>num_bikes_available_types.mechanical</strong></td>
                  <td style="width:61px">int64</td>
                  <td style="width:355px">autoexplicativa</td>
                  <td style="width:59px">0</td>
                  <td style="width:74px">54</td>
            </tr>
            <tr>
                  <td style="width:239px"><strong>num_bikes_available_types.ebike</strong></td>
                  <td style="width:61px">int64</td>
                  <td style="width:355px">autoexplicativa</td>
                  <td style="width:59px">0</td>
                  <td style="width:74px">41</td>
            </tr>
            <tr>
                  <td style="width:239px"><strong>num_docks_available</strong></td>
                  <td style="width:61px">int64</td>
                  <td style="width:355px">autoexplicativa</td>
                  <td style="width:59px">0</td>
                  <td style="width:74px">54</td>
            </tr>
            <tr>
                  <td style="width:239px"><strong>last_reported</strong></td>
                  <td style="width:61px">int64</td>
                  <td style="width:355px">Tiempo en segundos de cuanto se tomo el registro</td>
                  <td style="width:59px">&nbsp;</td>
                  <td style="width:74px">&nbsp;</td>
            </tr>
            <tr>
                  <td style="width:239px"><strong>is_charging_station</strong></td>
                  <td style="width:61px">bool</td>
                  <td style="width:355px">Si la estaci&oacute;n permite cargar bicis el&eacute;ctricas</td>
                  <td style="width:59px">&nbsp;</td>
                  <td style="width:74px">&nbsp;</td>
            </tr>
            <tr>
                  <td style="width:239px"><strong>status</strong></td>
                  <td style="width:61px">object</td>
                  <td style="width:355px">
                  <pre>
IN_SERVICE       
MAINTENANCE      
PLANNED
NOT_IN_SERVICE 
END_OF_LIFE
</pre>
                  </td>
                  <td style="width:59px">&nbsp;</td>
                  <td style="width:74px">&nbsp;</td>
            </tr>
            <tr>
                  <td style="width:239px"><strong>is_installed</strong></td>
                  <td style="width:61px">int64</td>
                  <td style="width:355px">Si la estaci&oacute;n est&aacute; instalada</td>
                  <td style="width:59px">0</td>
                  <td style="width:74px">1</td>
            </tr>
            <tr>
                  <td style="width:239px"><strong>is_renting</strong></td>
                  <td style="width:61px">int64</td>
                  <td style="width:355px">Si la estaci&oacute;n permite la entrega(desbloquo) de bicicletas</td>
                  <td style="width:59px">0</td>
                  <td style="width:74px">1</td>
            </tr>
            <tr>
                  <td style="width:239px"><strong>is_returning</strong></td>
                  <td style="width:61px">int64</td>
                  <td style="width:355px">Si la estaci&oacute;n permite la devoluci&oacute;n de bicicletas</td>
                  <td style="width:59px">0</td>
                  <td style="width:74px">1</td>
            </tr>
            <tr>
                  <td style="width:239px"><strong>last_updated</strong></td>
                  <td style="width:61px">int64</td>
                  <td style="width:355px">Tiempo en segundos de la &uacute;ltima actualizaci&oacute;n&nbsp;</td>
                  <td style="width:59px">&nbsp;</td>
                  <td style="width:74px">&nbsp;</td>
            </tr>
            <tr>
                  <td style="width:239px">
                  <p><strong>traffic (a partir de finales de 2021)</strong></p>
                  </td>
                  <td style="width:61px">float64</td>
                  <td style="width:355px">Desconocemos su significado, pero en la mayoria de casos o no est&aacute; disponible o contiene NAN</td>
                  <td style="width:59px">&nbsp;</td>
                  <td style="width:74px">&nbsp;</td>
            </tr>
            <tr>
                  <td style="width:239px"><strong>ttl</strong></td>
                  <td style="width:61px">int64</td>
                  <td style="width:355px">Variable descartable para este proyecto</td>
                  <td style="width:59px">&nbsp;</td>
                  <td style="width:74px">
                  <p>&nbsp;</p>
                  </td>
            </tr>
      </tbody>
</table>

<p>Debido al gran tama&ntilde;o de los ficheros, en un primer paso concatenamos los ficheros mensuales&nbsp;agrupando&nbsp;la informaci&oacute;n por a&ntilde;os, salvando cada a&ntilde;o en un fichero csv, y procedermos a analizar los datos a&ntilde;o por a&ntilde;o para ver qu&eacute; tipo de datos tenemos&nbsp;y hacer un primer procesado&nbsp;descartando&nbsp;aquellas variables que consideremos innecesarias para este proyecto o transformando algunas de ellas.</p>

<p>Hacemos las siguientes observaciones:</p>

<ul>
      <li>La variable <strong>last_reported</strong> no tiene registro en algunos casos. La descartaremos</li>
      <li>Nos quedamos con la variable <strong>last_udpated</strong>&nbsp;para saber en qu&eacute; momento se tomaron los datos, cambiaremos el formato a la fecha y hora correspondiente a&nbsp;nuestra zona horaria&nbsp;(timezone&nbsp;Europe/Madrid) creando&nbsp;las nuevas variables: <strong>year, month, day, hour, min</strong></li>
      <li>Las variables <strong>ttl</strong>&nbsp;y&nbsp;<strong>traffic</strong> tambi&eacute;n las descartaremos. Est&aacute; &uacute;ltima variable no est&aacute; recogida durante los primeros a&ntilde;os, se incorpora a finalesl de 2021, pero en la mayoria de casos contine NAN</li>
      <li>Interpretamos los posibles valores de la variable status de la siguiente manera:
      <ul>
            <li>IN_SERVICE: estaci&oacute;n en pleno funcionamiento</li>
            <li>NOT_IN_SERVICE: estaci&oacute;n temporalmente fuera de servicio. Puede ser por unas horas debido a alg&uacute;n evento o por varios dias debido a obras en la zona</li>
            <li>MAINTENANCE: la estaci&oacute;n est&aacute; siendo asistida por el servicio de bicing, a&ntilde;adiendo o sustrayendo las bicicletas disponible en esa estaci&oacute;n. Ese proceso dura unos minutos</li>
            <li>PLANNED: estaci&oacute;n planificada pero todavia no est&aacute; en servicio.&nbsp;</li>
            <li>END_OF_LIFE: estaci&oacute;n suprimida</li>
      </ul>
      </li>
</ul>

<p style="margin-left:40px">Tambi&eacute;n observamos que el&nbsp;n&uacute;mero de [&nbsp;NOT_IN_SERVICE + MAINTENANCE + PLANNED] &nbsp;equivale al n&uacute;mero de &nbsp;[<strong>is_returning</strong>==0] ; y que&nbsp;el n&uacute;mero de [PLANNED] equivale al n&uacute;mero [<strong>is_installed</strong>==0].&nbsp;</p>

<p style="margin-left:40px">Tambi&eacute;n vemos que cuando las estaciones tienen un estado distinto a IN_SERVICE los datos &nbsp;sobre <strong>num_bikes_available</strong>, <strong>num_bikes_available_types.ebike</strong>, <strong>num_bikes_available_types.mechanical</strong> y <strong>num_docks_available</strong> tienen inconsistencias. En la mayoria de casos num_bikes_available est&aacute; a cero cuando el detalle bicicletas el&eacute;ctricas y mec&aacute;nicas dice lo contrario; y tambi&eacute;n hay varios casos con num_bike_available y num_docks_available ambos a cero. Adem&aacute;s en esos casos no es posible devolver bicicletas como acabamos de comentar arriba, por lo que a efectos pr&aacute;cticos no hay docks disopnibles para el usuario.. Por todo ello procederemos a eliminar los records en los que <strong>status</strong> != IN_SERVICE</p>

<p>El formato de los ficheros .csv que guardamos con las informaci&oacute;n anual sobre el bicing contendr&aacute; esta informaci&oacute;n:</p>

<table border="1" cellpadding="1" cellspacing="1" style="width:998px">
      <thead>
            <tr>
                  <th scope="col" style="width:72px">station_id</th>
                  <th scope="col" style="width:147px">num_bikes_available</th>
                  <th scope="col" style="width:241px"><strong>num_bikes_available_types.mechanical</strong></th>
                  <th scope="col" style="width:212px"><strong>num_bikes_available_types.ebike</strong></th>
                  <th scope="col" style="width:147px">num_docks_available</th>
                  <th scope="col" style="width:33px">year</th>
                  <th scope="col" style="width:32px">month</th>
                  <th scope="col" style="width:40px">day</th>
                  <th scope="col" style="width:42px">hour</th>
                  <th scope="col" style="width:41px">min</th>
            </tr>
      </thead>
      <tbody>
      </tbody>
</table>

<p>Estos ficheros ser&aacute;n los que usaremos para analizar con m&aacute;s detalle qu&eacute; ocurri&oacute; en 2020 y c&oacute;mo funciona el bicing en la actualidad,&nbsp;2022 mostrarndo gr&aacute;ficas y mapas&nbsp;coloreads din&aacute;micamente.</p>

<p>Una de las principales observaciones que hacemos al haber revisado todos los a&ntilde;os, es la diferencia de registros, los a&ntilde;os 2019 y 2020 tiene menos frecuencia de registros, y en particular el a&ntilde;o 20</p>

<p><a href="https://lh3.googleusercontent.com/drive-viewer/AFGJ81qjiGJAZn7t0H1lfFmtk6SCI_znPHYlGOTnARjawU7ks2mGKx244rsRPXiFUrWcpswGYf3hyeSAoPJSbCl254JlZ7OP=s2560?source=screenshot.guru"><img src="https://lh3.googleusercontent.com/drive-viewer/AFGJ81qjiGJAZn7t0H1lfFmtk6SCI_znPHYlGOTnARjawU7ks2mGKx244rsRPXiFUrWcpswGYf3hyeSAoPJSbCl254JlZ7OP=s2560" /> </a></p>

<h2>Descarga megadatos de las estaciones&nbsp;</h2>

<p>Antes de seguir con el</p>

<pre>

&nbsp;</pre>
</body>
</html>
