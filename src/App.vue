<template>
  <div id="app">
    <header id="header-03" class="header">
    <!-- START NAVBAR -->
      <nav class="navbar navbar-expand-md navbar-light bg-faded">
        <div class="container">
            <a class="navbar-brand" href="index.html"><img src="images/logo.png" alt="SafeTour"></a>
            <ul class="navbar-nav ml-auto">
                <li class="nav-item dropdown"><a href="index.html" class="nav-link active">Home</a>
                    <ul class="dropdown-menu">
                      <li><a class="dropdown-item" href="index.html">Home Version 1</a></li>
                      <li><a class="dropdown-item" href="index-02.html">Home Version 2</a></li>
                      <li><a class="dropdown-item" href="index-03.html">Home Version 3</a></li>
                      <li><a class="dropdown-item" href="index-04.html">Home Version 4</a></li>                            
                      <li><a class="dropdown-item" href="index-05.html">Home Version 5</a></li>
                    </ul>
                </li>
                <li class="nav-item dropdown"><a href="packages-grid.html" class="nav-link">Tours</a>
                    <ul class="dropdown-menu">
                      <li><a class="dropdown-item" href="packages-grid.html">Tour Grid</a></li>
                      <li><a class="dropdown-item" href="packages-list.html">Tour List</a></li>
                      <li><a class="dropdown-item" href="tour-search.html">Tour Search</a></li>
                      <li><a class="dropdown-item" href="packages-single.html">Tour Details</a></li>
                    </ul>
                </li>
                <li class="nav-item dropdown"><a href="hotels.html" class="nav-link ">Hotel</a>
          <ul class="dropdown-menu">
                        <li><a class="dropdown-item" href="hotels-grid.html">Hotel Grid</a></li>
                        <li><a class="dropdown-item" href="hotels.html">Hotel Search</a></li>
                    </ul>
        </li>
                <li class="nav-item dropdown"><a href="car-rents-list.html" class="nav-link">Services</a>
                    <ul class="dropdown-menu">
                        <li><a class="dropdown-item" href="car-rents-list.html">Car Rents</a></li>
                        <li><a class="dropdown-item" href="cruise-list.html">Cruise</a></li>
                    </ul>
                </li>
                <li class="nav-item dropdown"><a href="index.html" class="nav-link">Pages</a>
                    <ul class="dropdown-menu">
                        <li class="dropdown"><a class="dropdown-item d-flex justify-content-between" href="index.html">Dropdown</a>
                            <ul class="dropdown-menu">
                                <li><a class="dropdown-item" href="index.html">Lavel 2</a></li>
                                <li><a class="dropdown-item" href="index.html">Lavel 2</a></li>
                                <li><a class="dropdown-item" href="index.html">Lavel 2</a></li>
                            </ul>
                        </li>
                        <li><a class="dropdown-item" href="packages-grid.html">Packages Grid</a></li>
                        <li><a class="dropdown-item" href="packages-list.html">Packages List</a></li>
                        <li><a class="dropdown-item" href="packages-single.html">Single Packages</a></li>
                        <li><a class="dropdown-item" href="blog-grid.html">Blog Grid</a></li>
                        <li><a class="dropdown-item" href="blog-list.html">Blog List</a></li>
                        <li><a class="dropdown-item" href="blog-single.html">Blog Post</a></li>
                        <li><a class="dropdown-item" href="contact.html">Contact</a></li>
                    </ul>
                </li>
                <li class="nav-item dropdown"><a href="blog-grid.html" class="nav-link">Blog</a>
                    <ul class="dropdown-menu">
                        <li><a class="dropdown-item" href="blog-grid.html">Blog Grid</a></li>
                        <li><a class="dropdown-item" href="blog-list.html">Blog List</a></li>
                        <li><a class="dropdown-item" href="blog-single.html">Blog Post</a></li>
                    </ul>
                </li>
                <li class="nav-item"><a href="contact.html" class="nav-link">Contact</a></li>
            </ul>
            <div class="">
                <a href="#" class="btn btn-default book-btn">Book Now</a>
            </div>
        </div>
      </nav><!-- END NAVBAR -->

    </header>

    <router-view/>

        <!--============= { Footer Area } ===========-->
    <footer id="footer-03" class="footer">
      <div class="container">
        <div class="row footer-col-list">
            <div class=" footer-single-col footer_single_col_1">
                <h3 class="subtitle_1"><img src="images/logo.png" alt="SafeTure"></h3>
                <p>Lorem Ipsum has been the industry's standard dummy text scrambled it to make a type specimen book.</p>
                <div class="subscribe-social">
                    <ul class="social-items list-unstyled">
                        <li><a href="#"><i class="fab fa-facebook-f fb-icon"></i></a></li>
                        <li><a href="#"><i class="fab fa-twitter twitt-icon"></i></a></li>
                        <li><a href="#"><i class="fab fa-linkedin-in link-icon"></i></a></li>
                        <li><a href="#"><i class="fab fa-instagram ins-icon"></i></a></li>
                    </ul>
                </div> 
            </div>

            <div class="footer-single-col footer_single_col_2">
                <h3 class="subtitle_1">Link</h3> 
                <ul class="list-unstyled">
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Pages</a></li>
                    <li><a href="#">Hotel</a></li>
                    <li><a href="#">Testimonials</a></li>
                    <li><a href="#">Blog</a></li>
                    <li><a href="#">Contact</a></li>
                </ul>
            </div>

            <div class="footer-single-col footer_single_col_3"> 
                <h3 class="subtitle_1">Support</h3>
                <ul class="list-unstyled">
                    <li><a href="#">Simply</a></li>
                    <li><a href="#">Dummy</a></li>
                    <li><a href="#">Printing</a></li>
                    <li><a href="#">Industry</a></li>                    
                    <li><a href="#">Standard</a></li>
                    <li><a href="#">Galley</a></li>
                </ul>
            </div>
            <div class="footer-single-col footer_single_col_4">
                <h3 class="subtitle_1">Booking</h3>
                <p>Contrary to popular belief, Lorem Ipsum is not simply random text. It has roots classical</p>
            </div>  
        </div>
        <div class="copyright">
            <p> Copyright &copy; 2018, Created  by <span>NajmulHaque</span></p>            
        </div>         
      </div>      
    </footer><!-- ./ End Footer Area-->
  </div>
</template>

<style>
</style>
