<template>
  <div class="destinations">

  
<!-- Preloader -->
<div id="loader-wrapper">
    <div id="loader"></div>
    <div class="loader-section section-left"></div>
    <div class="loader-section section-right"></div>
</div>
<!--============= { Header } ===========-->
<header id="Packege-grid" class="header inner-pages">
    <nav class="navbar navbar-expand-md navbar-light bg-faded">
        <div class="container">
            <a class="navbar-brand" href="index.html"><img src="images/logo.png" alt="SafeTure"></a>
            <ul class="navbar-nav ml-auto">
                <li class="nav-item dropdown"><a href="index.html" class="nav-link">Home</a>
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
                <li class="nav-item dropdown"><a href="index.html" class="nav-link active">Pages</a>
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
                <li class="nav-item"><a href="contact.html" class="nav-link ">Contact</a></li>
            </ul>
            <div class="">
                <a href="#" class="btn btn-default book-btn">Book Now</a>
            </div>
        </div>
    </nav><!-- END NAVBAR -->        

    <div class="intro-text">
        <div class="container">
            <div class="row">
                <div class="col-md-12">
                    <h1 class="title">Hotels</h1>
                    <div class="page-link">
                        <a href="" title="">Home</a>
                        <a href="" title="">Hotels</a>
                    </div>                    
                </div>
            </div> 
        </div>
    </div>
</header> <!-- End Header -->


<!--============= { Packages Grid Area } ===========-->
<section id="packages_grid_items" class="packages">
    <div class="container">
        <div class="row">        
            <div class="col-sm-12">
                <div class="sub-title">
                    <h2>Top Rated Hotels</h2>
                    <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam</p>
                </div>
            </div>
        </div>
        <div class="row pb-30">
            <div class="col-sm-4 single-package-wrapper rpb" v-for="destination in destinations">
                <div class="singel-packages">
                    <div class="img-wrapper">
                        <a href="" title=""><img src="images/search/hotel-01.jpg" alt=""></a>
                    </div>
                    <div class="packages-title">
                        <div class="title-wrapper">
                            <h3><a href="" title="">Inverlochy Castle Hotel</a></h3>
                            <p>2 days, 3 Nights start from </p>
                        </div> 
                        <div class="packages_details">
                           <span>$120</span>
                           <a href="" class="packages_booking">Book Now</a>
                        </div>   
                    </div>
                </div>   
            </div>            

            <div class="col-sm-4 single-package-wrapper rpb">
                <div class="singel-packages">
                    <div class="img-wrapper">
                        <a href="" title=""><img src="images/search/hotel-02.jpg" alt=""></a>
                    </div>
                    <div class="packages-title">
                        <div class="title-wrapper">
                            <h3><a href="" title="">Patagonia Hotel</a></h3>
                            <p>4 days, 5 Nights start from </p>
                        </div> 
                        <div class="packages_details">
                           <span>$400</span>
                           <a href="" class="packages_booking">Book Now</a>
                        </div>   
                    </div>
                </div>   
            </div>             

            <div class="col-sm-4 single-package-wrapper rpb">
                <div class="singel-packages">
                    <div class="img-wrapper">
                        <a href="" title=""><img src="images/search/hotel-03.jpg" alt=""></a>
                    </div>
                    <div class="packages-title">
                        <div class="title-wrapper">
                            <h3><a href="" title="">La Reserve Hotel</a></h3>
                            <p>4 days, 5 Nights start from </p>
                        </div> 
                        <div class="packages_details">
                           <span>$220</span>
                           <a href="" class="packages_booking">Book Now</a>
                        </div>   
                    </div>
                </div>   
            </div>  
        </div>

        <div class="row pb-30">
            <div class="col-sm-4 single-package-wrapper rpb">
                <div class="singel-packages">
                    <div class="img-wrapper">
                        <a href="" title=""><img src="images/search/hotel-06.jpg" alt=""></a>
                    </div>
                    <div class="packages-title">
                        <div class="title-wrapper">
                            <h3><a href="" title="">San Miguel de</a></h3>
                            <p>4 days, 5 Nights start from </p>
                        </div> 
                        <div class="packages_details">
                           <span>$850</span>
                           <a href="" class="packages_booking">Book Now</a>
                        </div>   
                    </div>
                </div>   
            </div>            

            <div class="col-sm-4 single-package-wrapper rpb">
                <div class="singel-packages">
                    <div class="img-wrapper">
                        <a href="" title=""><img src="images/search/hotel-05.jpg" alt=""></a>
                    </div>
                    <div class="packages-title">
                        <div class="title-wrapper">
                            <h3><a href="" title="">Hotel Wailea</a></h3>
                            <p>2 days, 2 Nights start from </p>
                        </div> 
                        <div class="packages_details">
                           <span>$320</span>
                           <a href="" class="packages_booking">Book Now</a>
                        </div>   
                    </div>
                </div>   
            </div>             

            <div class="col-sm-4 single-package-wrapper rpb">
                <div class="singel-packages">
                    <div class="img-wrapper">
                        <a href="" title=""><img src="images/search/hotel-04.jpg" alt=""></a>
                    </div>
                    <div class="packages-title">
                        <div class="title-wrapper">
                            <h3><a href="" title="">Sheen Falls Lodge</a></h3>
                            <p>2 days, 3 Nights start from </p>
                        </div> 
                        <div class="packages_details">
                           <span>$500</span>
                           <a href="" class="packages_booking">Book Now</a>
                        </div>   
                    </div>
                </div>   
            </div> 
        </div>

        <div class="row pb-30">
            <div class="col-sm-4 single-package-wrapper rpb">
                <div class="singel-packages">
                    <div class="img-wrapper">
                        <a href="" title=""><img src="images/search/hotel-07.jpg" alt=""></a>
                    </div>
                    <div class="packages-title">
                        <div class="title-wrapper">
                            <h3><a href="" title="">Las Ventanas</a></h3>
                            <p>3 days, 4 Nights start from </p>
                        </div> 
                        <div class="packages_details">
                           <span>$280</span>
                           <a href="" class="packages_booking">Book Now</a>
                        </div>   
                    </div>
                </div>   
            </div>            

            <div class="col-sm-4 single-package-wrapper rpb">
                <div class="singel-packages">
                    <div class="img-wrapper">
                        <a href="" title=""><img src="images/search/hotel-08.jpg" alt=""></a>
                    </div>
                    <div class="packages-title">
                        <div class="title-wrapper">
                            <h3><a href="" title="">Fogo Island Inn</a></h3>
                            <p>2 days, 1 Nights start from </p>
                        </div> 
                        <div class="packages_details">
                           <span>$300</span>
                           <a href="" class="packages_booking">Book Now</a>
                        </div>   
                    </div>
                </div>   
            </div> 
      <div class="col-sm-4 single-package-wrapper rpb">
                <div class="singel-packages">
                    <div class="img-wrapper">
                        <a href="" title=""><img src="images/search/hotel-04.jpg" alt=""></a>
                    </div>
                    <div class="packages-title">
                        <div class="title-wrapper">
                            <h3><a href="" title="">The Peninsula</a></h3>
                            <p>4 days, 5 Nights start from </p>
                        </div> 
                        <div class="packages_details">
                           <span>$700</span>
                           <a href="" class="packages_booking">Book Now</a>
                        </div>   
                    </div>
                </div>   
            </div>      
        </div>
    <div class="row">
      <div class="col-sm-4 offset-md-5">
        <nav aria-label="Page navigation">
          <ul class="pagination">
            <li class="page-item">
              <a class="page-link" href="#" aria-label="Previous">
                <span aria-hidden="true"><i class="fa fa-angle-left"></i></span>
                <span class="sr-only">Previous</span>
              </a>
            </li>
            <li class="page-item active"><a class="page-link active" href="#">1</a></li>
            <li class="page-item"><a class="page-link" href="#">2</a></li>
            <li class="page-item"><a class="page-link" href="#">3</a></li>
            <li class="page-item">
              <a class="page-link" href="#" aria-label="Next">
                <span aria-hidden="true"><i class="fa fa-angle-right"></i></span>
                <span class="sr-only">Next</span>
              </a>
            </li>
          </ul>
        </nav>
      </div>
    </div>
    </div>
</section>


<!--============= { Scroll Top Area } ===========-->
<section id="scroll-top" class="scroll-top">
    <div class="container">      
        <div class="row">
            <div class="col-sm-12 d-flex justify-content-end">
                <h2>&nbsp;</h2>
                <div class="to-top pos-rtive">
                    <a href="#"><i class = "fa fa-angle-up"></i></a>
                </div><!-- Scroll to top button end-->
            </div>
        </div>
    </div>
</section>

  </div>
</template>

<style>
</style>

<script>
import axios from "axios";
import Vue2Filters from "vue2-filters";

export default {
  mixins: [Vue2Filters.mixin],
  data: function() {
    return {
      destinations: [],
      id: 221,
      origin: {
        origin_trip_destinys: []
      },
      sortDestinationsBy: "",
    };
  },
  created: function() {
    axios.get("/api/destinations").then(response => {

      this.destinations = response.data;

      this.destinations.forEach((destination) => {
        if (this.$route.query.origin === destination.airport_code) {
          this.id = destination.id;
        }
      });

      axios.get("/api/destinations/" + this.id).then(response => {
        console.log(response.data);
        this.origin = response.data;
      });

      if (this.$route.query.moneyToSpend === 'lotsOfMoney') {
        this.sortDestinationsBy = 'rank';
      } else if (this.$route.query.moneyToSpend === 'budget') {
        this.sortDestinationsBy = 'cheapness';
      } else if (this.$route.query.moneyToSpend === 'mix') {
        this.sortDestinationsBy = 'mix';
      }
    });
  },
  methods: {}
};
</script>