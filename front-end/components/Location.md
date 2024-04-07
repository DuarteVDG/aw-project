## `Components` associated with the `Location` Micro-frontend views

<table>
  <tr>
    <th>Micro-frontend</th>
    <th>Views</th>
    <th>Components</th>
    <th>ViewModels</th>
  </tr>
  <tr>
    <td rowspan="13" style="vertical-align: top;">Location</td>
    <td rowspan="4">
      <img src="https://github.com/DuarteVDG/aw-project/blob/main/views/View8.png?raw=true" style="width: 150px; height: auto;" />
    </td>
    <td style="vertical-align: top;">Header<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/components/images/Location1.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.title<br>props.image</td>
  </tr>
  </td>
    <td style="vertical-align: top;">Supermarket List<br>
   <img src="https://github.com/DuarteVDG/aw-project/blob/main/components/images/Location2.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.dropDownList<br>props.selectionStatus<br>  <ul>
    <li>1 = waiting</li>
    <li>2 = requested</li>
    <li>3 = accepted</li>
    <li>4 = denied</li>
  </ul>props.locationSelection

  
  props.goSelectionButton</td>
  </tr>
   </td>
    <td style="vertical-align: top;">Highlighted Products<br>
   <img src="https://github.com/DuarteVDG/aw-project/blob/main/components/images/Location3.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.gridLayout<br>props.text<br>props.image<br>props.selectProductButton</td>
  </tr>
  </td>
    <td style="vertical-align: top;">Footer/Menu<br>
  <img src="https://github.com/DuarteVDG/aw-project/blob/main/components/images/Location4.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.navigateHomepage<br>props.navigateSavedProducts<br>props.navigateQrCodeScanner<br>props.navigateNews<br>props.navigateUserProfile</td>
  </tr>
    <tr>
    <td rowspan="4">
      <img src="https://github.com/DuarteVDG/aw-project/blob/main/views/View7.png?raw=true" style="width: 150px; height: auto;" />
    </td>
    <td style="vertical-align: top;">Header<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/components/images/Location5.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.title<br>props.navigateBack</td>
  </tr>
  <tr>
    <td style="vertical-align: top;">Google Maps API Window<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/components/images/Location6.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.mapStatus
    <ul>
      <li>1 = loading</li>
    <li>2 = ready</li>
    <li>3 = error</li>
    <li>4 = interacting</li>
    </ul>
props.zoomIn<br>props.zoomOut<br>props.move</td>
  </tr>
  <tr>
    <td style="vertical-align: top;">Product Categories<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/components/images/Location7.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.gridLayout<br>props.text<br>props.image<br>props.selectProductButton</td>
  </tr>
  <tr>
    <td style="vertical-align: top;">Footer/Menu<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/components/images/Location8.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.navigateHomepage<br>props.navigateSavedProducts<br>props.navigateQrCodeScanner<br>props.navigateNews<br>props.navigateUserProfile</td>
  </tr>
    <tr>
    <td rowspan="5">
      <img src="https://github.com/DuarteVDG/aw-project/blob/main/views/View16.png?raw=true" style="width: 150px; height: auto;" />
        </td>
    <td style="vertical-align: top;">Header<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/components/images/Location9.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.title<br>props.navigateBack</td>
  </tr>
  <tr>
    <td style="vertical-align: top;">Selected Information<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/components/images/Location10.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.supermarketLocation<br>props.productCategory</td>
  </tr>
  <tr>
    <td style="vertical-align: top;">Highlighted Product<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/components/images/Location11.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.title<br>props.selectHighlightedProduct<br>props.navigateHighlights</td>
  </tr>
  <tr>
    <td style="vertical-align: top;">All Products<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/components/images/Location12.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.title<br>props.scroll<br>props.scrollStatus
      <ul>
    <li>1 = scrolling</li>
    <li>2 = idle</li>
    <li>3 = reached top/bottom</li>
  </ul>
      props.selectProduct</td>
  </tr>
  <tr>
    <td style="vertical-align: top;">Footer/Menu<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/components/images/Location13.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.navigateHomepage<br>props.navigateSavedProducts<br>props.navigateQrCodeScanner<br>props.navigateNews<br>props.navigateUserProfile</td>
  </tr>
</table>
