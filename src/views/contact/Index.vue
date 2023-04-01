<template>
    <div class="post-index">
        <!-- header -->
        <Header />
        <!-- end header -->

        <!-- main content -->
        <header class="pt-5 border-bottom bg-light">
            <div class="container pt-md-1 pb-md-1">
                <h1 class="bd-title mt-4 font-weight-bold"><i class="fa fa-phone" aria-hidden="true"></i> KONTAK</h1>
                <p class="bd-lead">Kontak SMK Indonesia.</p>
            </div>
        </header>

        <!-- breadcrumb -->
        <nav aria-label="breadcrumb">
            <ol class="breadcrumb">
                <li class="breadcrumb-item">
                    <router-link :to="{ name: 'home' }" class="text-decoration-none"><i class="fa fa-home"></i> Home
                    </router-link>
                </li>
                <li class="breadcrumb-item">
                    <router-link :to="{ name: 'contact' }" class="text-decoration-none"><i class="fa fa-phone"></i>
                        Kontak</router-link>
                </li>
            </ol>
        </nav>
        <!-- end breadcrumb -->

        <div class="container-fluid mt-5 mb-5">

            <div class="row">
                <div class="col-md-7">
                    <div class="card border-0 shadow-sm rounded">
                        <div class="card-body">
                            <iframe
                                src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d63413.46594457189!2d106.69057555820311!3d-6.604401199999989!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e69c59e57bac1d7%3A0x1943a38308293b61!2sKantor%20MA%20PPIQ!5e0!3m2!1sid!2sid!4v1680386677561!5m2!1sid!2sid"
                                width="100%" height="400" frameborder="0" style="border:0;" allowfullscreen=""
                                aria-hidden="false" tabindex="0"></iframe>
                        </div>
                    </div>
                </div>
                <div class="col-md-5">
                    <div class="card border-0 shadow-sm rounded">
                        <div class="card-body">
                            <h3>KONTAK KAMI</h3>
                            <hr>
                            <p>
                                <i class="fa fa-map-marker" aria-hidden="true"></i> Jl. H. Somad No.140, Pagelaran, Kec. Ciomas, Kabupaten
                            </p>
                            <p>
                                <i class="fas fa-phone"></i> +62180299924
                            </p>
                            <p>
                                <i class="fas fa-phone"></i> +6281210271946
                            </p>
                            <!-- <p>
                                <i class="fas fa-envelope"></i> 
                            </p> -->
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <!-- main content -->

        <!-- footer -->
        <Footer />
        <!-- end footer -->
    </div>
</template>

<script>
    //import component
    import Header from "../../components/Header.vue";
    import Footer from "../../components/Footer.vue";


    export default {
        name: 'ContactComponent',
        components: {
            Header,
            Footer
        }
    }
</script>