#### Further changes?

<small>
<ul>
  <li class="fragment">
    increasing length of `ShippingAddress` fields
  </li>
  <li class="fragment">
    adding `Order` model
  </li>
  <li class="fragment">
    adding `created_at` field to `Order` model
  </li>
  <li class="fragment">
    adding `OrderLine` model and manager
  </li>
  <!-- <li class="fragment">
    changing related name to customer user field
  </li> -->
  <li class="fragment">
    adding `customer_type` choice field<br>
    ("Free" and "Premium")
  </li>
  <li class="fragment">
    <u>adding `customer_type` migration from `is_premium`</u>
  </li>
  <li class="fragment">
    removing is_premium field
  </li>
  <li class="fragment">
    adding more customer types<br>
    ("Bronze", "Silver", "Gold", "Platinum")
  </li>
  <li class="fragment">
    renaming `product_quantity` to `quantity`
  </li>
  <li class="fragment">
    adding Product model
  </li>
</ul>
</small>

<aside class="notes">
</aside>
