#### 🛒🛍 Add `shop` app

<small>
<ul>
  <li>
    `Customer` model and shipping details
  </li>
  <li class="fragment">
    adding `is_premium` field to `Customer` model
  </li>
  <li class="fragment">
    creating dedicated `ShippingAddress` model
  </li>
  <li class="fragment">
    <u>migrating data to new shipping addresses</u>
  </li>
  <li class="fragment">
    removing Customer shipping fields<br>
    (one migration per field: state, province, city, zip code, address, name)
  </li>
</ul>
</small>


<aside class="notes">
</aside>
