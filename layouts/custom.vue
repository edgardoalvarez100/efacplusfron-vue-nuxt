    <template>
  <html lang="en">
    <head>
      <meta charset="utf-8" />
      <meta http-equiv="X-UA-Compatible" content="IE=edge" />
      <meta
        name="viewport"
        content="width=device-width, initial-scale=1, shrink-to-fit=no"
      />
      <meta name="description" content="" />
      <meta name="author" content="" />
      <title>SB Admin 2 - Dashboard</title>

      <link
        href="https://fonts.googleapis.com/css?family=Nunito:200,200i,300,300i,400,400i,600,600i,700,700i,800,800i,900,900i"
        rel="stylesheet"
      />
    </head>

    <body id="page-top">
      <!-- Page Wrapper -->
      <div id="wrapper">
        <Sidebar />

        <!-- Content Wrapper -->
        <div id="content-wrapper" class="d-flex flex-column">
          <!-- Main Content -->
          <div id="content">
            <Topbar />
            <slot />
          </div>
          <!-- End of Main Content -->

          <Footer />
        </div>
        <!-- End of Content Wrapper -->
      </div>
      <!-- End of Page Wrapper -->

      <!-- Scroll to Top Button-->
      <a class="scroll-to-top rounded" href="#page-top">
        <i class="fas fa-angle-up"></i>
      </a>

      <!-- Logout Modal-->
      <div
        class="modal fade"
        id="logoutModal"
        tabindex="-1"
        role="dialog"
        aria-labelledby="exampleModalLabel"
        aria-hidden="true"
      >
        <div class="modal-dialog" role="document">
          <div class="modal-content">
            <div class="modal-header">
              <h5 class="modal-title" id="exampleModalLabel">
                Ready to Leave?
              </h5>
              <button
                class="close"
                type="button"
                data-dismiss="modal"
                aria-label="Close"
              >
                <span aria-hidden="true">×</span>
              </button>
            </div>
            <div class="modal-body">
              Select "Logout" below if you are ready to end your current
              session.
            </div>
            <div class="modal-footer">
              <button
                class="btn btn-secondary"
                type="button"
                data-dismiss="modal"
              >
                Cancel
              </button>
              <a class="btn btn-primary" href="login">Logout</a>
            </div>
          </div>
        </div>
      </div>
    </body>
  </html>
</template>
<style>
</style>

<script>
export default {
  head() {
    return {
      script: [
        { src: "./theme-1/vendor/jquery/jquery.min.js" },
        { src: "./theme-1/vendor/bootstrap/js/bootstrap.bundle.min.js" },
        { src: "./theme-1/vendor/jquery-easing/jquery.easing.min.js" },
        { src: "./theme-1/js/sb-admin-2.min.js" },
        { src: "./theme-1/js/demo/chart-area-demo.js" },
        { src: "./theme-1/js/demo/chart-pie-demo.js" },
      ],
    };
  },
};
</script>