## `Components` associated with the `QR Code` Micro-frontend views

<table>
  <tr>
    <th>Micro-frontend</th>
    <th>Views</th>
    <th>Components</th>
    <th>ViewModels</th>
  </tr>
  <tr>
    <td rowspan="4" style="vertical-align: center;">QRCode</td>
    <td rowspan="4">
      <img src="https://github.com/DuarteVDG/aw-project/blob/main/views/View11.png?raw=true" style="width: 150px; height: auto;" />
    </td>
    <td style="vertical-align: top;">Header<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/components/images/QRCode1.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.title<br>props.navigateBack</td>
  </tr>
  <tr>
    <td style="vertical-align: top;">QR Scan<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/components/images/QRCode2.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.qrScan<br>props.status<br>  <ul>
    <li>1 = scanning</li>
    <li>2 = scanned</li>
    <li>3 = processing</li>
    <li>4 = error</li>
  </ul> </td>
  </tr>
  <tr>
    <td style="vertical-align: top;">Scanned Product Details<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/components/images/QRCode3.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.viewProductDetails</td>
  </tr>
  <tr>
    <td style="vertical-align: top;">Footer/Menu<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/components/images/QRCode4.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.navigateHomepage<br>props.navigateSavedProducts<br>props.navigateQrCodeScanner<br>props.navigateNews<br>props.navigateUserProfile</td>
  </tr>
</table>
