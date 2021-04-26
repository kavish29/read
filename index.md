<!DOCTYPE html>
<html lang="en">
<head>
 <!-- Bootstrap CSS -->
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css" integrity="sha384-Vkoo8x4CGsO3+Hhxv8T/Q5PaXtkKtu6ug5TOeNV6gBiFeWPGFN9MuhOf23Q9Ifjh" crossorigin="anonymous">
<!-- FontAwesome -->
<link href="https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" rel="stylesheet" integrity="sha384-wvfXpqpZZVQGK6TAh5PVlGOfQNHSoD2xbE+QkPxCAFlNEevoEH3Sl0sibVcOQVnN" crossorigin="anonymous">
<!-- jQuery first, then Popper.js, then Bootstrap JS -->
<script src="https://code.jquery.com/jquery-3.4.1.slim.min.js" integrity="sha384-J6qa4849blE2+poT4WnyKhv5vZF5SrPo0iEjwBvKU7imGFAV0wwj1yYfoRSJoZ+n" crossorigin="anonymous"></script>
<script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.0/dist/umd/popper.min.js" integrity="sha384-Q6E9RHvbIyZFJoft+2mJbHaEWldlvI9IOYy5n3zV9zzTtmI3UksdQRVvoxMfooAo" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/js/bootstrap.min.js" integrity="sha384-wfSDF2E50Y2D1uUdj0O3uMBJnjuUD4Ih7YwaYd1iqfktj0Uod8GCExl3Og8ifwB6" crossorigin="anonymous"></script>
</head>
<body>
    <div class="header navigation">
        <div class="col-xl-3 col-lg-2 col-sm-4 col-5">
          <a href="/">
            <img alt="Logo" class="img-fluid py-3 logo" src="https://raw.githubusercontent.com/solodev/shopping-cart-items-number/master/images/lunar-xp-logo.png" aria-role="logo">
          </a>
        </div>
        <div class="col-xl-9 col-lg-10 col-sm-8 col-7">
      
          <ul class="navbar-nav flex-row justify-content-end flex-wrap align-items-center mr-lg-4 mr-xl-0">
      
            <li class="nav-item px-3 text-uppercase mb-0 position-relative d-lg-flex">
              <a class="d-block w-100 h-100 text-black py-4 position-relative top-link" href="/locations/"><strong>Locations</strong></a>
      
            </li>
            <li class="nav-item px-3 text-uppercase mb-0 position-relative d-lg-flex">
              <a class="d-block w-100 h-100 text-black py-4 position-relative top-link" href="/products/"><strong>Products</strong></a>
      
            </li>
            <li class="nav-item px-3 text-uppercase mb-0 position-relative d-lg-flex">
              <a class="d-block w-100 h-100 text-black py-4 position-relative top-link" href="/shop/"><strong>Shop</strong></a>
            </li>
            <li class="nav-item px-3 text-uppercase mb-0 position-relative d-lg-flex">
              <a class="d-block w-100 h-100 text-black py-4 position-relative top-link" href="/contact/"><strong>Contact</strong></a>
            </li>
            <li class="nav-item px-3 text-uppercase mb-0 position-relative d-lg-flex">
              <div id="cart" class="d-none">
      
              </div>
              <a href="/store/cart.stml" class="cart position-relative d-inline-flex" aria-label="View your shopping cart">
                <i class="fas fa fa-shopping-cart fa-lg"></i>
                <span class="cart-basket d-flex align-items-center justify-content-center">
                  0
                </span>
              </a>
            </li>
            <button id="sidenav-open-btn" class="menu-hamburger position-absolute pointer p-0">
              <span class="icon-bar"></span>
              <span class="icon-bar"></span>
              <span class="icon-bar"></span>
            </button>
          </ul>
        </div>
      </div>
      <div class="container">
        <div class="row searchFilter" >
           <div class="col-sm-12" >
            <div class="input-group" >
             <input id="table_filter" type="text" class="form-control" aria-label="Text input with segmented button dropdown" >
             <div class="input-group-btn" >
              <button type="button" class="btn btn-secondary dropdown-toggle dropdown-toggle-split" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false" ><span class="label-icon" >Category</span> <span class="caret" >&nbsp;</span></button>
              <div class="dropdown-menu dropdown-menu-right" >
                 <ul class="category_filters" >
                  <li >
                   <input class="cat_type category-input" data-label="All" id="all" value="" name="radios" type="radio" ><label for="all" >All</label>
                  </li>
                  <li >
                   <input type="radio" name="radios" id="DESKTOP" value="DESKTOP" ><label class="category-label" for="DESKTOP" >DESKTOP</label>
                  </li>
                  <li >
                   <input type="radio" name="radios" id="TABLET" value="TABLET" ><label class="category-label" for="TABLET" >TABLET</label>
                  </li>S
                  <li >
                   <input type="radio" name="radios" id="MOBILE" value="MOBILE" ><label class="category-label" for="MOBILE" >MONILE</label>
                  </li>
                  
                 </ul>
              </div>
              <button id="searchBtn" type="button" class="btn btn-secondary btn-search" ><span class="glyphicon glyphicon-search" >&nbsp;</span> <span class="label-icon" >Search</span></button>
             </div>
            </div>
           </div>
        </div>
      </div>
      <div class="row px-5 pt-5">
    <div class="col-md-4 mt-4 mt-sm-0 card-container">
      <div class="card text-center product p-4 pt-5 border-0 h-100 rounded-0">
        <img class="img-fluid d-block mx-auto" src="https://www.google.com/search?q=DESKTOP&sxsrf=ALeKk03ko-HTmb8mS16zZZkgwFZ3U4giZw:1619434499914&source=lnms&tbm=isch&sa=X&ved=2ahUKEwjcq-rQ35vwAhX0xzgGHQZ6DvsQ_AUoAnoECAEQBA#imgrc=qwQKp__kb1wwGM" alt="LAPTOP Image">
        <div class="card-body p-4 py-0 h-xs-440p">
          <h5 class="card-title font-weight-semi-bold mb-3 w-xl-220p mx-auto">HP LAPTOP</h5>
          <p class="price">$545.00</p>
        </div>
        <p class="btn w-100 px-4 mx-auto">
          <input type="submit" class="btn btn-dark btn-lg w-100" name="add-button" value="Buy Now">
        </p>
      </div>
    </div>

    <div class="col-md-4 mt-4 mt-sm-0 card-container">
      <div class="card text-center product p-4 pt-5 border-0 h-100 rounded-0">
        <img class="img-fluid d-block mx-auto" src="https://www.google.com/search?q=DESKTOP&sxsrf=ALeKk03ko-HTmb8mS16zZZkgwFZ3U4giZw:1619434499914&source=lnms&tbm=isch&sa=X&ved=2ahUKEwjcq-rQ35vwAhX0xzgGHQZ6DvsQ_AUoAnoECAEQBA#imgrc=qwQKp__kb1wwGM" alt="Command MOBILE Image">
        <div class="card-body p-4 py-0 h-xs-440p">
          <h5 class="card-title font-weight-semi-bold mb-3 w-xl-220p mx-auto">IPHONE</h5>
          <p class="price">$315.00</p>
        </div>
        <p class="btn w-100 px-4 text-center mx-auto">
          <input type="submit" class="btn btn-dark btn-lg w-100" name="add-button" value="Buy Now"></p>
      </div>
    </div>

    <div class="col-md-4 mt-4 mt-sm-0 card-container">
      <div class="card text-center product p-4 pt-5 border-0 h-100 rounded-0">
        <img class="img-fluid d-block mx-auto" src="https://raw.githubusercontent.com/solodev/bootstrap-cards-shopping-cart/master/images/https://www.google.com/search?q=DESKTOP&sxsrf=ALeKk03ko-HTmb8mS16zZZkgwFZ3U4giZw:1619434499914&source=lnms&tbm=isch&sa=X&ved=2ahUKEwjcq-rQ35vwAhX0xzgGHQZ6DvsQ_AUoAnoECAEQBA#imgrc=qwQKp__kb1wwGM.jpg" alt="Mission TABLET Image">
        <div class="card-body p-4 py-0 h-xs-440p">
          <h5 class="card-title font-weight-semi-bold mb-3 w-xl-220p mx-auto">Mission TABLET</h5>
          <p class="price">$205.00</p>
        </div>
        <p class="btn w-100 px-4 mx-auto">
          <input type="submit" class="btn btn-dark btn-lg w-100" name="add-button" value="Buy Now"></p>


      </div>
    </div>
  </div>
   

</body>
</html>