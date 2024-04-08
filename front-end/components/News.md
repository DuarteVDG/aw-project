## `Components` associated with the `News` Micro-frontend views

<table>
  <tr>
    <th>Micro-frontend</th>
    <th>Views</th>
    <th>Components</th>
    <th>ViewModels</th>
  </tr>
  <tr>
    <td rowspan="4" style="vertical-align: top;">Menu</td>
    <td rowspan="4">
      <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/views/View4.png?raw=true" style="width: 150px; height: auto;" />
    </td>
    <td style="vertical-align: top;">Header<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/News1.png?raw=true" style="width: 150px; height: auto;" />
    </td>
    <td style="vertical-align: top;">props.title<br>props.navigateBack<br>props.navigateToStatistics</td>
  </tr>
  <tr>
    <td style="vertical-align: top;">Highlighted News<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/News2.png?raw=true" style="width: 150px; height: auto;" />
    </td>
    <td style="vertical-align: top;">props.image<br>props.title<br>props.readMore</td>
  </tr>
  <tr>
    <td style="vertical-align: top;">Latest News<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/News3.png?raw=true" style="width: 150px; height: auto;" />
    </td>
    <td style="vertical-align: top;">props.date<br>props.origin<br>props.newsList<br>props.scrollList<br>props.scrollStatus
      <ul>
    <li>1 = scrolling</li>
    <li>2 = idle</li>
    <li>3 = reached top/bottom</li>
  </ul>
      props.selectNews</td>
  </tr>
  <tr>
    <td style="vertical-align: top;">Footer/Menu<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/News4.png?raw=true" style="width: 150px; height: auto;" />
    </td>
    <td style="vertical-align: top;">props.navigateHomepage<br>props.navigateSavedProducts<br>props.navigateQrCodeScanner<br>props.navigateNews<br>props.navigateUserProfile</td>
  </tr>
  
  <tr>
    <td rowspan="3" style="vertical-align: top;">News</td>
    <td rowspan="3">
      <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/views/View6.png?raw=true" style="width: 150px; height: auto;" />
    </td>
    <td style="vertical-align: top;">Header<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/News5.png?raw=true" style="width: 150px; height: auto;" />
    </td>
    <td style="vertical-align: top;">props.title<br>props.navigateBack</td>
  </tr>
  <tr>
    <td style="vertical-align: top;">Article<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/News6.png?raw=true" style="width: 150px; height: auto;" />
    </td>
    <td style="vertical-align: top;">props.image<br>props.title<br>props.text<br>props.scrollArticle<br>props.scrollStatus
      <ul>
    <li>1 = scrolling</li>
    <li>2 = idle</li>
    <li>3 = reached top/bottom</li>
  </ul></td>
  </tr>
  <tr>
    <td style="vertical-align: top;">Footer/Menu<br>
   <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/News7.png?raw=true" style="width: 150px; height: auto;" />
    </td>
    <td style="vertical-align: top;">props.navigateHomepage<br>props.navigateSavedProducts<br>props.navigateQrCodeScanner<br>props.navigateNews<br>props.navigateUserProfile</td>
  </tr>
  </tr>
</table>
