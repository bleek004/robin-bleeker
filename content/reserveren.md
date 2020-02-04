+++
img_path = ""
layout = "page"
subtitle = ""
title = "Reserveren"
[menu.main]
weight = 8

+++
<!DOCTYPE html>

<html>

  <head>

    <meta charset="utf-8">

    <meta http-equiv="X-UA-Compatible" content="IE=edge">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title></title>

    <link rel="stylesheet" href="assets/style.css">

    <link rel="stylesheet" href="assets/dateTimePicker.css">

  </head>

  <body>

    <div class="container">

      <h2>Tulia</h2>

      <div class="row">

        <div class="col-xss-12">

          <div id="show-next-month1" data-toggle="calendar"></div>

        </div>

        

      </div>

      

  </div>

    <div class="container">

      <h2>Tent 1</h2>

      <div class="row">

        <div class="col-xss-12">

          <div id="show-next-month2" data-toggle="calendar"></div>

        </div>

        

      </div>

      

  </div>

    <div class="container">

      <h2>Tent 2</h2>

      <div class="row">

        <div class="col-xss-12">

          <div id="show-next-month3" data-toggle="calendar"></div>

        </div>

        

      </div>

      

  </div>

  

    <script type="text/javascript" src="scripts/components/jquery.min.js"></script>

    <script type="text/javascript" src="scripts/dateTimePicker.min.js"></script>

    <script type="text/javascript">

    $(document).ready(function()

    {

      $('#show-next-month1').calendar(

      {

        num_next_month: 1,

        num_prev_month: 1,

        unavailable: \['*-*-9', '*-*-10'\],

		onSelectDate: function(date, month, year){

          alert(\[year, month, date\].join('-') + ' is: ' + this.isAvailable(date, month, year));}

      });

    });

	$(document).ready(function()

    {

      $('#show-next-month2').calendar(

      {

        num_next_month: 1,

        num_prev_month: 1,

        unavailable: \['*-*-9', '*-*-10'\]

      });

    });

	$(document).ready(function()

    {

      $('#show-next-month3').calendar(

      {

        num_next_month: 1,

        num_prev_month: 1,

        unavailable: \['*-*-9', '*-*-10'\]

      });

    });

    </script>

  </body>

</html>