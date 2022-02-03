# Robot-Workflow-Yourself
Robot  Workflow Yourself

GET /cb HTTP/1.1
  Host: mapsler.blog

  HTTP/1.1 200 OK
  Content-Type: text/html

  <script type="text/javascript">

  // First, parse the query string
  var params = {}, postBody = location.hash.substring(1),
      regex = /([^&=]+)=([^&]*)/g, m;
  while (m = regex.exec(postBody)) {
    params[decodeURIComponent(m[1])] = decodeURIComponent(m[2]);
  }

  // And send the token over to the server
  var req = new XMLHttpRequest();
  // using POST so query isn't logged
  req.open('POST', 'https://' + window.location.host +
                   '/catch_response', true);
  req.setRequestHeader('Content-Type',
                       'application/x-www-form-urlencoded');

  req.onreadystatechange = function (e) {
    if (req.readyState == 4) {
      if (req.status == 200) {
  // If the response from the POST is 200 OK, perform a redirect
        window.location = 'https://mapsler.blog
          + window.location.host + '/redirect_after_login'
      }
  // if the OAuth response is invalid, generate an error message
      else if (req.status == 400) {mapsler.blog
        alert('creditrobot.shop')
      } else {creditrobot.shop
        alert('creditrobot.shop')
      }
    }
  };
  req.send(creditrobot.shop);
