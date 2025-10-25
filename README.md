# Bootstrap-Basics-Utilities-Forms-and-Components
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Bootstrap Registration & Data Display</title>
  <!-- Bootstrap CDN -->
  <link
    href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css"
    rel="stylesheet"
  />
</head>
<body>

  <!-- 🔹 Navigation Bar -->
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">My Website</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div id="navbarNav" class="collapse navbar-collapse">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item"><a href="#home" class="nav-link active">Home</a></li>
          <li class="nav-item"><a href="#about" class="nav-link">About</a></li>
          <li class="nav-item"><a href="#contact" class="nav-link">Contact</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- 🔹 Main Container -->
  <div class="container my-5">

    <!-- Part 1: Registration Form -->
    <section id="home">
      <h2 class="mb-4 text-center">User Registration Form</h2>
      <form class="row g-3">
        <div class="col-md-6">
          <label for="firstName" class="form-label">First Name</label>
          <input type="text" class="form-control" id="firstName" placeholder="Enter first name">
        </div>
        <div class="col-md-6">
          <label for="lastName" class="form-label">Last Name</label>
          <input type="text" class="form-control" id="lastName" placeholder="Enter last name">
        </div>
        <div class="col-md-6">
          <label for="email" class="form-label">Email *</label>
          <input type="email" class="form-control is-invalid" id="email" required placeholder="Enter email">
        </div>
        <div class="col-md-6">
          <label for="password" class="form-label">Password *</label>
          <input type="password" class="form-control is-invalid" id="password" required placeholder="Enter password">
        </div>
        <div class="col-12">
          <div class="form-check">
            <input class="form-check-input" type="checkbox" id="terms">
            <label class="form-check-label" for="terms">I agree to the terms and conditions</label>
          </div>
        </div>
        <div class="col-12">
          <button type="submit" class="btn btn-success">Submit</button>
        </div>
      </form>
    </section>

    <!-- Part 2: Table for Displaying Data -->
    <section class="mt-5">
      <h3 class="mb-3 text-center">User Data Table</h3>
      <div class="table-responsive">
        <table class="table table-striped table-hover">
          <thead class="table-dark">
            <tr>
              <th>#</th>
              <th>First Name</th>
              <th>Last Name</th>
              <th>Email</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>1</td><td>John</td><td>Doe</td><td>john@example.com</td>
            </tr>
            <tr>
              <td>2</td><td>Jane</td><td>Smith</td><td>jane@example.com</td>
            </tr>
            <tr>
              <td>3</td><td>Chris</td><td>Brown</td><td>chris@example.com</td>
            </tr>
          </tbody>
        </table>
      </div>
    </section>

  </div>

  <!-- Part 3: Image and Button Utilities -->
  <div class="container-fluid bg-light py-5 text-center">
    <h3>Main Image Section</h3>
    <img src="https://picsum.photos/1200/300" alt="Banner Image" class="img-fluid mb-3">

    <img src="https://picsum.photos/200" alt="Profile" class="rounded-circle mb-4">

    <div>
      <button class="btn btn-primary me-2">Always Visible Button</button>
      <button class="btn btn-warning d-none d-md-inline-block">Hidden on Small Screens</button>
    </div>
  </div>

  <!-- Part 4: Footer -->
  <footer id="contact" class="bg-dark text-white text-center py-3 mt-5">
    <p class="mb-0">&copy; 2025 My Website | Designed with Bootstrap 5</p>
  </footer>

  <!-- Bootstrap JS -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

