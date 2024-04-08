## `Components` associated with the `User` Micro-frontend views

<table>
  
<tr>
    <th>Micro-frontend</th>
    <th>Views</th>
    <th>Components</th>
    <th>ViewModels</th>
  </tr>
  <tr>
    <td rowspan="20" style="vertical-align: top;">User</td>
    <td rowspan="3">
      <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/views/View3.png?raw=true" style="width: 150px; height: auto;" />
    </td>
    <td style="vertical-align: top;">
      Header<br>
      <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/USER1.png?raw=true" style="width: 150px; height: auto;" />
    </td>
    <td style="vertical-align: top;">props.title<br>props.text<br>props.image</td>
  </tr>
  <tr>
    <td style="vertical-align: top;">
      Login<br>
      <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/USERLOGIN.png?raw=true" style="width: 150px; height: auto;" />
    </td>
    <td style="vertical-align: top;">props.email<br>props.password<br>props.logInStatus
    <ul>
  <li>1 = waiting</li>
  <li>2 = requested</li>
  <li>3 = accepted</li>
  <li>4 = denied</li>
</ul>
    </td>
  </tr>
  <tr>
    <td style="vertical-align: top;">
      Footer<br>
      <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/USERFOOTER.png?raw=true" style="width: 150px; height: auto;" />
    </td>
    <td style="vertical-align: top;">props.forgotPasswordLink<br>props.createAccountLink</td>
  </tr>
  <tr>
    <td rowspan="6">
      <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/views/View1.png?raw=true" style="width: 150px; height: auto;" />
    </td>
    <td style="vertical-align: top;">
      Header<br>
      <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/USER3.png?raw=true" style="width: 150px; height: auto;" />
    </td>
    <td style="vertical-align: top;">props.navigateBack<br>props.title<br>props.image</td>
  </tr>
  <tr>
    <td style="vertical-align: top;">
      User Avatar<br>
      <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/USER4.png?raw=true" style="width: 150px; height: auto;" />
    </td>
    <td style="vertical-align: top;">props.uploadAvatarImage<br>props.uploadImageStatus
      <ul>
      <li>1 = uploading</li>
      <li>2 = upload success</li>
      <li>3 = upload error</li>
    </ul>
      props.avatarImage</td>
  </tr>
  <tr>
    <td style="vertical-align: top;">
      User Details<br>
      <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/USER5.png?raw=true" style="width: 150px; height: auto;" />
    </td>
    <td style="vertical-align: top;">props.userName<br>props.userEmail</td>
  </tr>
  <tr>
    <td style="vertical-align: top;">
      User Profile<br>
      <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/USER6.png?raw=true" style="width: 150px; height: auto;" />
    </td>
    <td style="vertical-align: top;">props.myAccountButton<br>props.settingsButton<br>prop.contactButton</td>
  </tr>
  <tr>
    <td style="vertical-align: top;">
      Log Out<br>
      <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/USER7.png?raw=true" style="width: 150px; height: auto;" />
    </td>
    <td style="vertical-align: top;">props.logOutButton<br>props.logOutButtonStatus 
      <ul>
      <li>1 = logging out</li>
      <li>2 = logged out</li>
      <li>3 = error</li>
    </ul></td>
  </tr>
  <tr>
    <td style="vertical-align: top;">
      Footer/Menu<br>
      <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/FOOTER.png?raw=true" style="width: 150px; height: auto;" />
    </td>
    <td style="vertical-align: top;">props.navigateHomepage<br>props.navigateSavedProducts<br>props.navigateQrCodeScanner<br>props.navigateNews<br>props.navigateUserProfile</td>
  </tr>
    <tr>
    <td rowspan="2">
      <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/views/View12.png?raw=true" style="width: 150px; height: auto;" />
        </td>
    <td style="vertical-align: top;">Header<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/USER9.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.navigateBack</td>
  </tr>
      <td style="vertical-align: top;">Saved Product Pop-up<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/USER10.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.text<br>props.okButton</td>
  </tr>
 

  <tr>
    <td rowspan="3">
      <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/views/View13.png?raw=true" style="width: 150px; height: auto;" />
        </td>
    <td style="vertical-align: top;">Header<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/Product1.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.navigateBack<br>props.title</td>
  </tr>
  <tr>
    <td style="vertical-align: top;">Saved Products<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/USER12.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.title<br>props.savedProducs<br>props.selectProduct<br>props.text</td>
  </tr>

  <tr>
    <td style="vertical-align: top;">Footer/Menu<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/FOOTER.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.navigateHomepage<br>props.navigateSavedProducts<br>props.navigateQrCodeScanner<br>props.navigateNews<br>props.navigateUserProfile</td>
  </tr>
       <tr>
    <td rowspan="5">
      <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/views/View10.png?raw=true" style="width: 150px; height: auto;" />
        </td>
    <td style="vertical-align: top;">Header<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/Product1.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.navigateBack<br>props.title</td>
  </tr>
  <tr>
    <td style="vertical-align: top;">Product Image<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/Product2.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.productImage</td>
  </tr>
  <tr>
    <td style="vertical-align: top;">Product Details<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/Product3.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.title<br>props.price<br>props.selectedLocation<br>props.details<br>props.expandDetailsButton</td>
  </tr>
  <tr>
    <td style="vertical-align: top;">User Feedback<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/Product4.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.title<br>props.seeFeedbackButton</td>
  </tr>
  <tr>
    <td style="vertical-align: top;">Footer/Menu<br>
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/components/images/Product5.png?raw=true" style="width: 150px; height: auto;" /></td>
    <td style="vertical-align: top;">props.navigateHomepage<br>props.navigateSavedProducts<br>props.navigateQrCodeScanner<br>props.navigateNews<br>props.navigateUserProfile</td>
  </tr>
</table>
