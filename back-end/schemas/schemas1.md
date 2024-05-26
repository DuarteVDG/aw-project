<table>
  <tr>
    <th>BE Services</th>
    <th>Requests</th>
    <th>Responses</th>
  </tr>
  <tr>
    <td rowspan="4">AuthenticationService</td>
    <td>GET /auth/status<br>
        <strong>Type:</strong> object<br>
        <strong>Properties:</strong><br>
        - status: string (Authentication status)
    </td>
    <td>
        <strong>200:</strong><br>
        <strong>Description:</strong> Current authentication status.<br>
        <strong>Content:</strong> application/json<br>
        <strong>Schema:</strong> { status: string }
    </td>
  </tr>
  <tr>
      <td>POST /auth/login<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong><br>
          - username: string (Username)<br>
          - password: string (Password)
      </td>
      <td>
          <strong>201:</strong><br>
          <strong>Description:</strong> User authenticated successfully.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> { token: string }
      </td>
  </tr>
  <tr>
      <td>PUT /auth/update<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong><br>
          - username: string (Username)<br>
          - oldPassword: string (Old Password)<br>
          - newPassword: string (New Password)
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> User credentials updated.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> { status: string }
      </td>
  </tr>
  <tr>
      <td>DELETE /auth/logout<br>
          <strong>Type:</strong> None
      </td>
      <td>
          <strong>204:</strong><br>
          <strong>Description:</strong> User logged out.<br>
          <strong>Content:</strong> None
      </td>
  </tr>

  <tr>
      <td rowspan="5">ProductInfoService</td>
      <td>GET /products<br>
          <strong>Type:</strong> None
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> List of all products.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> array<br>
          <strong>Items:</strong> { productId: integer, name: string, price: decimal, description: string }
      </td>
  </tr>
  <tr>
      <td>GET /products/{id}<br>
          <strong>Type:</strong> path parameter<br>
          <strong>Properties:</strong> { id: integer }
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> Details of the specified product.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> { productId: integer, name: string, price: decimal, description: string }
      </td>
  </tr>
  <tr>
      <td>POST /products<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong> { name: string, price: decimal, description: string }
      </td>
      <td>
          <strong>201:</strong><br>
          <strong>Description:</strong> Product created successfully.<br>
          <strong>Content:</strong> application/json
      </td>
  </tr>
  <tr>
      <td>PUT /products/{id}<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong> { name: string, price: decimal, description: string }
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> Product information updated.<br>
          <strong>Content:</strong> application/json
      </td>
  </tr>
  <tr>
      <td>DELETE /products/{id}<br>
          <strong>Type:</strong> path parameter<br>
          <strong>Properties:</strong> { id: integer }
      </td>
      <td>
          <strong>204:</strong><br>
          <strong>Description:</strong> Product information deleted.<br>
          <strong>Content:</strong> None
      </td>
  </tr>

  <tr>
      <td rowspan="2">StoreLocatorService</td>
      <td>GET /stores<br>
          <strong>Type:</strong> None
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> List of all stores.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> array<br>
          <strong>Items:</strong> { storeId: integer, name: string, location: string }
      </td>
  </tr>
  <tr>
      <td>GET /stores/{id}<br>
          <strong>Type:</strong> path parameter<br>
          <strong>Properties:</strong> { id: integer }
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> Details of the specified store.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> { storeId: integer, name: string, location: string }
      </td>
  </tr>

  <tr>
      <td rowspan="2">InventoryService</td>
      <td>GET /inventory<br>
          <strong>Type:</strong> None
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> Product availability in stores.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> array<br>
          <strong>Items:</strong> { productId: integer, storeId: integer, availability: boolean }
      </td>
  </tr>
  <tr>
      <td>GET /inventory/{id}<br>
          <strong>Type:</strong> path parameter<br>
          <strong>Properties:</strong> { id: integer }
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> Availability of the specified product.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> { productId: integer, storeId: integer, availability: boolean }
      </td>
  </tr>

  <tr>
      <td rowspan="4">FeedbackService</td>
      <td>GET /feedback<br>
          <strong>Type:</strong> None
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> List of all feedback.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> array<br>
          <strong>Items:</strong> { feedbackId: integer, userId: integer, productId: integer, rating: integer, comment: string }
      </td>
  </tr>
  <tr>
      <td>GET /feedback/{id}<br>
          <strong>Type:</strong> path parameter<br>
          <strong>Properties:</strong> { id: integer }
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> Details of the specified feedback.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> { feedbackId: integer, userId: integer, productId: integer, rating: integer, comment: string }
      </td>
  </tr>
  <tr>
      <td>POST /feedback<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong> { userId: integer, productId: integer, rating: integer, comment: string }
      </td>
      <td>
          <strong>201:</strong><br>
          <strong>Description:</strong> Feedback submitted successfully.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> { feedbackId: integer, userId: integer, productId: integer, rating: integer, comment: string }
      </td>
  </tr>
  <tr>
      <td>DELETE /feedback/{id}<br>
          <strong>Type:</strong> path parameter<br>
          <strong>Properties:</strong> { id: integer }
      </td>
      <td>
          <strong>204:</strong><br>
          <strong>Description:</strong> Feedback removed.<br>
          <strong>Content:</strong> None
      </td>
  </tr>

  <tr>
    <td rowspan="5">UserProfileService</td>
    <td>GET /profiles<br>
        <strong>Type:</strong> None
    </td>
    <td>
        <strong>200:</strong><br>
        <strong>Description:</strong> List of all user profiles.<br>
        <strong>Content:</strong> application/json<br>
        <strong>Schema:</strong> array<br>
        <strong>Items:</strong> { userId: integer, name: string, email: string, age: integer }
    </td>
  </tr>
  <tr>
      <td>GET /profiles/{id}<br>
          <strong>Type:</strong> path parameter<br>
          <strong>Properties:</strong> { id: integer }
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> Details of the specified user profile.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> { userId: integer, name: string, email: string, age: integer }
      </td>
  </tr>
  <tr>
      <td>POST /profiles<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong> { name: string, email: string, age: integer }
      </td>
      <td>
          <strong>201:</strong><br>
          <strong>Description:</strong> User profile created successfully.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> { userId: integer, name: string, email: string, age: integer }
      </td>
  </tr>
  <tr>
      <td>PUT /profiles/{id}<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong> { name: string, email: string, age: integer }
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> User profile updated.<br>
          <strong>Content:</strong> application/json
      </td>
  </tr>
  <tr>
      <td>DELETE /profiles/{id}<br>
          <strong>Type:</strong> path parameter<br>
          <strong>Properties:</strong> { id: integer }
      </td>
      <td>
          <strong>204:</strong><br>
          <strong>Description:</strong> User profile removed.<br>
          <strong>Content:</strong> None
      </td>
  </tr>

  <tr>
    <td rowspan="1">QRCodeService</td>
    <td>POST /qrcode/decode<br>
        <strong>Type:</strong> object<br>
        <strong>Properties:</strong> { qrcode: string }
    </td>
    <td>
        <strong>200:</strong><br>
        <strong>Description:</strong> QR code decoded successfully.<br>
        <strong>Content:</strong> application/json<br>
        <strong>Schema:</strong> { productId: integer, name: string, price: decimal, description: string }
    </td>
  </tr>

  <tr>
    <td rowspan="6">NewsService</td>
    <td>GET /news<br>
        <strong>Type:</strong> None
    </td>
    <td>
        <strong>200:</strong><br>
        <strong>Description:</strong> List of all news articles.<br>
        <strong>Content:</strong> application/json<br>
        <strong>Schema:</strong> array<br>
        <strong>Items:</strong> { newsId: integer, title: string, content: string, date: string }
    </td>
  </tr>
  <tr>
      <td>GET /news/{id}<br>
          <strong>Type:</strong> path parameter<br>
          <strong>Properties:</strong> { id: integer }
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> Details of the specified news article.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> { newsId: integer, title: string, content: string, date: string }
      </td>
  </tr>
  <tr>
      <td>POST /news<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong> { title: string, content: string, date: string }
      </td>
      <td>
          <strong>201:</strong><br>
          <strong>Description:</strong> News article created successfully.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> { newsId: integer, title: string, content: string, date: string }
      </td>
  </tr>
  <tr>
      <td>PUT /news/{id}<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong> { title: string, content: string, date: string }
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> News article updated.<br>
          <strong>Content:</strong> application/json
      </td>
  </tr>
  <tr>
      <td>DELETE /news/{id}<br>
          <strong>Type:</strong> path parameter<br>
          <strong>Properties:</strong> { id: integer }
      </td>
      <td>
          <strong>204:</strong><br>
          <strong>Description:</strong> News article removed.<br>
          <strong>Content:</strong> None
      </td>
  </tr>
  <tr>
      <td>PUT /news/{id}/archive<br>
          <strong>Type:</strong> path parameter<br>
          <strong>Properties:</strong> { id: integer }
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> News article archived.<br>
          <strong>Content:</strong> application/json
      </td>
  </tr>

  <tr>
    <td rowspan="2">AnalyticsService</td>
    <td>GET /analytics<br>
        <strong>Type:</strong> None
    </td>
    <td>
        <strong>200:</strong><br>
        <strong>Description:</strong> Statistical data and analysis.<br>
        <strong>Content:</strong> application/json<br>
        <strong>Schema:</strong> array<br>
        <strong>Items:</strong> { analyticsId: integer, metric: string, value: number }
    </td>
  </tr>
  <tr>
      <td>GET /analytics/{id}<br>
          <strong>Type:</strong> path parameter<br>
          <strong>Properties:</strong> { id: integer }
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> Details of the specified statistical data.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> { analyticsId: integer, metric: string, value: number }
      </td>
  </tr>

  <tr>
    <td rowspan="3">FavoritesService</td>
    <td>GET /favorites<br>
        <strong>Type:</strong> None
    </td>
    <td>
        <strong>200:</strong><br>
        <strong>Description:</strong> List of user's favorite products.<br>
        <strong>Content:</strong> application/json<br>
        <strong>Schema:</strong> array<br>
        <strong>Items:</strong> { favoriteId: integer, productId: integer, userId: integer }
    </td>
  </tr>
  <tr>
      <td>POST /favorites<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong> { productId: integer, userId: integer }
      </td>
      <td>
          <strong>201:</strong><br>
          <strong>Description:</strong> Product added to favorites.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> { favoriteId: integer, productId: integer, userId: integer }
      </td>
  </tr>
  <tr>
      <td>DELETE /favorites/{id}<br>
          <strong>Type:</strong> path parameter<br>
          <strong>Properties:</strong> { id: integer }
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> Favorite product removed.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> { success: boolean }
      </td>
  </tr>

  <tr>
    <td rowspan="5">StoreManagementService</td>
    <td>GET /stores<br>
        <strong>Type:</strong> None
    </td>
    <td>
        <strong>200:</strong><br>
        <strong>Description:</strong> List of all stores.<br>
        <strong>Content:</strong> application/json<br>
        <strong>Schema:</strong> array<br>
        <strong>Items:</strong> { storeId: integer, name: string, location: string }
    </td>
  </tr>
  <tr>
      <td>GET /stores/{id}<br>
          <strong>Type:</strong> path parameter<br>
          <strong>Properties:</strong> { id: integer }
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> Details of the specified store.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> { storeId: integer, name: string, location: string }
      </td>
  </tr>
  <tr>
      <td>POST /stores<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong> { name: string, location: string }
      </td>
      <td>
          <strong>201:</strong><br>
          <strong>Description:</strong> Store created successfully.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> { storeId: integer, name: string, location: string }
      </td>
  </tr>
  <tr>
      <td>PUT /stores/{id}<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong> { name: string, location: string }
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> Store information updated.<br>
          <strong>Content:</strong> application/json
      </td>
  </tr>
  <tr>
      <td>DELETE /stores/{id}<br>
          <strong>Type:</strong> path parameter<br>
          <strong>Properties:</strong> { id: integer }
      </td>
      <td>
          <strong>204:</strong><br>
          <strong>Description:</strong> Store information deleted.<br>
          <strong>Content:</strong> None
      </td>
  </tr>
  <tr>
    <td rowspan="5">PricingService</td>
    <td>GET /prices<br>
        <strong>Type:</strong> None
    </td>
    <td>
        <strong>200:</strong><br>
        <strong>Description:</strong> List of product prices.<br>
        <strong>Content:</strong> application/json<br>
        <strong>Schema:</strong> array<br>
        <strong>Items:</strong> { priceId: integer, productId: integer, price: decimal }
    </td>
  </tr>
  <tr>
      <td>GET /prices/{id}<br>
          <strong>Type:</strong> path parameter<br>
          <strong>Properties:</strong> { id: integer }
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> Details of the specified product price.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> { priceId: integer, productId: integer, price: decimal }
      </td>
  </tr>
  <tr>
      <td>POST /prices<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong> { productId: integer, price: decimal }
      </td>
      <td>
          <strong>201:</strong><br>
          <strong>Description:</strong> Product price added successfully.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> { priceId: integer, productId: integer, price: decimal }
      </td>
  </tr>
  <tr>
      <td>PUT /prices/{id}<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong> { price: decimal }
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> Product price updated.<br>
          <strong>Content:</strong> application/json
      </td>
  </tr>
  <tr>
      <td>DELETE /prices/{id}<br>
          <strong>Type:</strong> path parameter<br>
          <strong>Properties:</strong> { id: integer }
      </td>
      <td>
          <strong>204:</strong><br>
          <strong>Description:</strong> Product price removed.<br>
          <strong>Content:</strong> None
      </td>
  </tr>

  <tr>
    <td rowspan="4">ReviewService</td>
    <td>GET /reviews<br>
        <strong>Type:</strong> None
    </td>
    <td>
        <strong>200:</strong><br>
        <strong>Description:</strong> List of customer reviews.<br>
        <strong>Content:</strong> application/json<br>
        <strong>Schema:</strong> array<br>
        <strong>Items:</strong> { reviewId: integer, productId: integer, userId: integer, rating: integer, comment: string }
    </td>
  </tr>
  <tr>
      <td>GET /reviews/{id}<br>
          <strong>Type:</strong> path parameter<br>
          <strong>Properties:</strong> { id: integer }
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> Details of the specified review.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> { reviewId: integer, productId: integer, userId: integer, rating: integer, comment: string }
      </td>
  </tr>
  <tr>
      <td>POST /reviews<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong> { productId: integer, userId: integer, rating: integer, comment: string }
      </td>
      <td>
          <strong>201:</strong><br>
          <strong>Description:</strong> New review added successfully.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> { reviewId: integer, productId: integer, userId: integer, rating: integer, comment: string }
      </td>
  </tr>
  <tr>
      <td>DELETE /reviews/{id}<br>
          <strong>Type:</strong> path parameter<br>
          <strong>Properties:</strong> { id: integer }
      </td>
      <td>
          <strong>204:</strong><br>
          <strong>Description:</strong> Review deleted.<br>
          <strong>Content:</strong> None
      </td>
  </tr>

  <tr>
    <td rowspan="2">AppConfigService</td>
    <td>GET /config<br>
        <strong>Type:</strong> None
    </td>
    <td>
        <strong>200:</strong><br>
        <strong>Description:</strong> Application configurations.<br>
        <strong>Content:</strong> application/json<br>
        <strong>Schema:</strong> { configId: integer, key: string, value: string }
    </td>
  </tr>
  <tr>
      <td>PUT /config<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong> { key: string, value: string }
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> Application configurations updated.<br>
          <strong>Content:</strong> application/json
      </td>
  </tr>
</table>
