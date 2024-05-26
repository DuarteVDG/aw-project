<table>
  <tr>
    <th>BE Services</th>
    <th>Requests</th>
    <th>Resources</th>
    <th>Description</th>
  </tr>
  <tr>
    <td rowspan="4">Authentication</td>
    <td>GET</td>
    <td>/auth/status</td>
    <td>Retrieve user authentication status.</td>
  </tr>
  <tr>
    <td>POST</td>
    <td>/auth/login</td>
    <td>Authenticate user and create session.</td>
  </tr>
  <tr>
    <td>PUT</td>
    <td>/auth/update</td>
    <td>Update user credentials.</td>
  </tr>
  <tr>
    <td>DELETE</td>
    <td>/auth/logout</td>
    <td>Remove user session.</td>
  </tr>
  <tr>
    <td rowspan="5">ProductInfo</td>
    <td>GET</td>
    <td>/products</td>
    <td>Retrieve a list of all products.</td>
  </tr>
  <tr>
    <td>GET</td>
    <td>/products/{id}</td>
    <td>Retrieve specific product by ID.</td>
  </tr>
  <tr>
    <td>POST</td>
    <td>/products</td>
    <td>Add new product information.</td>
  </tr>
  <tr>
    <td>PUT</td>
    <td>/products/{id}</td>
    <td>Update existing product information.</td>
  </tr>
  <tr>
    <td>DELETE</td>
    <td>/products/{id}</td>
    <td>Remove product information.</td>
  </tr>
    <td rowspan="2">Inventory</td>
    <td>GET</td>
    <td>/inventory</td>
    <td>Retrieve product availability in stores.</td>
  </tr>
  <tr>
    <td>GET</td>
    <td>/inventory/{id}</td>
    <td>Retrieve availability of specific product by ID.</td>
  </tr>
  <tr>
    <td rowspan="4">Feedback</td>
    <td>GET</td>
    <td>/feedback</td>
    <td>Retrieve a list of all feedback.</td>
  </tr>
  <tr>
    <td>GET</td>
    <td>/feedback/{id}</td>
    <td>Retrieve specific feedback by ID.</td>
  </tr>
  <tr>
    <td>POST</td>
    <td>/feedback</td>
    <td>Submit new feedback.</td>
  </tr>
  <tr>
    <td>DELETE</td>
    <td>/feedback/{id}</td>
    <td>Remove feedback.</td>
  </tr>
  <tr>
    <td rowspan="5">UserProfile</td>
    <td>GET</td>
    <td>/profiles</td>
    <td>Retrieve a list of all user profiles.</td>
  </tr>
  <tr>
    <td>GET</td>
    <td>/profiles/{id}</td>
    <td>Retrieve specific user profile by ID.</td>
  </tr>
  <tr>
    <td>POST</td>
    <td>/profiles</td>
    <td>Create new user profile.</td>
  </tr>
  <tr>
    <td>PUT</td>
    <td>/profiles/{id}</td>
    <td>Update existing user profile.</td>
  </tr>
  <tr>
    <td>DELETE</td>
    <td>/profiles/{id}</td>
    <td>Remove user profile.</td>
  </tr>
  <tr>
    <td>QRCodeService</td>
    <td>POST</td>
    <td>/qrcode/decode</td>
    <td>Decode QR code and retrieve product information.</td>
  </tr>
  <tr>
    <td rowspan="7">News</td>
    <td>GET</td>
    <td>/news</td>
    <td>Retrieve a list of all news articles.</td>
  </tr>
  <tr>
    <td>GET</td>
    <td>/news/{id}</td>
    <td>Retrieve specific news article by ID.</td>
  </tr>
  <tr>
    <td>POST</td>
    <td>/news</td>
    <td>Create a new news article.</td>
  </tr>
  <tr>
    <td>PUT</td>
    <td>/news/{id}</td>
    <td>Update existing news article.</td>
  </tr>
  <tr>
    <td>DELETE</td>
    <td>/news/{id}</td>
    <td>Delete specific news article.</td>
  </tr>
  <tr>
    <td>PUT</td>
    <td>/news/{id}/archive</td>
    <td>Archive specific news article.</td>
  </tr>
  <tr>
    <td>GET</td>
    <td>/news/</td>
    <td>Retrieve a list of all news articles.</td>
  </tr>
  <tr>
    <td rowspan="2">Analytics</td>
    <td>GET</td>
    <td>/analytics</td>
    <td>Retrieve statistical data and analysis.</td>
  </tr>
  <tr>
    <td>GET</td>
    <td>/analytics/{id}</td>
    <td>Retrieve specific statistical data by ID.</td>
  </tr>
  <tr>
    <td rowspan="3">Favorites</td>
    <td>GET</td>
    <td>/favorites</td>
    <td>Retrieve a list of user's favorite products.</td>
  </tr>
  <tr>
    <td>POST</td>
    <td>/favorites</td>
    <td>Add product to favorites.</td>
  </tr>
  <tr>
    <td>DELETE</td>
    <td>/favorites/{id}</td>
    <td>Remove product from favorites.</td>
  </tr>
  <tr>
    <td rowspan="5">StoreManagement</td>
    <td>GET</td>
    <td>/stores</td>
    <td>Retrieve a list of all stores.</td>
  </tr>
  <tr>
    <td>GET</td>
    <td>/stores/{id}</td>
    <td>Retrieve specific store by ID.</td>
  </tr>
  <tr>
    <td>POST</td>
    <td>/stores</td>
    <td>Add new store.</td>
  </tr>
  <tr>
    <td>PUT</td>
    <td>/stores/{id}</td>
    <td>Update existing store.</td>
  </tr>
  <tr>
    <td>DELETE</td>
    <td>/stores/{id}</td>
    <td>Remove store.</td>
  </tr>
  <tr>
    <td rowspan="2">AppConfig</td>
    <td>GET</td>
    <td>/config</td>
    <td>Retrieve application configurations.</td>
  </tr>
  <tr>
    <td>PUT</td>
    <td>/config</td>
    <td>Update application configurations.</td>
  </tr>
</table>
