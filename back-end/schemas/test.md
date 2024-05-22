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
      <td>DELETE /auth/logout</td>
      <td></td>
  </tr>
  
  <tr>
      <td rowspan="5">ProductInfoService</td>
      <td>GET /products<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong><br>
          - productId: integer (Unique product identifier)<br>
          - name: string (Product name)<br>
          - price: decimal (Product price)<br>
          - description: string (Product description)
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> List of all products.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> array<br>
          <strong>Items:</strong> $ref: '#/components/schemas/Product'
      </td>
  </tr>
  <tr>
      <td>GET /products/{id}<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong><br>
          - productId: integer (Unique product identifier)<br>
          - name: string (Product name)<br>
          - price: decimal (Product price)<br>
          - description: string (Product description)
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> Details of the specified product.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> $ref: '#/components/schemas/Product'
      </td>
  </tr>
  <tr>
      <td>POST /products<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong><br>
          - name: string (Product name)<br>
          - price: decimal (Product price)<br>
          - description: string (Product description)
      </td>
      <td>
          <strong>201:</strong><br>
          <strong>Description:</strong> Product created successfully.<br>
          <strong>Content:</strong> application/json
      </td>
  </tr>
  <tr>
      <td>PUT /products/{id}</td>
      <td></td>
  </tr>
  <tr>
      <td>DELETE /products/{id}</td>
      <td></td>
  </tr>
  
  <tr>
      <td rowspan="2">StoreLocatorService</td>
      <td>GET /stores<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong><br>
          - storeId: integer (Unique store identifier)<br>
          - name: string (Store name)<br>
          - location: string (Store location)
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> List of all stores.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> array<br>
          <strong>Items:</strong> $ref: '#/components/schemas/Store'
      </td>
  </tr>
  <tr>
      <td>GET /stores/{id}<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong><br>
          - storeId: integer (Unique store identifier)<br>
          - name: string (Store name)<br>
          - location: string (Store location)
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> Details of the specified store.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> $ref: '#/components/schemas/Store'
      </td>
  </tr>
  
  <tr>
      <td rowspan="2">InventoryService</td>
      <td>GET /inventory<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong><br>
          - productId: integer (Unique product identifier)<br>
          - storeId: integer (Unique store identifier)<br>
          - availability: boolean (Product availability)
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> Product availability.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> array<br>
          <strong>Items:</strong> $ref: '#/components/schemas/Inventory'
      </td>
  </tr>
  <tr>
      <td>GET /inventory/{id}<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong><br>
          - productId: integer (Unique product identifier)<br>
          - storeId: integer (Unique store identifier)<br>
          - availability: boolean (Product availability)
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> Availability of the specified product.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> $ref: '#/components/schemas/Inventory'
      </td>
  </tr>
  
  <tr>
      <td rowspan="4">FeedbackService</td>
      <td>GET /feedback<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong><br>
          - feedbackId: integer (Unique feedback identifier)<br>
          - userId: integer (Unique user identifier)<br>
          - productId: integer (Unique product identifier)<br>
          - rating: integer (Product rating)<br>
          - comment: string (User comment)
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> List of all feedback.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> array<br>
          <strong>Items:</strong> $ref: '#/components/schemas/Feedback'
      </td>
  </tr>
  <tr>
      <td>GET /feedback/{id}<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong><br>
          - feedbackId: integer (Unique feedback identifier)<br>
          - userId: integer (Unique user identifier)<br>
          - productId: integer (Unique product identifier)<br>
          - rating: integer (Product rating)<br>
          - comment: string (User comment)
      </td>
      <td>
          <strong>200:</strong><br>
          <strong>Description:</strong> Details of the specified feedback.<br>
          <strong>Content:</strong> application/json<br>
          <strong>Schema:</strong> $ref: '#/components/schemas/Feedback'
      </td>
  </tr>
  <tr>
      <td>POST /feedback<br>
          <strong>Type:</strong> object<br>
          <strong>Properties:</strong><br>
          - userId: integer (Unique user identifier)<br>
          - productId: integer (Unique product identifier)<br>
          - rating: integer (Product rating)<br>
          - comment: string (User comment)
      </td>
      <td>
          <strong>201:</strong><br>
          <strong>Description:</strong> Feedback submitted successfully.<br>
          <strong>Content:</strong> application/json
      </td>
  </tr>
  <tr>
      <td>DELETE /feedback/{id}</td>
      <td></td>
  </tr>
</table>
