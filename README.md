# task
<!doctype html>
<html lang="en">

<head>
  <title>Section Estimator</title>
  <!-- Font Awesome -->
  <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.7.0/css/all.css">
  <!-- Bootstrap core CSS -->
  <link href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.2.1/css/bootstrap.min.css" rel="stylesheet">
  <!-- Material Design Bootstrap -->
  <link href="https://cdnjs.cloudflare.com/ajax/libs/mdbootstrap/4.7.3/css/mdb.min.css" rel="stylesheet">

</head>

<body>
  <main class="container-fluid">

    <h1>Given number of students and number of sections, display average number of students per section</h1>
    

    <p>Enter your name:
      <input id="guest" type="text" value="Eden">
    </p>

    <p>Enter students:
      <input id="students" type="number" value="30">
    </p>

    <p>Enter sections:
      <input id="sections" type="number" value="5">
    </p>

    <button id="clicker" class="btn btn-primary">Click me!</button>

    <p id="result"></p>

  </main>

  <script>
    console.log('SCRIPT START')
    console.log('Declare testable functions.....................')
    function div(students,sections) {
      return students/sections;
    }
    console.log('Defined division=' + div)
    console.log('Declare event listeners .......................')
    document.getElementById('clicker').addEventListener('click', function () {
      const s = document.getElementById('guest').value
      const i = parseInt(document.getElementById('students').value)
      console.log('i=' + i)
      const j = parseInt(document.getElementById('sections').value)
      console.log('j=' + j)
      const ans = s + ', your product is ' + div(i, j) + '.'
      document.getElementById('result').innerHTML = ans
    })
    console.log('SCRIPT END')
  </script>

  <!-- JQuery -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
  <!-- Bootstrap tooltips -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.4/umd/popper.min.js"></script>
  <!-- Bootstrap core JavaScript -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.2.1/js/bootstrap.min.js"></script>
  <!-- MDB core JavaScript -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/mdbootstrap/4.7.3/js/mdb.min.js"></script>
</body>

</html>
